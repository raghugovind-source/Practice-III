# Module 17: Comparing Classifiers

Practical application comparing **K-Nearest Neighbors**, **Logistic Regression**, **Decision Trees**, and **Support Vector Machines** on a bank marketing dataset.

## Overview

The goal is to predict whether a client will subscribe to a **term deposit** (binary classification) using bank client features. The notebook walks through data understanding, feature engineering, baseline and model comparison, hyperparameter tuning, and visualizations for each model.

## Dataset

- **Source:** [UCI Bank Marketing](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- **Content:** Results of 17 marketing campaigns from a Portuguese banking institution (May 2008 – November 2010).
- **Location:** `data/bank-additional/bank-additional-full.csv` (semicolon-separated)

## Requirements

- Python 3.x
- pandas
- scikit-learn
- matplotlib

Install with:

```bash
pip install pandas scikit-learn matplotlib
```

## Usage

1. Open `prompt_III.ipynb` in Jupyter Notebook or JupyterLab (or run in VS Code / Cursor).
2. Ensure the dataset is at `data/bank-additional/bank-additional-full.csv` relative to the notebook.
3. Run all cells in order.
4. Outputs (tables and plots) are written to the `results/` folder.

## Outputs

After running the notebook, the `results/` directory contains:

| File | Description |
|------|-------------|
| `model_comparison.csv` | Train time, train accuracy, test accuracy for LR, KNN, Decision Tree, SVM |
| `tuned_models.csv` | Test accuracy and Test F1 for tuned KNN, Decision Tree, SVM |
| `model_comparison_plots.png` | Train vs test accuracy, training time, and confusion matrices per model |
| `model_roc_curves.png` | ROC curves and AUC for each model |
| `cross_validation_scores.csv` | 5-fold CV mean and std accuracy per model |
| `cross_validation_plots.png` | Box plot of CV fold scores and bar chart of mean CV accuracy ± std |
| `tuned_models_plots.png` | Test accuracy and F1 bar charts for tuned models |

## Notebook Structure

| Section | Description |
|--------|-------------|
| Problems 1–4 | Data understanding, feature check, business objective |
| Problem 5 | Feature engineering (bank client features, one-hot encoding) |
| Problem 6 | Train/test split |
| Problem 7 | Baseline (majority class) |
| Problems 8–9 | Logistic Regression model and scoring |
| Problem 10 | Compare LR, KNN, Decision Tree, SVM; save table; **plots**: accuracy, train time, confusion matrices, ROC curves; **cross-validation**: 5-fold CV with box plot and mean±std bar chart |
| Problem 11 | Hyperparameter tuning (GridSearchCV), F1 comparison; save table; **plots**: tuned model accuracy and F1 |

## Citation

Moro et al., 2014. A Data-Driven Approach to Predict the Success of Bank Telemarketing. *Decision Support Systems*. [DOI](http://dx.doi.org/10.1016/j.dss.2014.03.001)
