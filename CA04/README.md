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
```

---

## Model Implementation

For each model, n_estimators was tested using the following values:

```
[50, 100, 150, 200, 250, 300, 350, 400, 450, 500]
```

All other hyperparameters were kept at their default values.

For every model, the following plots were generated:

- Accuracy vs. n_estimators
- AUC vs. n_estimators

---

## Results & Observations

### 1. Random Forest

Best Accuracy: 0.839076 (n_estimators = 500)  
Best AUC: 0.881726 (n_estimators = 500)

Observation:

Accuracy and AUC steadily improved as the number of estimators increased. The model achieved its best performance at 500 estimators. Performance gains diminished at higher values, indicating stabilization.

Optimal Estimator in Range: 500

---

### 2. AdaBoost

Best Accuracy: 0.845833 (n_estimators = 100)  
Best AUC: 0.897429 (n_estimators = 100)

Observation:

Performance peaked early at 100 estimators. Increasing beyond 100 provided minimal improvement and showed plateau behavior.

Optimal Estimator in Range: 100

---

### 3. Gradient Boosting

Best Accuracy: 0.847245 (n_estimators = 50)  
Best AUC: 0.899046 (n_estimators = 200)

Observation:

Gradient Boosting achieved the highest overall performance among all models. Accuracy peaked at 50 estimators, while AUC continued to improve until 200 estimators before stabilizing.

Optimal Estimator in Range:

- Accuracy → 50
- AUC → 200

---

### 4. XGBoost

Best Accuracy: 0.844236 (n_estimators = 50)  
Best AUC: 0.896334 (n_estimators = 50)

Observation:

XGBoost achieved strong performance at lower estimator values. Increasing the number of estimators beyond 50 did not significantly improve results, demonstrating efficient learning.

Optimal Estimator in Range: 50

---

## Performance Comparison

| Model              | Best Accuracy | Best AUC |
|--------------------|--------------|----------|
| Random Forest      | 0.839076     | 0.881726 |
| AdaBoost           | 0.845833     | 0.897429 |
| Gradient Boosting  | 0.847245     | 0.899046 |
| XGBoost            | 0.844236     | 0.896334 |

---

## Overall Best Model

Highest Accuracy: Gradient Boosting (0.847245)  
Highest AUC: Gradient Boosting (0.899046)

Gradient Boosting demonstrated the strongest overall performance in this analysis.

---

## Author

Sadaf, Sude  
MSBA Program  
Course: Machine Learning
