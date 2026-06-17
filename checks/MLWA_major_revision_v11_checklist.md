# MLWA/Q1 revision v11 checklist

## Main changes from v10

- Added focused V11 process-control experiments for the central reviewer concern.
- Moved the process/order claim closer to the main result rather than treating it as peripheral validation.
- Sharpened novelty framing: benchmarking protocol and empirical process-dependence result, not a new robustness theory or new interaction statistic.
- Added Macro-F1 process-control table and figure.
- Added composition diagnostics showing the clean-label control retains more clean minority evidence.
- Rewrote abstract, highlights, contributions, discussion, threats to validity, and conclusion to avoid overclaiming.
- Explicitly states that the strong effect is tied to observed corrupted labels defining the imbalance sampling frame.
- Added limits for naturally occurring noise, real selection bias, high-cardinality categorical data, time-dependent data, semi-supervised settings, and intertwined pipelines.
- Keeps missingness as secondary rather than the main scientific claim.

## Key V11 process-control results

| Process variant | Macro-F1 interaction | Dataset-clustered 95% CI |
|---|---:|---:|
| Original: noise then observed-label imbalance | +0.184 | [0.136, 0.232] |
| Clean-label imbalance then noise | +0.023 | [0.007, 0.037] |
| Fixed retained-index control | +0.225 | [0.167, 0.285] |
| Equal-training-size control | +0.166 | [0.121, 0.213] |

## Remaining author-side tasks

- Replace anonymous author block if the target journal is not double-blind.
- Insert final public or anonymous-review repository/archive URL if available.
- Confirm journal formatting requirements before submission.
