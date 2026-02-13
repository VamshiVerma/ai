# LineLock Pilot (Fork Benchmark)

Date: 2026-02-13

This branch records a LineLock fork benchmark for this repository.

## Source incidents

- https://github.com/vercel/ai/issues/12052
- https://github.com/vercel/ai/issues/11413

## Pilot result snapshot

- Replay exit code: `1` (expected; regression case is included)
- True block rate: `1.00`
- False block rate: `0.00`
- Confusion matrix: `TP=1 FP=0 TN=1 FN=0`

## Why this matters

This shows deterministic pre-merge blocking for issue-shaped tool-stream regressions while preserving pass behavior on control cases.

## Next step in this fork

1. Add `.linelock/` contract/suite/baseline assets for this repo.
2. Add `.github/workflows/linelock-gate.yml` as a required check candidate.
3. Run weekly and track true/false block outcomes.
