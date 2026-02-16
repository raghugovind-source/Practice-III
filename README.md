# Module 17: Comparing Classifiers

Practical application comparing **K-Nearest Neighbors**, **Logistic Regression**, **Decision Trees**, and **Support Vector Machines** on a bank marketing dataset.

## Overview

The goal is to predict whether a client will subscribe to a **term deposit** (binary classification) using bank client features. The notebook walks through data understanding, feature engineering, baseline and model comparison, and hyperparameter tuning.

## Dataset

- **Source:** [UCI Bank Marketing](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- **Content:** Results of 17 marketing campaigns from a Portuguese banking institution (May 2008 – November 2010).
- **Location:** `data/bank-additional/bank-additional-full.csv` (semicolon-separated)

## Requirements

- Python 3.x
- pandas
- scikit-learn

Install with:

```bash
pip install pandas scikit-learn
```

## Usage

1. Open `prompt_III.ipynb` in Jupyter Notebook or JupyterLab (or run in VS Code / Cursor).
2. Ensure the dataset is at `data/bank-additional/bank-additional-full.csv` relative to the notebook.
3. Run all cells in order.

## Notebook Structure

| Section | Description |
|--------|-------------|
| Problems 1–4 | Data understanding, feature check, business objective |
| Problem 5 | Feature engineering (bank client features, one-hot encoding) |
| Problem 6 | Train/test split |
| Problem 7 | Baseline (majority class) |
| Problems 8–9 | Logistic Regression model and scoring |
| Problem 10 | Compare LR, KNN, Decision Tree, SVM (train time & accuracy) |
| Problem 11 | Hyperparameter tuning (GridSearchCV) and F1 comparison |

## Citation

Moro et al., 2014. A Data-Driven Approach to Predict the Success of Bank Telemarketing. *Decision Support Systems*. [DOI](http://dx.doi.org/10.1016/j.dss.2014.03.001)
