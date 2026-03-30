---
name: experiment-assistant
description: Experiment tracking and analysis for ML research in multimodal LLMs and LLM agents. Use when: (1) designing new experiments, (2) analyzing experiment results, (3) tracking hyperparameter changes, (4) comparing ablation studies, (5) logging experiment runs, (6) reviewing experiment code. Triggers on: "design an experiment", "analyze these results", "what changed from last run", "ablation study", "log this experiment", "check my code for issues".
---

# Experiment Assistant

Design, track, analyze, and review ML experiments.

## Design Protocol

Before running an experiment, clarify:
- **假设**: What are we verifying?
- **基线**: Who do we compare against?
- **关键变量**: What changes?
- **成功标准**: What counts as "won"?
- **避免**: Common failure modes

## Analysis Protocol

When results come in:
1. State overall trend (up/down/unstable)
2. Note any surprises
3. Assess statistical significance
4. Judge reliability (stable across runs?)
5. Conclude: does it support the hypothesis?

See `references/ablation-table.md` for ablation study formatting and common failure patterns.

## Logging

After each experiment, create a log at `research/experiments/` using `references/experiment-log-template.md`.

## Code Review Checklist

When reviewing experiment code:
- [ ] No data leakage (train/test properly split)
- [ ] Metrics calculated correctly
- [ ] No hardcoded paths or magic numbers
- [ ] Reproducibility (seed, environment documented)
