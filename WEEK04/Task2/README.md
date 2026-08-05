# Ensemble Learning: Random Forest vs XGBoost

## Objective

The objective of this project is to compare ensemble learning algorithms with a baseline Logistic Regression model using the Titanic dataset.

## Dataset

- Titanic Dataset
- Total Records: 891

## Data Preprocessing

- Filled missing Age values using median.
- Filled missing Embarked values using mode.
- Dropped Cabin due to excessive missing values.

## Feature Engineering

Two new features were created:

- FamilySize
- IsAlone

## Models Used

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

## Model Comparison

| Model | Accuracy |
|--------|-----------|
| Logistic Regression | 80.60% |
| Random Forest | 77.91% |
| XGBoost | 77.91% |

## Feature Importance

### Random Forest

Top Features:

- Fare
- Age
- Sex_male
- Pclass
- FamilySize

### XGBoost

Top Features:

- Sex_male
- Pclass
- FamilySize
- Embarked_S
- Age

## Random Forest vs XGBoost

Random Forest builds many independent decision trees and combines their predictions using majority voting.

XGBoost builds trees sequentially, where each new tree learns from the mistakes of previous trees.

Although ensemble methods are generally more powerful, Logistic Regression achieved the highest accuracy on this dataset with the current settings.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Google Colab
