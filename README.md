# A3 2026 Leaderboard

Last updated: `April 03, 2026 at 10:03:04 AM ET`

## Pages

- [Official Regimes](official_regimes.md): official per-regime boards using the newest evaluated `submission.py`.
- [Historical Best By Regime](historical_regimes.md): best passing per-regime results across `submission.py` and `develop.py`.
- [Latest Tracking](latest_tracking.md): newest evaluated attempts in round-robin order.

## Official Overall

| rank | nickname | status | commit | runtime_s | score | R1 (tok/s) | R2 (tok/s) | R3 (ms) | R4 (ms) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | - - | evaluated | adc0f3 | 25.6/2.5/28.1 | 1.989 | 591.4 | 386.9 | 21.8 | 44.5 |
| 2 | chyyy | evaluated | 34cc06 | 33.5/2.4/35.9 | 1.918 | 555.7 | 433.8 | 24.8 | 47.6 |
| 3 | gm | evaluated | 540f22 | 21.2/2.7/24.0 | 1.747 | 515.9 | 355.3 | 26.8 | 48.7 |
| 4 | nickname55555555 | evaluated | 99ddc2 | 27.8/2.8/30.6 | 1.633 | 552.2 | 334.1 | 32.4 | 53.0 |
| 5 | andrasferenczy | evaluated | 9c7f53 | 37.3/3.2/40.5 | 1.486 | 539.1 | 277.2 | 31.9 | 63.7 |
| 6 | gravlax | evaluated | b1229d | 19.9/3.2/23.1 | 1.464 | 532.3 | 272.5 | 35.0 | 59.7 |
| 7 | happyface | evaluated | 7e8b61 | 18.5/3.4/22.0 | 1.219 | 543.0 | 258.2 | 63.7 | 66.0 |
| 8 | TA | evaluated | 324cb8 | 19.8/3.5/23.3 | 0.997 | 553.3 | 295.5 | 83.2 | 131.7 |
| 9 | lipphi | evaluated | a3a71b | 40.5/3.6/44.2 | 0.911 | 534.8 | 306.7 | 104.4 | 150.9 |
| 10 | bl792 | evaluated | 9af784 | 18.9/4.2/23.0 | 0.886 | 525.3 | 226.0 | 97.1 | 131.5 |
| 11 | 1_Core_2GHz_Colab_CPU | evaluated | bd9ae0 | 34.9/4.4/39.3 | 0.790 | 558.0 | 221.1 | 160.0 | 131.1 |
| 12 | Shengwei | evaluated | 33733e | 40.6/4.7/45.3 | 0.710 | 543.9 | 224.0 | 238.7 | 132.9 |
| 13 | your_nickname_here | evaluated | f10b9b | 22.4/6.1/28.5 | 0.539 | 557.8 | 173.1 | 308.1 | 246.4 |
|  | abarat007 | failed | 9e63f6 |  |  |  |  |  |  |
|  | ashaikh23 | failed | a5012f |  |  |  |  |  |  |
|  | dhanushikka | failed | 14b1fd |  |  |  |  |  |  |
|  | fishyfins | failed | b8a4a4 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | ishan-pat | failed | acf3d7 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | landrum | failed | b88426 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | prousoglou | failed | f33caa | 0.0/0.0/0.0 |  |  |  |  |  |
|  | tuo | failed | 6ea89f |  |  |  |  |  |  |
|  | yb | failed | 8ca88e | 0.0/0.0/0.0 |  |  |  |  |  |

## Column Guide

- `rank`: placement among passing rows in that table.
- `status`: public state for that row, such as `evaluated`, `failed`, `no_submission`, or `no_repo`.
- `graded_file`: which tracked file produced that result, either `submission.py` or `develop.py`.
- `commit`: short commit hash for the evaluated snapshot. Match it against your GitHub commit history to identify the exact version that produced that result.
- `runtime_s`: compact `setup/run/total` timing in seconds from the evaluator JSON.
- In `runtime_s`, the final `total` value is the timing value that matters for timeout comparisons.
- `score`: official overall score, larger is better.
- `R1` and `R2`: decode throughput in `tok/s`.
- `R3` and `R4`: TTFT in `ms`.

## Notes

- `R1` and `R2` are decode throughput in `tok/s`.
- `R3` and `R4` are TTFT in `ms`.
- Use this page for the official overall board.
- Use `Official Regimes` for official per-regime standings.
- Use `Historical Best By Regime` for progress visibility across both tracked files.
- Use `Latest Tracking` to see the newest evaluated attempts.
- Overall score is larger-is-better and reference-relative.
- `R1_time = 128 / R1_tok_per_s`
- `R2_time = 128 / R2_tok_per_s`
- `R3_time = R3_TTFT_ms`
- `R4_time = R4_TTFT_ms`
- `score = (ref_R1 / R1_time * ref_R2 / R2_time * ref_R3 / R3_time * ref_R4 / R4_time)^(1/4)`
- A score of `1.0` matches the reference implementation overall.
- The reference implementation is a fixed baseline for normalization, not an optimized ceiling.
- Public outputs show only nickname, commit hash, status, and metrics.
- Official views use the newest evaluated `submission.py` only.
- Historical per-regime views use the best passing result across `submission.py` and `develop.py`.
