# Developer Cookbook — K_PFLFL
**Stack:** Python 3.11, PyTorch 2.10+, Opacus (differential privacy), PySyft, PAX 27B, AIOSS_FORMAT
**Domain:** PFLFL: privacy-preserving federated learning with formal guarantees for Anticloud

## Federated training coordinator
```python
from k_pflfl import FederatedCoordinator

coord = FederatedCoordinator(
    global_model="./pax-27b-q4.gguf",
    dp_epsilon=1.0, dp_delta=1e-5,
    n_rounds=50,
    aioss_chain="./pflfl.aioss"
)

coord.register_node("hospital_01", endpoint="192.168.1.101:9000")
coord.register_node("hospital_02", endpoint="192.168.1.102:9000")

for round_result in coord.train():
    print(f"Round {round_result.round}: loss={round_result.loss:.4f}, "
          f"DP budget used: epsilon={round_result.epsilon_used:.3f}")
print(f"Final model: {coord.final_model_path}")
```

## Node (runs at each site)
```python
from k_pflfl import FederatedNode
node = FederatedNode(local_model="./local_pax.gguf", local_data="./patient_data/",
                     dp_noise_multiplier=1.1)
node.connect("192.168.1.100:8000")  # coordinator LAN IP
node.run()
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
