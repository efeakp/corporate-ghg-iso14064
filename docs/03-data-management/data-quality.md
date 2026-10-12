# Data quality and QA/QC

## QA/QC checklist

Complete this for every reporting year, in `inventory/<year>/qaqc-checklist.md`.

- [ ] Every entity in the boundary register has data, or a documented reason why not
- [ ] Every significant source has activity data for all 12 months
- [ ] Units are consistent; conversions have been checked
- [ ] Emission factors match the register and are for the right year and geography
- [ ] Estimates are flagged and their method is documented
- [ ] Year-on-year change is over ±_10_% for a source → explained
- [ ] Totals reconcile: source → category → inventory
- [ ] Double counting checked (for example, fleet fuel cards against expense claims)
- [ ] Category 2 reported location-based **and** market-based
- [ ] Biogenic CO₂ reported separately
- [ ] Sampled calculations recalculated by hand (at least _10_%)
- [ ] Internal reviewer sign-off recorded

## Evidence index

Every activity-data row must point to evidence (`evidence_id`). The index
(`inventory/<year>/evidence-index.csv`) records:

- evidence ID
- description, such as "British Gas invoice Jan 2025, Site A"
- where it is stored (path or link in the document store)
- who provided it, and when

Verifiers sample from this index. A broken link is a finding.
