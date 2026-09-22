# MLX MTP flywheel: Day-28 negative result

This public record reports the outcome of a 28-day, single-user experiment with a local Qwen-family MLX target and an MTP drafter. The preregistered primary question was whether mean speculative-token acceptance on a frozen 20-prompt personal holdout would rise by at least 10 percentage points above Day 0.

**It did not.** Day 0 was 57.63%; Day 28 was **56.935%** (20/20 prompts completed), against a registered **67.63%** target. The observed change was approximately **−0.695 percentage points**. No trained drafter was promoted.

The Day-28 incumbent stock suite measured **55.741667%** mean acceptance across **24/24** successful prompts, above its applicable **48.55%** floor. That is a passing result for that day's stock-suite row only. The series was not measured on Day 7, Day 14 or Day 21, so the planned weekly-continuity criterion remains **unestablished**. The separate 169-prompt candidate referee was **not run** during the Day-28 window and has no Day-28 candidate verdict.

## Method and scope

The primary curve used the same 20-prompt holdout, stock drafter, block size 5, 256-token cap and temperature-zero recipe across its recorded points. A service snapshot/restore bundle was recorded on Day 28, but its reported completion includes assertions of owner review and chat-request smoke checks that lack independent support in the operator log. We do not call service restoration fully attested on that basis. The curve and weekly numerical rows do not depend on those assertions.

A later audit found that the target's chat template rendered user content twice inside a Python-list-like representation. Both sides of the paired comparisons received the same rendering, so the within-recipe result stands, but absolute acceptance rates do **not** describe ordinary single-render prompts. Day 0 did not record a full generation-environment stamp; a subsequent stack change is a plausible cause of the Day-0 to Day-9 shift and limits cross-date attribution.

This is a bounded negative result for this target, drafter, training path, prompt distribution and measurement recipe. It does not show that every personalized drafter or speculative-decoding method fails. Separate work on a served block-size policy measured a favorable short-prompt speed contrast; it is not a positive Day-28 training result and has separate output-correctness and deployment gates.

## Public evidence boundary

The source repository and raw personal prompts are private. This publication gives aggregate outcomes, method constraints and SHA-256 checksums of retained raw artifacts. The raw rows are not publicly available, so an independent reader cannot recompute the numerical summaries from this repository alone. No model weights, customer text, personal prompt IDs, machine paths, or per-request traces are redistributed.

| Retained artifact | SHA-256 |
| --- | --- |
| Day-28 curve raw rows | `e898581ce6cb152100732c6c2d00052d17bed5a639a6bb5f5888f3ccf91d7d17` |
| Day-28 curve summary | `b9ff4dbbb1c47843bb770ce991be0c9250bbf84aa9fe29c91a3e7f9200e456d7` |
| Day-28 weekly stock-suite raw rows | `d7031cfcb6dfa3992fd0033e0012adbad0d9ff610f951523077c8154f8336dc4` |
| Day-28 weekly decision | `ad01cdfd19287781078e05c744999b2de70c77d581235f0f48634b04c72a9578` |

Recorded dates: Day 0, 2026-08-25; Day 28, 2026-09-22. The outcome was established before this public report. This repository contains no replacement data for missed days and no invented candidate measurement.

## Citation

QEbellavita. *MLX MTP flywheel: Day-28 negative result.* 2026-09-22. [Version 1 release](https://github.com/QEbellavita/mlx-mtp-day28-negative/releases/tag/v1.0.0).

Text in this public report is available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This license applies to this report only; it grants no rights to private datasets, models or third-party software.
