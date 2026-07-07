# From Black Box to Trusted ML: Explainable AutoML in Banking

This repository contains the code for the master thesis **"From Black Box to Trusted ML: Explainable AutoML in Banking"**.

The thesis investigates how explainability can be integrated into AutoML workflows in two banking-related use cases: **probability of default prediction** and **bank marketing**. H2O AutoML and AutoGluon are compared with a Logistic Regression benchmark. The evaluation considers both predictive performance and a human-centered assessment of interpretability, trust, acceptance, and regulatory plausibility. :contentReference[oaicite:0]{index=0}

## Use Cases

The repository contains notebooks for two use cases:

1. **PD prediction**  
   A simplified 12-month probability of default use case based on a loan default dataset.  
   The workflow includes WoE-based preprocessing, Logistic Regression, AutoML models, calibration, scorecard-oriented outputs, and governance-related artefacts.

2. **Bank marketing prediction**  
   A marketing campaign use case based on the Bank Marketing dataset.  
   The objective is to rank customers according to their predicted likelihood of subscribing to a term deposit and to support campaign planning through gains, lift, and budget-oriented evaluation.

## Models and Frameworks

The implementation includes:

- Logistic Regression baseline models (from sklearn.linear_model import LogisticRegression)
- H2O AutoML models (!pip install -U h2o)
- AutoGluon Tabular models (!pip install autogluon.tabular[all] and from autogluon.tabular import TabularPredictor)
- SHAP and LIME explanations (!pip install shap lime -q)
- additional scorecard-like, calibration, stability, and governance-oriented outputs (see notebooks)

## Explainability Levels

The notebooks follow the explainability structure used in the thesis:

| Level | Content |
|---|---|
| Level 0 | Logistic Regression baseline |
| Level 1 | AutoML with built-in explainability |
| Level 2 | Level 1 plus SHAP and LIME |
| Level 3 | Level 2 plus scorecard-like and governance-oriented outputs |
| Level 4 | Level 3 plus restricted AutoML search space and model-specific visualisations |

## Datasets

Dataset for the PD-Use Case: https://www.kaggle.com/datasets/nikhil1e9/loan-default
Dataset for the Marketing-Use Case: https://archive.ics.uci.edu/dataset/222/bank+marketing
