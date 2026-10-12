# Corporate GHG Accounting, Verification & Validation (ISO 14064)

Documentation, procedures and templates for preparing an organisation-level
greenhouse gas (GHG) inventory in line with **ISO 14064-1:2018**, and for
having that inventory verified (and forward-looking claims validated) in line
with **ISO 14064-3:2019**.

> **Copyright note.** ISO standards are copyrighted. This repository refers to
> clause numbers and paraphrases requirements; it does not reproduce the
> standards' text. Keep a licensed copy to hand and check every clause
> reference against it.

## What this repository covers

| Stage | ISO reference | Where |
|---|---|---|
| Principles, terms, the ISO 14064 family | 14064-1 cl. 4; 14064-3 cl. 4 | [`docs/00-overview`](docs/00-overview) |
| Inventory design: boundaries, significance, base year | 14064-1 cl. 5, 6.4 | [`docs/01-inventory-design`](docs/01-inventory-design) |
| Quantification: categories 1–6, emission factors, uncertainty | 14064-1 cl. 6, 8.3 | [`docs/02-quantification`](docs/02-quantification) |
| Data and quality management | 14064-1 cl. 8 | [`docs/03-data-management`](docs/03-data-management) |
| Reporting | 14064-1 cl. 9 | [`docs/04-reporting`](docs/04-reporting) |
| Verification of the GHG statement | 14064-3; 14064-1 cl. 10 | [`docs/05-verification`](docs/05-verification) |
| Validation of targets and reduction plans | 14064-3 | [`docs/06-validation`](docs/06-validation) |
| Data templates (CSV) | — | [`templates/`](templates) |

## Repository layout

```
.
├── docs/                    # Documentation site source (MkDocs)
│   ├── 00-overview/
│   ├── 01-inventory-design/
│   ├── 02-quantification/
│   ├── 03-data-management/
│   ├── 04-reporting/
│   ├── 05-verification/
│   └── 06-validation/
├── templates/               # CSV registers: activity data, factors, findings…
├── inventory/               # Anonymised examples only; real data is in a private repo
├── .github/                 # Issue templates, PR template, docs workflow
└── mkdocs.yml
```

## Working in this repository

- **Keep real data private.** This repository holds the methods and
  templates. Each year's inventory data lives in a separate **private**
  repository, one folder per reporting year (e.g. `inventory/FY2025/`),
  started from the CSVs in `templates/`. The data repository records which
  commit or tag of these methods it applied.
- **Every change goes through a pull request.** The PR history is the audit
  trail a verifier will ask for (who changed what, when, and why).
- **Tag the version that was verified** (e.g. `FY2025-verified`), so the
  verified GHG statement can always be traced back to its exact data.
- **Raise verification findings as issues** using the *Verification finding*
  template, and close them with the PR that resolves them.
- Do not commit confidential source evidence (invoices, meter photos) here.
  Keep it in the controlled document store and reference it from
  `evidence-index.csv`.

## Viewing the documentation site

```bash
pip install mkdocs-material
mkdocs serve        # http://127.0.0.1:8000
```

The GitHub Actions workflow in `.github/workflows/docs.yml` publishes the
site to GitHub Pages on every push to `main`.

## Status

Living document. See [`CHANGELOG.md`](CHANGELOG.md).

## Licence

© 2026 Efe Akpovwovwo. This work is licensed under the
[Creative Commons Attribution 4.0 International licence (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You may share and adapt it for any purpose, provided you give appropriate
credit, link to the licence and indicate if changes were made. See
[`LICENSE`](LICENSE).

The licence covers this repository's own content only. It does not cover the
ISO standards, which remain © ISO, or any third-party emission-factor
datasets referenced here, which remain subject to their own terms.
