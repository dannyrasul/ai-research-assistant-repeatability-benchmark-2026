---
license: other
task_categories:
- text-retrieval
language:
- en
tags:
- artificial-intelligence
- information-retrieval
- reproducibility
- research-assistants
pretty_name: AI Research Assistant Repeatability Benchmark 2026
size_categories:
- n<1K
---

# AI Research Assistant Repeatability Benchmark 2026

This dataset contains 15 run-level observations from a three-run comparison of five AI research assistants: ResearchRabbit, Elicit, Scite, Consensus and Undermind.

The benchmark tested whether repeated runs of the same higher-education research question produced consistent, traceable and accessible results. It records result-volume changes, access barriers, completion failures, sampled claim-to-source checks and preserved evidence URLs. It is not a vendor ranking.

## Canonical methodology

The complete testing protocol, evidence labels, disclosure rules and reusable workbook are published by [AI News & Updates](https://ainewsandupdates.com/how-we-review-ai-tools/).

- [Download the transparent review workbook](https://ainewsandupdates.com/wp-content/uploads/2026/07/AI-News-and-Updates-Transparent-AI-Tool-Review-Rubric.xlsx)
- [Download the compact protocol PDF](https://ainewsandupdates.com/wp-content/uploads/2026/07/AI-News-and-Updates-Transparent-AI-Tool-Review-Rubric.pdf)

## Benchmark question

For university or college students, does retrieval practice or practice testing improve retention after at least 24 hours compared with rereading or restudy?

## Method

- Testing date: 1 August 2026.
- Account context: the disclosed free or limited-access mode available to the reviewer.
- Repeats: three matched attempts per product.
- Human review: access barriers and obvious off-topic retrieval failures were logged rather than silently discarded.
- Evidence: public result URLs are included where available. Blank URLs indicate that only a local export was preserved.

## Data fields

- `tool`, `trial`, `test_date`, `account_tier_mode`: run identity and access context.
- `completion_status`: complete, partial or blocked.
- `reported_result_count`: count claimed or displayed by the product.
- `accessible_result_count`: records visibly accessible during the run.
- `full_text_count`: full-text records reported where the product exposed this value.
- `claim_source_checks`: sampled claims manually checked against source records.
- `failure_flag`, `access_barrier`: observed failure or access limitation.
- `elapsed_minutes`: hands-on elapsed time recorded in the review workbook.
- `evidence_url`, `observation`: preserved evidence and a concise factual note.

Blank values mean that the product did not expose the metric or that it was not measured. They do not mean zero.

## Limitations

- This is a small, dated, free-tier benchmark using one research question.
- Product indexes, ranking systems, models, prices and account limits can change.
- Result counts are not directly comparable across products because each interface defines and exposes results differently.
- Some evidence URLs may require an account or may change over time.
- The benchmark does not establish clinical, educational or commercial superiority.

## Attribution and reuse

Published by AI News & Updates. Reuse is permitted with attribution to the dataset and the canonical methodology page. For corrections, contact hello@ainewsandupdates.com.

Suggested attribution: AI News & Updates (2026), “AI Research Assistant Repeatability Benchmark 2026,” https://ainewsandupdates.com/how-we-review-ai-tools/.
