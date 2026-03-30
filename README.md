# A3 2026 Leaderboard

Last updated: `March 30, 2026 at 08:55:51 AM ET`

## Pages

- [Official Regimes](official_regimes.md): official per-regime boards using the newest evaluated `submission.py`.
- [Historical Best By Regime](historical_regimes.md): best passing per-regime results across `submission.py` and `develop.py`.
- [Latest Tracking](latest_tracking.md): newest evaluated attempts in round-robin order.

## Official Overall

| rank | nickname | status | commit | runtime_s | score | R1 (tok/s) | R2 (tok/s) | R3 (ms) | R4 (ms) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | - - | evaluated | adc0f3 | 25.6/2.5/28.1 | 1.989 | 591.4 | 386.9 | 21.8 | 44.5 |
| 2 | nickname55555555 | evaluated | 99ddc2 | 27.8/2.8/30.6 | 1.633 | 552.2 | 334.1 | 32.4 | 53.0 |
| 3 | gravlax | evaluated | b1229d | 19.9/3.2/23.1 | 1.464 | 532.3 | 272.5 | 35.0 | 59.7 |
| 4 | chyyy | evaluated | e845c2 | 39.4/3.3/42.7 | 1.149 | 554.7 | 295.4 | 56.9 | 109.3 |
| 5 | gm | evaluated | c64be1 | 29.1/3.2/32.3 | 1.115 | 524.0 | 335.4 | 62.2 | 121.2 |
| 6 | TA | evaluated | 324cb8 | 19.8/3.5/23.3 | 0.997 | 553.3 | 295.5 | 83.2 | 131.7 |
| 7 | lipphi | evaluated | a3a71b | 40.5/3.6/44.2 | 0.911 | 534.8 | 306.7 | 104.4 | 150.9 |
| 8 | your_nickname_here | evaluated | f10b9b | 22.4/6.1/28.5 | 0.539 | 557.8 | 173.1 | 308.1 | 246.4 |
|  | dhanushikka | failed | 14b1fd |  |  |  |  |  |  |
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
