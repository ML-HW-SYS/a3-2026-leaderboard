# A3 2026 Leaderboard

Last updated: `March 21, 2026 at 01:10:51 AM ET`

## Pages

- [Official Regimes](official_regimes.md): official per-regime boards using the newest evaluated `submission.py`.
- [Historical Best By Regime](historical_regimes.md): best passing per-regime results across `submission.py` and `develop.py`.
- [Latest Tracking](latest_tracking.md): newest evaluated attempts in round-robin order.

## Official Overall

| rank | nickname | status | commit | runtime_s | score | R1 (tok/s) | R2 (tok/s) | R3 (ms) | R4 (ms) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | TA | evaluated | 324cb8 | 19.8/3.5/23.3 | 0.997 | 553.3 | 295.5 | 83.2 | 131.7 |
|  | nickname55555555 | failed | 847a3d | 0.0/0.0/0.0 |  |  |  |  |  |

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
