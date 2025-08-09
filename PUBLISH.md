# Update an Existing GitHub Repo

If your code is already on GitHub, do this locally to add these new files (README, .gitignore, LICENSE, requirements, etc.) and push:

```bash
# from your project root
# 1) Copy the following files/folders into your repo:
#    - README.md
#    - .gitignore
#    - .gitattributes
#    - LICENSE
#    - requirements.txt
#    - CONTRIBUTING.md
#    - notebooks/walmart-sales-forecasting-w.r.t-time-series-analysis.ipynb  (if not already present)
#    - data/ (empty folder, stays ignored)
#    - reports/figures/ (empty folder, stays ignored)

# 2) Optional: enable clean notebook diffs
pip install nbstripout
nbstripout --install

# 3) Commit & push
git add -A
git commit -m "Repo polish: README, license, gitignore, requirements, structure"
git push origin main
```
