# Emission factors

Keep every factor used in `inventory/<year>/emission-factor-register.csv`
(template: `templates/emission-factor-register.csv`). Each factor needs:

- a unique ID
- its value, unit and the gases it covers
- its source, publication year and table or row reference
- its geography and period of validity
- the GWP basis, if the factor is given in CO₂e

## Preferred sources

| Use | Source |
|---|---|
| UK fuels, electricity, travel, freight, waste | UK Government GHG Conversion Factors for Company Reporting (DESNZ), for the reporting year |
| Non-UK electricity (location-based) | National inventory or IEA data |
| Market-based electricity | Supplier fuel-mix disclosure; residual-mix factors (such as AIB for Europe) |
| Refrigerants | GWPs from the selected IPCC assessment report |
| Spend-based screening | A recognised EEIO dataset (such as UK SIC-based, US EEIO or EXIOBASE). State the price year. |

## Rules

- Use factors for the **reporting year**. If they are not yet published, use
  the latest available and disclose this.
- Never change a factor in place. Add a new row and retire the old one, so
  that past calculations can be reproduced.
