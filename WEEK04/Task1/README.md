# Titanic Survival Prediction using Machine Learning Pipeline

## Objective

The goal of this project is to predict passenger survival on the Titanic using a Machine Learning Pipeline built with Scikit-learn.

## Dataset

- Titanic Dataset
- Records: 891
- Target: Survived

## Feature Engineering

Two new features were created:

- FamilySize = SibSp + Parch + 1
- IsAlone = Whether the passenger was traveling alone

## Pipeline

A Scikit-learn Pipeline was created using:

- ColumnTransformer
- StandardScaler (Numerical Features)
- OneHotEncoder (Categorical Features)
- Logistic Regression

## Numerical Features

- Age
- Fare
- FamilySize

## Categorical Features

- Pclass
- Sex
- Embarked
- IsAlone

## Model Performance

Accuracy: **80.60%**

## Classification Metrics

- Precision
- Recall
- F1-Score

## Pipeline Saved

The trained pipeline was saved using Joblib as:

titanic_pipeline.pkl

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib
- Google Colab
