# From Black Box to Trusted ML: Explainable AutoML in Finance

This repository contains the code developed for the master thesis **"From Black Box to Trusted ML: Explainable AutoML in Banking"**.  
The project investigates how explainability can be integrated into Automated Machine Learning (AutoML) workflows in financial use cases.

## Project Overview

The thesis compares classical and AutoML-based modelling approaches in two banking-related use cases:

1. **PD prediction**  
   Prediction of a 12-month probability of default for loan customers.

2. **Bank marketing prediction**  
   Prediction of whether a customer subscribes to a term deposit after a marketing campaign.

The main focus is not only predictive performance, but also the extent to which different models and explainability levels support interpretability, trust, regulatory plausibility, and user acceptance.

## Frameworks and Models

The repository includes implementations for:

- Logistic Regression baseline models
- H2O AutoML models
- AutoGluon Tabular models

Each use case is implemented across several explainability levels.

## Explainability Levels

The modelling workflow follows a stepwise explainability framework:

| Level | Description |
|---|---|
| Level 0 | Logistic Regression baseline |
| Level 1 | AutoML with built-in explainability |
| Level 2 | Level 1 plus post-hoc explanations such as SHAP and LIME |
| Level 3 | Level 2 plus governance-oriented and scorecard-like outputs |
| Level 4 | Level 3 plus restricted model search space and model-specific visualisations |

## Repository Structure

The repository contains the following material:

### Exploratory Data Analysis

- PD-12m EDA
- Marketing EDA

### PD-12m Use Case

- Level 0: Weight of Evidence (WoE) transformation and Logistic Regression
- AutoGluon Levels 1–4
- H2O AutoML Levels 1–4

### Marketing Use Case

- Level 0: Data preprocessing and Logistic Regression
- AutoGluon Levels 1–4
- H2O AutoML Levels 1–4

### Questionnaire Evaluation

The repository further contains the scripts used for the statistical evaluation of the questionnaire, the generation of figures and tables presented in the thesis.

### Questionnaire Material

- Questionnaire (PDF)
- Questionnaire responses (Excel)

