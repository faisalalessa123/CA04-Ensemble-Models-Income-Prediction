# CA04 – Ensemble Models Income Prediction

## Overview
This project applies multiple ensemble learning techniques to the Census Income dataset in order to predict whether an individual's income exceeds $50K per year. The models evaluated include:

- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost

Each model is trained using varying numbers of estimators, and performance is evaluated using Accuracy and AUC metrics.

---

## Dataset

- Source: U.S. Census Bureau
- Total Instances: 48,842
- Target Classes:
  - 1 → Income > 50K
  - 0 → Income ≤ 50K
- Features: 7 demographic attributes
- Data split provided via dataset flag (Training/Test)

Dataset used:
https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true

---

## Methodology

1. Data preprocessing and encoding (same transformations as CA03)
2. Train/Test split using provided flag column
3. One-hot encoding for categorical variables
4. Model training with varying `n_estimators` values:
   [50, 100, 150, 200, 250, 300, 350, 400, 450, 500]
5. Performance evaluation using:
   - Accuracy
   - ROC AUC
6. Visualization of:
   - Accuracy vs. n_estimators
   - AUC vs. n_estimators
7. Final comparison of best-performing configurations across models

---

## Results Summary

For each ensemble model:
- Performance trends were analyzed with respect to the number of estimators.
- The optimal estimator value within the tested range was identified.
- A comparison table summarizes the best Accuracy and AUC achieved by each model.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost

---

## Files Included

- `CA4.ipynb` – Fully executed notebook
- `README.md` – Project documentation

---

## Authors

Faisal Alessa  
Jake Bonavia  

MSBA – Loyola Marymount University
