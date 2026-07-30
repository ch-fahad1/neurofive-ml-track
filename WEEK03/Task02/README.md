# Customer Churn Prediction

## Objective

The goal of this project is to predict whether a customer will leave the company (Churn) using Machine Learning models.

## Dataset

- Telco Customer Churn Dataset
- Total Records: 7043
- Features: 30
- Target: Churn (Yes/No)

## Project Workflow

- Imported and explored the dataset
- Checked dataset shape, data types, and missing values
- Converted TotalCharges to numeric values
- Filled missing values
- Removed customerID
- Converted categorical variables using pd.get_dummies()
- Split the dataset into training and testing sets (70/30)
- Trained Logistic Regression and Decision Tree models
- Compared both models
- Identified the top 3 important features using Decision Tree

## Model Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | **81.31%** |
| Decision Tree | **73.88%** |

## Top 3 Important Features

1. tenure
2. TotalCharges
3. MonthlyCharges

## Business Summary

Customers with month-to-month contracts and shorter tenure are more likely to leave the company. Customers paying higher monthly charges also show a higher risk of churn. Logistic Regression achieved better performance than the Decision Tree model. These insights can help businesses improve customer retention by targeting high-risk customers with better plans and offers.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
