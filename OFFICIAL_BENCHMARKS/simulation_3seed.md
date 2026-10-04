# 3-Seed Simulation — K_PFLFL

**Seeds:** `13119` · `44456` · `78655`

**Seed method:** `sha256("K_PFLFL")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_PFLFL`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.1033 | 0.0146 | ±0.0286 |
| throughput_tokens_per_sec | 5588.4667 | 25.7858 | ±50.5402 |
| p50_latency_ms | 43.0233 | 2.4654 | ±4.8322 |
| p99_latency_ms | 99.0167 | 1.5085 | ±2.9567 |
| ttft_ms | 30.7633 | 4.2379 | ±8.3063 |
| mmlu_proxy | 0.6999 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.763 | 0.0168 | ±0.0329 |
| truthfulqa_proxy | 0.6368 | 0.0145 | ±0.0284 |
| arc_proxy | 0.7357 | 0.0159 | ±0.0312 |
| complexity_cyclomatic | 3.6333 | 0.0377 | ±0.0739 |
| maintainability_index | 72.4933 | 4.3511 | ±8.5282 |
| security_issues_high | 1.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 84.1 | 2.5456 | ±4.9894 |
| test_coverage_pct | 52.9333 | 0.2357 | ±0.462 |
| doc_coverage_pct | 59.1333 | 2.3099 | ±4.5274 |
| memory_mb | 1095.8 | 35.0725 | ±68.7421 |
| gpu_util_pct | 66.7667 | 2.7341 | ±5.3588 |
| openssf_score | 7.1067 | 0.3441 | ±0.6744 |
| eu_ai_act_compliance_pct | 81.1 | 0.5657 | ±1.1088 |
| slsa_level | 1.0 | 0.0 | ±0.0 |

## Per-Seed Raw Results

| Metric | Seed 13119 | Seed 44456 | Seed 78655 |
|--------|------------|------------|------------|
| trl_score | 7.093 | 7.124 | 7.093 |
| throughput_tokens_per_sec | 5606.7 | 5552.0 | 5606.7 |
| p50_latency_ms | 41.28 | 46.51 | 41.28 |
| p99_latency_ms | 97.95 | 101.15 | 97.95 |
| ttft_ms | 33.76 | 24.77 | 33.76 |
| mmlu_proxy | 0.6999 | 0.6998 | 0.6999 |
| hellaswag_proxy | 0.7749 | 0.7392 | 0.7749 |
| truthfulqa_proxy | 0.6471 | 0.6163 | 0.6471 |
| arc_proxy | 0.7469 | 0.7132 | 0.7469 |
| complexity_cyclomatic | 3.66 | 3.58 | 3.66 |
| maintainability_index | 75.57 | 66.34 | 75.57 |
| security_issues_high | 2 | 1 | 2 |
| dependency_freshness_pct | 82.3 | 87.7 | 82.3 |
| test_coverage_pct | 53.1 | 52.6 | 53.1 |
| doc_coverage_pct | 57.5 | 62.4 | 57.5 |
| memory_mb | 1120.6 | 1046.2 | 1120.6 |
| gpu_util_pct | 68.7 | 62.9 | 68.7 |
| openssf_score | 7.35 | 6.62 | 7.35 |
| eu_ai_act_compliance_pct | 80.7 | 81.9 | 80.7 |
| slsa_level | 1 | 1 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._