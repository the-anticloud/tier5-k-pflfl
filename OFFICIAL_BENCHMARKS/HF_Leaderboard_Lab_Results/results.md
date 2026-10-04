# HF_Leaderboard_Lab_Results

**Project:** `K_PFLFL`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `adap/flower`  
**Commit:** `3bb1dcf78b2c`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **48.81 ms** |
| Min latency | 43.21 ms |
| Max latency | 55.53 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **38** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5899 |
| Classification latency | 273.48 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_PFLFL (adap/flower) — 3256 files, 334427 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'p', '##fl', '##fl', '(', 'ada', '##p', '/', 'flower', ')', '—', '325', '##6', 'files', ',', '334', '##42', '##7']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_