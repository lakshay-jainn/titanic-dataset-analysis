# Titanic - Machine Learning from Disaster

This repository contains an end-to-end machine learning project on the Kaggle Titanic dataset.
The objective is to predict whether a passenger survived the Titanic disaster using classification models.

---

## Project Overview

* Data exploration and cleaning
* Handling missing values, duplicates, and outliers
* Exploratory Data Analysis (univariate and bivariate analysis)
* Feature engineering (age binning, categorical encoding, log transformations)
* Training multiple classification models
* Hyperparameter tuning with GridSearchCV
* Submitting predictions to Kaggle competition

---

## Dataset Information

The dataset includes the following features:

| Feature  | Description                                                          |
| -------- | -------------------------------------------------------------------- |
| Survival | 0 = No, 1 = Yes                                                      |
| Pclass   | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)                             |
| Sex      | Gender                                                               |
| Age      | Age in years                                                         |
| SibSp    | Number of siblings/spouses aboard                                    |
| Parch    | Number of parents/children aboard                                    |
| Ticket   | Ticket number                                                        |
| Fare     | Passenger fare                                                       |
| Cabin    | Cabin number                                                         |
| Embarked | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## Workflow

1. **Data Loading and Inspection**

   * Loaded the dataset and checked types, shapes, and missing values
   * Removed duplicate rows

2. **Exploratory Data Analysis**

   * Distribution plots for numerical features
   * Survival rate comparisons across categorical features
   * Binning of age to reduce outlier impact

3. **Feature Engineering**

   * Encoding categorical variables (Sex, Embarked)
   * Creating age bins
   * Log transformation applied to skewed features such as Fare

4. **Model Training**
   Implemented the following models:

   * Logistic Regression
   * Random Forest
   * Support Vector Machine (SVM)
   * Naive Bayes
   * K-Nearest Neighbors (KNN)
   * XGBoost

5. **Hyperparameter Tuning**

   * GridSearchCV used to optimize Random Forest
   * Compared all model accuracies

---

## Results

* Random Forest with tuned hyperparameters achieved the best performance on the test data.
* Kaggle Public Leaderboard Score: **0.72727**

---

## Repository Structure

```
├── analysis.ipynb   # Jupyter notebook with analysis and modeling
├── myans.csv        # Submission file
├── train.csv        # training file
├── test.csv         # testing file
├── ACCURACY.png     # Model accuracy comparison chart
└── README.md        # Project documentation
```

---


