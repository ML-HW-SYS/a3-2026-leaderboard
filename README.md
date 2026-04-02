# A3 2026 Leaderboard

Last updated: `April 02, 2026 at 03:20:08 PM ET`

## Pages

- [Official Regimes](official_regimes.md): official per-regime boards using the newest evaluated `submission.py`.
- [Historical Best By Regime](historical_regimes.md): best passing per-regime results across `submission.py` and `develop.py`.
- [Latest Tracking](latest_tracking.md): newest evaluated attempts in round-robin order.

## Official Overall

| rank | nickname | status | commit | runtime_s | score | R1 (tok/s) | R2 (tok/s) | R3 (ms) | R4 (ms) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | - - | evaluated | adc0f3 | 25.6/2.5/28.1 | 1.989 | 591.4 | 386.9 | 21.8 | 44.5 |
| 2 | chyyy | evaluated | 34cc06 | 33.5/2.4/35.9 | 1.918 | 555.7 | 433.8 | 24.8 | 47.6 |
| 3 | gm | evaluated | 0c2fc9 | 50.7/2.7/53.5 | 1.746 | 518.1 | 355.8 | 26.9 | 48.9 |
| 4 | nickname55555555 | evaluated | 99ddc2 | 27.8/2.8/30.6 | 1.633 | 552.2 | 334.1 | 32.4 | 53.0 |
| 5 | gravlax | evaluated | b1229d | 19.9/3.2/23.1 | 1.464 | 532.3 | 272.5 | 35.0 | 59.7 |
| 6 | TA | evaluated | 324cb8 | 19.8/3.5/23.3 | 0.997 | 553.3 | 295.5 | 83.2 | 131.7 |
| 7 | happyface | evaluated | ca7f90 | 36.1/3.9/40.1 | 0.927 | 541.5 | 244.1 | 94.2 | 126.1 |
| 8 | lipphi | evaluated | a3a71b | 40.5/3.6/44.2 | 0.911 | 534.8 | 306.7 | 104.4 | 150.9 |
| 9 | tuo | evaluated | 4735b8 | 60.3/5.0/65.4 | 0.686 | 460.6 | 197.3 | 168.0 | 161.7 |
| 10 | your_nickname_here | evaluated | f10b9b | 22.4/6.1/28.5 | 0.539 | 557.8 | 173.1 | 308.1 | 246.4 |
|  | andrasferenczy | failed | 43dff4 | 19.4/4.0/23.4 |  |  |  |  |  |
|  | ashaikh23 | failed | a5012f |  |  |  |  |  |  |
|  | dhanushikka | failed | 14b1fd |  |  |  |  |  |  |
|  | fishyfins | failed | b8a4a4 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | ishan-pat | failed | acf3d7 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | landrum | failed | b88426 | 0.0/0.0/0.0 |  |  |  |  |  |
|  | Shengwei | failed | aba515 |  |  |  |  |  |  |

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
