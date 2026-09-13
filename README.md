# Waze: User Churn Prediction

## Project Overview

This project builds and evaluates machine learning models that predict whether a Waze user is likely to churn. The results are intended to help teams understand retention risk and focus user-engagement efforts more effectively.

The analysis follows the PACE framework: Plan, Analyze, Construct, and Execute. It includes data preparation, feature engineering, model training, evaluation, and recommendations for responsible application.

## Objectives

- Inspect and prepare Waze user activity data.
- Engineer behavioral features related to driving and app usage.
- Train Random Forest and XGBoost classification models.
- Compare model performance using recall, precision, F1 score, accuracy, and confusion matrices.
- Identify important predictors and communicate practical next steps.

## Contents

| File | Description |
| --- | --- |
| `Activity_Course 6 Waze project lab.ipynb` | Complete analysis, feature engineering, modeling, and evaluation notebook. |
| `waze_dataset.csv` | Waze user activity data used for churn modeling. |
| `Pace.png`, `Plan.png`, `Analyze.png`, `Construct.png`, `Execute.png` | Visual markers used in the notebook's PACE sections. |

## Workflow

The notebook copies and prepares the source data, creates behavioral features such as driving-day and usage measures, encodes categorical variables, and separates predictors from the churn target. Random Forest and XGBoost models are tuned and evaluated on held-out data.

Model performance is assessed with:

- Recall
- Precision
- F1 score
- Accuracy
- Confusion matrix
- Feature importance

Recall is especially important when missing a user who will churn is more costly than contacting a user who remains active.

## Getting Started

1. Clone or download this repository.
2. Open the notebook in Jupyter Notebook, JupyterLab, or VS Code.
3. Select a Python 3 kernel with the required packages installed.
4. Run the notebook cells in order.

Typical dependencies include `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `xgboost`.

The data loader supports running from either the project folder or the repository root.

## Responsible Use

Churn predictions should guide supportive retention analysis, not trigger automatic penalties or unwanted targeting. Any intervention should respect user privacy, be evaluated for effectiveness, and be monitored for unequal impact. Model predictions should remain one input among several, with human review and clear safeguards.

## Learning Context

This project was completed as part of the Google Advanced Data Analytics coursework and demonstrates an end-to-end binary classification workflow.
