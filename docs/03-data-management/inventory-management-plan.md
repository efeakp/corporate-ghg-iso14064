# GHG inventory management plan

*ISO 14064-1:2018, clause 8*

## Annual cycle

| Month (FY end + n) | Activity | Owner | Output |
|---|---|---|---|
| −2 | Review boundary, source register and significance assessment | Inventory manager | Updated registers |
| −1 | Brief data owners; issue data requests | Inventory manager | Data request log |
| +1 | Collect activity data and evidence | Data owners | `activity-data.csv`, evidence index |
| +2 | Calculate; QA/QC checks; uncertainty assessment | Inventory manager | Draft inventory |
| +2 | Internal review | Internal reviewer | Review record |
| +3 | Draft GHG report and GHG statement | Inventory manager | Draft report |
| +3–4 | Verification | Verification body | Findings, opinion |
| +4 | Fix findings; sign-off; publish | Inventory owner | Final report; git tag `FYxxxx-verified` |

## Information management procedures (clause 8.1)

- **Single source of truth.** This repository holds methods, registers and
  calculations. Source evidence lives in the controlled document store at
  _[location]_.
- **Change control.** Every change is made by pull request and reviewed by
  someone other than the author.
- **Access.** Write access is limited to the inventory team.
- **QA/QC checks** before sign-off. See [data quality](data-quality.md).

## Document retention (clause 8.2)

Keep the documents behind each verified inventory for at least _7_ years,
or longer if regulation or contracts require it.

## Improvement plan

| ID | Source | Issue | Action | Owner | Target year | Status |
|---|---|---|---|---|---|---|
| IMP-01 | | | | | | |
