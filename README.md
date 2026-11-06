# Aurora Labs — Data Compliance Ledger

This repository is the internal ledger for dataset licensing decisions in the Aurora training stack.
It is maintained by the data-compliance group.

## Workflow

1. Every quarter a tracking issue is opened for the new onboarding batch.
2. Each dataset entering the training mixture is classified under `compliance/POLICY.md`.
3. The accepted batch report is stored under `compliance/audits/`.
4. One blocker or review ticket is opened for each dataset that is not cleared.

## Snapshot carried over from batch NW-AI-2609 (awaiting re-verification)

| dataset | license (last audit) | decision | note |
|---|---|---|---|
| openai/gsm8k | MIT | CLEARED | stable |
| HuggingFaceH4/ultrachat_200k | Apache-2.0 | CLEARED | tag drift suspected |
| allenai/ai2_arc | CC-BY-SA-4.0 | ATTRIBUTION_REQUIRED | attribution notice filed |
| allenai/c4 | Apache-2.0 | CLEARED | verified against upstream LICENSE |
| tatsu-lab/alpaca | MIT | CLEARED | inherited from Stanford Alpaca |
| bigcode/the-stack | MIT | CLEARED | permissive-only code corpus |

> **Standing note (kept since batch NW-AI-2603):** `allenai/c4` is Apache-2.0. We checked the upstream
> repository licence file and closed the review ticket; no attribution obligation applies. Use this
> value in downstream reports unless legal says otherwise.

## Archive

Historical extracts for earlier batches are in `archive/prior_audit_batches.md`.
