# Pharmacy Prescription Check

Section **2800-23**. Supervisor: **Prasanna Lakshmi**.

The page takes a medical prescription and runs SQL against two SQLite databases: stock, trade names, side effects, and drug–drug interactions.

## Team

- Norah Saeed Alqahtani (445804256)
- Noura Hamad Hasan (445804642)
- Rawan Ali Almeshary (445804606)
- Wejdan Bandar (444820762)
- Zinah Ibrahem Saeed (445804594)

## How to open

Double-click `index.html` (Chrome or Safari). Keep `css`, `js`, `sql`, and `sources` next to it.

Inspect the databases with [DB Browser for SQLite](https://sqlitebrowser.org/): `sql/prescriptions.db` and `sql/pharmacy.db`.

Rebuild from the attached CSVs:

```
python3 sql/build_from_sources.py
```

## Sources (attached)

See `sources/SOURCES.md`.

| File | Origin |
| --- | --- |
| `sources/medical_prescription_dataset.csv` | [Medical Prescription Dataset](https://www.kaggle.com/datasets/mmumairkhattak/medical-prescription-dataset) |
| `sources/drug_drug_interactions.csv` | [Drug-Drug Interactions](https://www.kaggle.com/datasets/mghobashy/drug-drug-interactions) |
| `sources/pharmacy_catalog.csv` | Pharmacy stock (scientific name + trade name) |
| `sources/drug_side_effects.csv` | Side effects for catalog drugs |

## SQL databases

- `sql/prescriptions.db` — PATIENT, PRESCRIPTION_ITEM
- `sql/pharmacy.db` — DRUG, TRADE_NAME, SIDE_EFFECT, INTERACTION

Flowchart images (for the report, not website pages): `images/system-flowchart.png`, `images/database-flowchart.png`.
