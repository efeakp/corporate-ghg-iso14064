# Organisational boundary

*ISO 14064-1:2018, clause 5.1*

## Consolidation approach

Choose **one** approach and apply it to every entity:

| Approach | Rule | Choose when |
|---|---|---|
| **Operational control** | 100% of emissions from operations we control operationally | Most common. Aligns with where we can act. |
| Financial control | 100% of emissions from operations we control financially | Aligns with financial reporting. |
| Equity share | Emissions in proportion to our ownership share | Required by some joint-venture arrangements. |

**Selected approach:** _TBC_
**Rationale:** _TBC_ (log it in the [decision log](../03-data-management/decision-log.md))

## Entity and facility register

Maintain the register in `inventory/<year>/boundary-register.csv`
(template: `templates/boundary-register.csv`). For each entity record:

- legal name, country and ownership %
- whether we hold operational and financial control
- whether it is included, and the inclusion %
- the reason for any exclusion

## Changes during the year

Record acquisitions, disposals, mergers and outsourcing with their effective
date. Check each against the
[base-year recalculation policy](base-year.md#recalculation-policy).
