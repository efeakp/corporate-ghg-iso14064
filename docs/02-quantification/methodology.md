# Quantification methodology

*ISO 14064-1:2018, clause 6*

## General approach

For most sources:

```
Emissions (tCO₂e) = Activity data × Emission factor × GWP
```

Where the factor is already in CO₂e, no separate GWP step is needed.

## Hierarchy of methods

Use the most accurate method that is practical. Record the method used for
each source in `activity-data.csv` (`method_tier` column).

| Tier | Method | Example |
|---|---|---|
| A | Direct measurement | Continuous emissions monitoring |
| B | Supplier-specific or primary activity data × specific factor | Fuel invoices × fuel-specific factor; supplier-specific electricity factor |
| C | Primary activity data × published average factor | kWh from meters × national grid factor |
| D | Estimated or modelled activity data × average factor | Floor-area estimate of energy use |
| E | Spend-based (EEIO) | £ spend × kgCO₂e/£ |

## Global warming potentials

**Selected GWP set:** IPCC AR_ (100-year). Use **one** set throughout, and
record it in the GHG report. If the set changes, recalculate the base year.

## Calculation rules

- Hold all calculations in version-controlled files. Never hard-code numbers
  in a report.
- Use the same units throughout. Convert at the activity-data stage.
- Every row of activity data must reference an evidence ID (see
  [data quality](../03-data-management/data-quality.md#evidence-index)).
- Estimates and extrapolations, such as a missing month of meter data, must
  be flagged (`is_estimate = TRUE`) with the method described.
