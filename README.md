# Walmart Sales Forecasting — Time Series Analysis

Forecasting Walmart store-item sales using classical and modern time-series methods. This repo contains a reproducible Jupyter notebook and a lightweight project structure so you (or recruiters) can run it quickly.

## Highlights
- End‑to‑end: EDA → feature engineering → model training → evaluation → visualization
- Methods: ARIMA/SARIMA (statsmodels), Prophet, and ML baselines (scikit‑learn), depending on availability
- Clean repo structure with data + figures ignored by Git
- Auto‑generated `requirements.txt` from the notebook imports

## Dataset
This notebook was built for Walmart-style daily/weekly sales time series (e.g., M5/Walmart).  
> **Note:** Raw datasets are **not** committed. Place your CSVs under `data/` and adjust paths in the notebook if necessary.

- Example sources you can use:
  - Kaggle (Walmart/M5 datasets) — download locally and keep under `data/` (ignored by Git).

## Quickstart
```bash
# 1) Clone
git clone https://github.com/<your-username>/walmart-sales-forecasting-timeseries.git
cd walmart-sales-forecasting-timeseries

# 2) Python env
python -m venv .venv
# macOS/Linux:
source .venv/bin/activate
# Windows (PowerShell):
# .venv\Scripts\Activate.ps1

# 3) Install deps
pip install -r requirements.txt

```

Open: `notebooks/walmart-sales-forecasting-w.r.t-time-series-analysis.ipynb`

## Project Structure
```
walmart-sales-forecasting-timeseries/
├─ notebooks/
│  └─ walmart-sales-forecasting-w.r.t-time-series-analysis.ipynb
├─ data/                  # put raw/processed data here (ignored)
├─ reports/
│  └─ figures/            # charts exported here (ignored)
├─ requirements.txt
├─ .gitignore
├─ .gitattributes         # nicer diffs for notebooks
├─ LICENSE                # MIT
├─ README.md
└─ CONTRIBUTING.md
```

## Results (fill in with your run)
- Metrics: RMSE / MAE / MAPE
- Best model:
- Notes: holidays/seasonality handled?, cross‑validation window?, exogenous features?

## Repro Tips
- Export plots to `reports/figures/` (already gitignored) for easy embedding in README.
- If you change library versions, update `requirements.txt`:
  ```bash
  pip freeze > requirements.txt
  ```

## License
MIT — see `LICENSE`.
