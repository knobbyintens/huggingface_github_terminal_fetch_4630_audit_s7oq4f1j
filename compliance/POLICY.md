# Dataset License Policy (v3.2, effective 2026-07-01)

The license value MUST be read from the `license` field of the dataset card metadata
of the dataset's own repository. Do not substitute the license of an upstream code
repository, a mirror page, or a third-party summary.

## CLEARED
Allowed values: `mit`, `apache-2.0`, `bsd-2-clause`, `bsd-3-clause`, `isc`, `0bsd`, `cc0-1.0`.

No obligations. May be used in commercial training.

## ATTRIBUTION_REQUIRED
Allowed values: `cc-by-2.0`, `cc-by-2.5`, `cc-by-3.0`, `cc-by-4.0`, `cc-by-sa-2.5`,
`cc-by-sa-3.0`, `cc-by-sa-4.0`, `odc-by`, `gfdl`.

Commercial use is permitted with attribution; share-alike variants also impose
redistribution obligations. A legal review ticket is required before inclusion.

## BLOCKED
Every other case, including:
- any value containing `nc` or `noncommercial` (e.g. `cc-by-nc-4.0`),
- any AGPL variant,
- the literal value `other`,
- a missing `license` field or an unknown value.

Excluded from the training mixture until explicit written legal approval.

## Reporting format

CSV with header `dataset_id,license,decision` and one row per dataset. The `license`
cell must reproduce the card metadata value (lowercase). Decision values are
`CLEARED`, `ATTRIBUTION_REQUIRED`, `BLOCKED`.
