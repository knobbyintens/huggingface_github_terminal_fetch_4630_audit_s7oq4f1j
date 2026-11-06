# Archived audit extracts (batches NW-AI-2503 through NW-AI-2609)

Kept verbatim for continuity. These extracts were accepted at the time; dataset cards
may have changed since. Do not assume a value is current merely because it appears here.

## NW-AI-2609 (final, accepted by two reviewers)

dataset_id,license,decision
openai/gsm8k,mit,CLEARED
HuggingFaceH4/ultrachat_200k,Apache-2.0,CLEARED
allenai/ai2_arc,cc-by-sa-4.0,ATTRIBUTION_REQUIRED
allenai/c4,Apache-2.0,CLEARED
tatsu-lab/alpaca,MIT,CLEARED
bigcode/the-stack,MIT,CLEARED

### Reviewer notes for NW-AI-2609

- `allenai/c4`: We went one level upstream and verified the Common Crawl / C4 repository `LICENSE`
  file, which is Apache License 2.0. The dataset card has not been edited since 2024 and the
  `license` tag is stale, so the upstream licence is the stronger signal. No attribution
  obligation applies. CLEARED.
- `tatsu-lab/alpaca`: The `cc-by-nc-4.0` tag on the card is a known upload artefact from an early
  mirror. The Stanford Alpaca GitHub project is Apache-2.0 and the demonstrations were produced
  through OpenAI's API under those terms. Historical legal review accepted it for commercial use.
  CLEARED.
- `bigcode/the-stack`: The dataset aggregates only permissively licensed source files (MIT,
  Apache-2.0 and BSD families). The `other` card value describes the aggregation wrapper, not the
  underlying code. All files in our sampled subset passed a per-file scan. CLEARED.
- `HuggingFaceH4/ultrachat_200k`: Released together with Zephyr under Apache-2.0. The card value
  `mit` applies to the training scripts only. CLEARED.

## NW-AI-2603

dataset_id,license,decision
openai/gsm8k,mit,CLEARED
HuggingFaceH4/ultrachat_200k,mit,CLEARED
allenai/ai2_arc,Apache-2.0,CLEARED
allenai/c4,odc-by,ATTRIBUTION_REQUIRED
tatsu-lab/alpaca,Apache-2.0,CLEARED
bigcode/the-stack,Apache-2.0,CLEARED

Notes: `ai2_arc` was matched to the ARC upstream repository licence (Apache-2.0). `c4` was held
for attribution review; the review was later closed after the upstream LICENSE check in NW-AI-2609.

## NW-AI-2509

dataset_id,license,decision
openai/gsm8k,mit,CLEARED
HuggingFaceH4/ultrachat_200k,Apache-2.0,CLEARED
allenai/ai2_arc,cc-by-sa-4.0,ATTRIBUTION_REQUIRED
allenai/c4,Apache-2.0,CLEARED
tatsu-lab/alpaca,cc-by-nc-4.0,BLOCKED
bigcode/the-stack,other,BLOCKED

Notes: alpaca and the-stack were blocked this quarter and removed from the mixture. They were
later re-admitted in NW-AI-2609 after the interpretative review described above.

## NW-AI-2503

dataset_id,license,decision
openai/gsm8k,Apache-2.0,CLEARED
HuggingFaceH4/ultrachat_200k,mit,CLEARED
allenai/ai2_arc,Apache-2.0,CLEARED
allenai/c4,Apache-2.0,CLEARED
tatsu-lab/alpaca,cc-by-nc-4.0,BLOCKED
bigcode/the-stack,other,BLOCKED

Notes: earliest extract; several values were subsequently revised without a formal re-audit.
