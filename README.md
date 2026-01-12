# Multivariate pIC50 modeling for Carbonic Anhydrase II (ChEMBL205) — OLS + diagnostics

**Goal:** Build a reproducible data science workflow to model **pIC50** for **Carbonic Anhydrase II (ChEMBL205)** using a **multiple linear regression (OLS)** with two molecular descriptors: **AlogP** (lipophilicity) and **Molecular Weight (MW)**.

📄 Full report (Spanish): `reports/reporte_P2.pdf`

---

## Why this matters
- Shows progression from a weak baseline (Project 1) to a **multivariate model** with improved explanatory power.
- Includes **diagnostics** (collinearity, heteroscedasticity, influence) and proposes concrete next steps.
- Reproducibility: **Python-first workflow** + optional **R cross-check**.

---

## Executive summary
- Model: **pIC50 ~ AlogP + MW** (OLS)
- Outputs include: coefficients, R²/adjusted R², F-test, residual diagnostics, VIF, Cook’s distance, and Breusch–Pagan test.

---

## Key figures (EDA + diagnostics)

![Correlation heatmap](figures/Figure_04.png)

![Residuals vs fitted](figures/residuals_vs_fitted.png)

![Cook's distance](figures/cooks_distance.png)

---

## Notebooks
1. `notebooks/01_multivariate_eda.ipynb`
2. `notebooks/02_multivariate_ols.ipynb`
3. `notebooks/03_diagnostics_influence.ipynb`

---

## Author
M. Osvaldo Hernández Montoya
