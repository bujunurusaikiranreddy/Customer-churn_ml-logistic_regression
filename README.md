# Customer-churn_ml-logistic_regression

## Model Description

This model predicts customer churn using a Logistic Regression algorithm.  The model is trained on a dataset containing various customer attributes and their churn status.

**Data Preprocessing:**

1. **Data Cleaning:** Handled missing values and duplicates. Replaced 'Error' values in 'avg_frequency_login_days' with 0.
2. **Feature Engineering:** Created 'joining_year' and 'joining_month' features from the 'joining_date' column.  Sorted data by these new features.
3. **Data Transformation:**  Converted categorical features into numerical representations using one-hot encoding.  Irrelevant or redundant features were dropped.  The 'last_visit_time' feature was removed.
4. **Data Splitting:** The dataset was split into training and testing sets (80/20 split) using `train_test_split`.

**Model Training:**

A Logistic Regression model was trained on the preprocessed training data.

**Model Evaluation:**

The model's performance was evaluated on the test set using the following metrics:

* **Accuracy:**  The overall accuracy of the model in predicting churn.
* **Confusion Matrix:** A matrix showing the counts of true positives, true negatives, false positives, and false negatives.
* **Classification Report:** Provides precision, recall, F1-score, and support for each class (churned or not churned).
