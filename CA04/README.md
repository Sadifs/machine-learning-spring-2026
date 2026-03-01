# CA04 – Ensemble Models

## Project Overview

This project implements and evaluates four Ensemble Machine Learning classifiers to predict whether an individual's income exceeds $50K per year using the Census Income dataset.

The primary objective is to analyze how model performance changes with respect to the hyperparameter n_estimators, and to determine the optimal number of estimators for each model.

The following models were implemented:
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost

Each model was evaluated using:
- Accuracy
- AUC (Area Under the ROC Curve)

---

## Dataset Information

The dataset is obtained from the U.S. Census Bureau and contains demographic information used to predict income classification.

### Dataset Characteristics

- Total instances: 48,842
- Number of attributes: 7
- Target Classes:
- 1 → Income > 50K
- 0 → Income ≤ 50K

### Data Source

https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true

The dataset includes a column that indicates whether a record belongs to the Training or Testing set. Training and testing datasets were created programmatically based on this column.

Data cleaning and transformations were performed in the same manner as CA03.

---

## Environment & Libraries Used

- Python 3.x
- Jupyter Notebook

### Required Libraries

- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost

To install dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost
