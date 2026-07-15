# Medical Insurance Cost Analysis — An Actuarial Pricing Study

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-success)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

An in-depth actuarial analysis of medical insurance costs using the classic Kaggle Medical Cost dataset. This project explores key pricing drivers — age, BMI, smoking status, and region — and builds a suite of regression models to predict individual healthcare premiums. The analysis demonstrates how statistical and machine learning approaches can be applied to insurance pricing and risk modelling.

## Key Findings

- **Smoking is the dominant pricing factor** — smokers incur premiums 3–4× higher than non-smokers across all models
- **Age has a strong positive relationship** with charges, adding approximately $250–$300 per year of age
- **BMI shows a non-linear effect** — the impact accelerates at higher BMI values, particularly for smokers
- **Region effects are relatively small**, with the Southeast showing marginally higher average charges
- **XGBoost and Random Forest achieve the best predictive performance** (lowest RMSE and highest R²), while GLM Gamma provides the most interpretable actuarial model

## Models Used

| Model | Type | Purpose |
|-------|------|---------|
| OLS Linear Regression | Statistical | Baseline interpretable model |
| GLM Gamma | Actuarial | Industry-standard for claim cost modelling |
| Ridge Regression | Regularised | Handle multicollinearity |
| Random Forest | Ensemble | Non-linear relationships |
| XGBoost | Gradient Boosting | Highest predictive accuracy |

## Tech Stack

- **Python** — pandas, numpy, scikit-learn, statsmodels, xgboost
- **Jupyter Notebook** — interactive analysis
- **Matplotlib / Seaborn** — visualisation
- **GitHub Pages** — public hosting

## How to View the Analysis

The full interactive notebook is hosted via GitHub Pages:

👉 [**View the Analysis**](https://liyrs58.github.io/insurance-pricing-analysis/notebook.html)

---

*Built as part of application for Howden Graduate Analyst — Employee Benefits Analytics and Risk Modelling role.*
