# Drug ML Tutorial (Mini-Course)

This repo contains three Google Colab–ready notebooks that take you from zero to
training simple models and (optionally) playing with real NCI‑60 drug‑response data.

## Notebooks
- `notebooks/01_intro_sklearn_breast_cancer.ipynb` — Binary classification demo with scikit‑learn.
- `notebooks/02_qsar_fish_toxicity.ipynb` — QSAR regression (LC50) using UCI data.
- `notebooks/03_nci60_toy_demo.ipynb` — Optional NCI‑60 toy regression (drug z‑scores from RNA‑seq).

## How to run in Colab
1. Open the notebook in Colab (File → Open Notebook → Upload).
2. Run the first cell to install dependencies in the Colab runtime.
3. Execute the cells top to bottom.

## Save to GitHub from Colab (GUI)
File → Save a copy in GitHub… (choose repo/branch, add commit message).

## Save to GitHub from Colab (CLI)
Create a Personal Access Token (classic, repo scope) on GitHub, then in a Colab cell:
```
!git config --global user.email "you@example.com"
!git config --global user.name "Your Name"
!git clone https://github.com/<user>/<repo>.git
# Move your .ipynb into the repo folder as needed
%cd /content/<repo>
!git add -A
!git commit -m "Add first ML notebooks"
!git push https://<TOKEN>@github.com/<user>/<repo>.git HEAD:main
```

## Reproducibility
Inside a running Colab kernel you can capture the environment with:
```
!pip freeze | tee environment.txt
```
and commit it to GitHub.