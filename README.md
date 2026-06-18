# Value-Hijacking: Data Selectors as Poisoning Amplifiers in LLM Fine-Tuning Supply Chains — Artifact

This repository hosts the supplementary material, configurations, and result tables
for the PVLDB submission *Value-Hijacking: Data Selectors as Poisoning Amplifiers in
LLM Fine-Tuning Supply Chains*.

The paper keeps the core results in its 12 pages and points here for full
configurations and supporting tables. The mapping below shows where each in-paper
pointer resolves.

## Where the paper points here

| In the paper | Provided in this repo |
|---|---|
| §4.1 / §4.4 / §7 — "trained-generator wrapper (full results in the artifact repository)" | [SUPPLEMENTARY.md → Trained-Generator Wrapper](SUPPLEMENTARY.md#trained-generator-wrapper) |
| §5.3 — "the confusion matrix and full sampling composition are provided in the artifact repository" | [SUPPLEMENTARY.md → Evaluation Protocol & Human Validation](SUPPLEMENTARY.md#evaluation-protocol-and-human-validation) |
| §5.5 — "the full BIDS, IFD-transfer, and DEITA chains are provided in the artifact repository" | [SUPPLEMENTARY.md → Cross-Selector Full Chains](SUPPLEMENTARY.md#cross-selector-full-chains) |
| §7 — "the K-sweep diagnostic (provided in the artifact repository)" | [SUPPLEMENTARY.md → K-Sweep Diagnostic](SUPPLEMENTARY.md#k-sweep-and-selection-budget-diagnostics) |
| Reproducibility (PVLDB availability requirement) | [SUPPLEMENTARY.md → AMRS Reproducibility Details](SUPPLEMENTARY.md#amrs-reproducibility-details) |

## Contents

- `SUPPLEMENTARY.md` — full judge protocol, HumanAudit-400 tables, cross-selector
  ablation chains, trained-generator wrapper, K-sweep, and reproducibility configs.
- `code/` — evaluation code, GPT-judge prompts, sanitized experimental configs
  *(add your existing code here)*.

## Reproducibility note

Per PVLDB policy, we release evaluation code, GPT-judge prompts, sanitized
experimental configurations, and aggregate result files. We do **not** release
optimized poisoned datasets directly; anchor-extraction and candidate-generation
code are released in a form that supports defense research (testing selector
robustness under adaptive attacks) rather than enabling turnkey attacks.

## Citation

> Yahao Ren, Jiawei Duan, and Huadi Zheng. Value-Hijacking: Data Selectors as
> Poisoning Amplifiers in LLM Fine-Tuning Supply Chains. PVLDB, 20(1), 2027.
