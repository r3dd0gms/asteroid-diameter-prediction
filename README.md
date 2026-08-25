# Predicting Asteroid Diameter

A regression project predicting the diameter of asteroids using a Decision Tree Regressor, based on physical and orbital features from NASA's asteroid dataset.

## Overview

The dataset is cleaned (duplicates and missing-target rows dropped, high-missingness columns removed, remaining gaps filled with median/mode), categorical fields are label-encoded, and the top 10 predictive features are selected via F-regression scoring. Features are standardised before an 80/20 train-test split and Decision Tree Regressor fit.

## Dataset

`asteroid.csv` — NASA asteroid physical and orbital parameters, with `diameter` as the prediction target.

## Key Findings

- The top 10 features by F-regression score were used for modelling(see feature importance plot for the ranked list).
- Model performance evaluated via MAE, MSE, RMSE, and R**2.
- A pruned decision tree (top 3 levels) is visualised to show the model's primary splitting logic.

## Tech Stack

pandas, numpy, matplotlib, seaborn, scikit-learn

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook Predicting_Asteriod_Diameter.ipynb
```
