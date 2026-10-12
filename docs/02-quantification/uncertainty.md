# Uncertainty assessment

*ISO 14064-1:2018, clause 8.3*

The organisation must assess the uncertainty of its GHG inventory, covering
both activity data and emission factors.

## Approach

1. Give each source an uncertainty (±%) for its **activity data** and its
   **emission factor**. Base these on meter accuracy class, invoice versus
   estimate, or the uncertainty published with the factor.
2. Combine the two for each source (error propagation, assuming they are
   independent):
   `U_source = √(U_AD² + U_EF²)`
3. Combine across sources, weighted by emissions:
   `U_total = √Σ(E_i × U_i)² / ΣE_i`
4. For large or skewed uncertainties, use Monte Carlo simulation instead.

## Qualitative rating

Where a number cannot be estimated, rate each source:

| Rating | Typical case |
|---|---|
| Low (< ±5%) | Billed, metered data with an official factor |
| Medium (±5–20%) | Partial estimates; average factors |
| High (> ±20%) | Spend-based; modelled or proxy data |

## Use the results

Focus improvement work on sources that are **both** large and highly
uncertain. Record planned improvements in the
[inventory management plan](../03-data-management/inventory-management-plan.md#improvement-plan).
