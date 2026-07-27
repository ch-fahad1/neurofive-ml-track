# 🚀 Week 3 - Model Evaluation & Hyperparameter Tuning

## 📌 Project Overview

In this project, I revisited my Titanic Survival Prediction model and learned how to evaluate machine learning models beyond accuracy.

I used additional evaluation metrics such as **Precision, Recall, and F1-Score** and improved the model using **GridSearchCV** for hyperparameter tuning.

---

## 🎯 Objectives

- Evaluate a classification model using multiple metrics.
- Understand why accuracy alone can be misleading.
- Apply Hyperparameter Tuning using GridSearchCV.
- Compare the original and tuned models.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab

---

## 📂 Dataset

**Titanic Dataset**

Target Variable:

- Survived

Features Used:

- Pclass
- Age
- SibSp
- Parch
- Fare
- Sex
- Embarked

Removed Columns:

- PassengerId
- Name
- Ticket
- Cabin

---

## 📋 Project Workflow

### 1. Import Libraries

Imported all required Python libraries for data processing, model training, evaluation, and hyperparameter tuning.

---

### 2. Data Preprocessing

- Filled missing values
- Removed unnecessary columns
- Encoded categorical variables using `pd.get_dummies()`

---

### 3. Train-Test Split

Split the dataset into:

- Training Data (70%)
- Testing Data (30%)

using `train_test_split()`.

---

### 4. Logistic Regression Model

Trained the baseline Logistic Regression model and generated predictions on the test dataset.

---

### 5. Model Evaluation

Evaluated the model using:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Classification Report

---

### 6. Hyperparameter Tuning

Used **GridSearchCV** with 5-fold Cross Validation.

Hyperparameters Tuned:

- C
- Solver

Best Parameters:

```python
{'C': 0.1, 'solver': 'lbfgs'}
```

---

## 📊 Results

### Original Model

| Metric | Value |
|---------|------:|
| Accuracy | **80.97%** |
| Precision | **0.79** |
| Recall | **0.73** |
| F1-Score | **0.76** |

---

### Tuned Model

| Metric | Value |
|---------|------:|
| Accuracy | **81.72%** |
| Precision | **0.82** |
| Recall | **0.71** |
| F1-Score | **0.76** |

---

## 📈 Performance Comparison

| Metric | Original | Tuned |
|---------|---------:|-------:|
| Accuracy | 80.97% | **81.72%** |
| Precision | 0.79 | **0.82** |
| Recall | **0.73** | 0.71 |
| F1-Score | 0.76 | 0.76 |

---

## 📚 Key Learnings

During this project, I learned:

- Accuracy is not always the best metric for evaluating a classification model.
- Precision measures how accurate positive predictions are.
- Recall measures how many actual positive cases the model correctly identifies.
- F1-Score provides a balance between Precision and Recall.
- GridSearchCV helps automatically find the best hyperparameters for a machine learning model.
- Hyperparameter tuning can improve model performance without changing the algorithm.

---

## 🏁 Conclusion

The original Logistic Regression model achieved an accuracy of **80.97%**.

After applying **GridSearchCV**, the model achieved **81.72%** accuracy.

Although the improvement was small, the tuning process selected a better combination of hyperparameters and demonstrated how model optimization works in real-world machine learning projects.

---

## 📁 Project Structure

```text
Week03/
│
├── Model_Evaluation_and_Tuning.ipynb
└── README.md
```

---

## 👨‍💻 Author

**Muhammad Fahad**

BS Computer Science Student

Learning Python • Data Science • Machine Learning
