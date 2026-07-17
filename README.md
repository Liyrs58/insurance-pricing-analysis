# Medical Insurance Cost Analysis

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-success)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

Actuarial-style pricing analysis using the public Medical Cost dataset. The project explores key premium drivers such as age, BMI, smoking status, and region, then compares interpretable statistical models with machine-learning regressors.

**Live notebook:** https://liyrs58.github.io/insurance-pricing-analysis/notebook.html

## What This Project Shows

This is a compact applied analytics project: it starts with a business pricing question, performs exploratory analysis, builds multiple predictive models, and explains the trade-off between accuracy and interpretability.

## Key Findings

- **Smoking is the dominant pricing factor** - smokers incur premiums 3-4x higher than non-smokers across all models
- **Age has a strong positive relationship** with charges, adding approximately $250-$300 per year of age
- **BMI shows a non-linear effect** - the impact accelerates at higher BMI values, particularly for smokers
- **Region effects are relatively small**, with the Southeast showing marginally higher average charges
- **XGBoost and Random Forest achieve the best predictive performance** (lowest RMSE and highest R-squared), while GLM Gamma provides the most interpretable actuarial model

## Models Compared

| Model | Type | Purpose |
|-------|------|---------|
| OLS Linear Regression | Statistical | Baseline interpretable model |
| GLM Gamma | Actuarial | Industry-standard for claim cost modelling |
| Ridge Regression | Regularised | Handle multicollinearity |
| Random Forest | Ensemble | Non-linear relationships |
| XGBoost | Gradient Boosting | Highest predictive accuracy |

## Skills Demonstrated

| Area | Evidence |
|------|----------|
| Pricing analytics | Identifies measurable cost drivers and compares model behaviour |
| Statistical modelling | Uses OLS, GLM Gamma, regularised regression, and tree-based methods |
| Model interpretation | Explains why the most accurate model is not always the most useful business model |
| Data communication | Presents findings in a hosted notebook with charts and written commentary |

## Tech Stack

- **Python** - pandas, numpy, scikit-learn, statsmodels, xgboost
- **Jupyter Notebook** - interactive analysis
- **Matplotlib / Seaborn** - visualisation
- **GitHub Pages** - public hosting

## View Locally

```bash
python3 -m http.server 8000
# Open http://localhost:8000/docs/notebook.html or the hosted notebook link above
```

## Limitations

The dataset is a public teaching dataset and should not be treated as a production actuarial pricing base. The analysis is useful for demonstrating modelling workflow, feature interpretation, and pricing reasoning.
