# Contributing & Local Workflow

## Local environment
1. Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\Activate.ps1
   pip install -r requirements.txt
   ```
2. Keep large data out of Git. Put it in `data/` (already gitignored).

## Notebooks best practices
- Install `nbstripout` to keep diffs clean:
  ```bash
  pip install nbstripout
  nbstripout --install
  ```
- Prefer saving heavy images to `reports/figures/` and embed relative paths in the notebook/README.

## Commit & push
```bash
git add -A
git commit -m "Describe your change briefly (EDA, model tuning, charts, etc.)"
git push origin main
```

## Releasing results
- Add a short section in README with metrics and a representative forecast chart.
- (Optional) Create a GitHub Release attaching a PNG of key results.
