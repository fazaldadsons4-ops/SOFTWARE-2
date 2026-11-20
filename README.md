# 16 Cities PDF Software

A separate local Python/Flask application for processing city-wise PDF reports, cleaning minus signs and calculating values, and consolidating up to 16 city Excel sheets.

## Features
- PDF table extraction with selectable source columns (medicine, net rate, net sale).
- Excel minus-sign cleanup and rate × net-sale calculation.
- City-wise consolidation into one A–Z workbook with one column per city.
- Conservative product-name normalization and fuzzy-match suggestions; uncertain matches should be reviewed rather than silently merged.

## Run locally (Windows)
```bat
py -m venv .venv
.venv\Scripts\activate
python -m pip install -r requirements.txt
py app.py
```
Open `http://127.0.0.1:5002/`.

Uploaded files and generated outputs are stored locally in `uploads/` and `outputs/`; do not commit confidential business data to GitHub.
