# AlmaLinux 8 PBS trace sweep

Date: 2026-05-18 PDT

Image: `almalinux:8.10-20260509`

Python: `/usr/libexec/platform-python` (`Python 3.6.8`)

Branch under test: `bounty-355-safe-yaml-literals` at qtop PR #362 head `f1f926b`.

Command shape per sample:

```bash
/usr/libexec/platform-python -m qtop_py.cli -b pbs -s /work/results/<sample> -c ON
```

Pass condition: exit code `0` and non-empty stdout.

Result: `447/447` PBS trace directories passed (`100.00%`).

Files:

- `summary.txt`: aggregate result.
- `sweep.csv`: per-sample status, exit code, stdout byte count, and stderr byte count.
