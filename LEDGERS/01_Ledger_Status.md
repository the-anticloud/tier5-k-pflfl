# Ledger Status

**Project:** `K_PFLFL`  
**Tier:** TIER_5_WORLD_NEURO_EMBODIED  
**Identity:** Upstream `adap/flower` @ `3bb1dcf78b2c` (Apache-2.0)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `adap/flower` |
| Commit | `3bb1dcf78b2c4c50d1216c31bb2fdc401748218a` |
| Upstream licence | Apache-2.0 |
| Licence class | permissive |
| Clone size | 133.39 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1000.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
