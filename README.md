# Breast Cancer Prediction Model

## Problem Statement
The goal of this project is to predict whether a patient has breast cancer or not using the Breast Cancer dataset.

This is a *classification problem* and the output belongs to one of two categories:
- *M (Malignant)* = 0 (Cancerous)
- *B (Benign)* = 1 (Not Cancerous)

## Dataset
- *Source:* Breast Cancer dataset
- *Total columns:* 33
- *Target:* Diagnosis (M or B)
- *Features:* 30 numerical features after dropping ID, Unnamed:32 and Diagnosis columns

## What I Did
- Explored the data using data.info() and data.describe()
- Checked for null values
- Dropped irrelevant columns (ID, Unnamed:32, Diagnosis)
- Encoded target variable: M = 0, B = 1
- Split data into training and test sets (80/20 split)
  - X_train: (455, 30)
  - X_test: (114, 30)
- Scaled features using feature scaling
- Trained multiple machine learning models

## Models Tested & Results

| Model | Parameters | Accuracy |
|---|---|---|
| Logistic Regression | max_iter=1000 | *97.36%* |
| Support Vector Machine | C=800, kernel=linear, random_state=42 | *97.36%* |
| Decision Tree | max_depth=4, random_state=50 | 93.85% |
| Pipeline (Linear Regression) | — | R² Score: 0.7656, MSE: 0.05 |

## Best Model
Both *Logistic Regression* and *Support Vector Machine* achieved the highest accuracy of *97.36%*, making them the strongest performers for this classification task.

## Key Takeaways
- Logistic Regression and SVM both achieved 97.36% accuracy showing strong performance on medical classification data
- Decision Tree performed well at 93.85% with controlled depth to prevent overfitting
- The Pipeline with Linear Regression achieved an R² score of 0.7656 and a very low MSE of 0.05
- Feature scaling significantly impacts model performance on this dataset

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn

## Author
Jemilah Alao | Data Analyst
[LinkedIn](https://www.linkedin.com/in/jemilah-alao-8a684528a)
