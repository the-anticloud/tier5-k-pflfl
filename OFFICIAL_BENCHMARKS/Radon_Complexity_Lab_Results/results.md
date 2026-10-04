# Radon_Complexity_Lab_Results
**Project:** `K_PFLFL` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 2.156862745098039}`
- **complexity_grade:** `A`
- **complexity_score:** `2.156862745098039`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PFLFL\UPSTREAM\.agents\skills\flower-release-changelog\sc`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PFLFL\UPSTREAM\.agents\skills\flower-release-changelog\scripts\validate_release_changelog.py
    F 45:0 validate - D (21)
    F 23:0 parse_prs - B (6)
    F 94:0 main - A (5)
    F 36:0 section_body - A (3)
    F 89:0 format_prs - A (2)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PFLFL\UPSTREAM\agent\docs\source\conf.py
    F 37:0 _substitute_version_in_code - A (1)
    F 44:0 setup - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PFLFL\UPSTREAM\baselines\niid_bench\run_exp.py
    F 16:0 get_commands - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PFLFL\UPSTREAM\baselines\dasha\dasha\client.py
    M 59:4 CompressionClient._set_parameters - B (6)
    C 19:0 CompressionClient - A (4)
    M 118:4 _GradientCompressionClient.evaluate - A (3)
    C 150:0 _BaseDashaClient - A (3)
    C 159:0 DashaClient - A (3)
    M 172:4 DashaClient._compression_step - A (3)
    C 188:0 MarinaClient - A (3)
    M 213:4 _StochasticGradientCompressionClient.__init__ - A (3)
    M 261:4 _StochasticGradientCompressionClient.evaluate - A (3)
    C 323:0 StochasticDashaClient - A (3)
    M 340:4 StochasticDashaClient._stochastic_compression_step - A (3)
    C 364:0 StochasticMarinaClient - A (3)
    M 29:4 CompressionClient.__init__ - A (2)
    M 51:4 CompressionClient.get_parameters - A (2)
    M 78:4 CompressionClient._get_current_gradients - A (2)
    C 93:0 _GradientCompress
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_