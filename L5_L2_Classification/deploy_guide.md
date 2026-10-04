# Deploy Guide — K_PFLFL
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, PyTorch 2.10+, Opacus (differential privacy), PySyft, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PyTorch 2.10+, Opacus 1.4+, PySyft 0.8+. T4 GPU per node.

## Environment
T4 GPU per node. Coordinator: 16GB RAM, no GPU required. Nodes communicate over LAN only.

## AIOSS Integration
```bash
aioss init --module K_PFLFL --output ./k_pflfl.aioss
aioss append --chain ./k_pflfl.aioss --payload ./output.bin --module K_PFLFL
aioss verify --chain ./k_pflfl.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_PFLFL",
    aioss_chain="./K_PFLFL.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_PFLFL.aioss --verbose
python -m K_PFLFL.tests.smoke
```
