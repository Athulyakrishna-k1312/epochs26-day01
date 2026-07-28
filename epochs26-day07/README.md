# Customer Churn Prediction using Machine Learning

## Participant Details

**Name:** Athulyakrishna K
**MUID:** *athulyakrishnak@mulearn*

---

# Business Objective

Customer churn is a major challenge for subscription-based businesses. Retaining existing customers is generally more cost-effective than acquiring new ones. The objective of this project is to develop machine learning models that can accurately predict whether a customer is likely to churn based on their demographic information, subscription details, and usage patterns. These predictions can help businesses take proactive measures to improve customer retention.

---

# Dataset Overview

* **Dataset Name:** Customer Churn Dataset
* **Source:** Kaggle
* **Problem Type:** Binary Classification
* **Target Variable:** `Churn`

The dataset contains customer-related information such as age, gender, subscription type, usage frequency, payment behavior, customer tenure, and total spending. The goal is to classify customers into two categories:

* **0:** Customer will not churn
* **1:** Customer is likely to churn

---

# Features and Target Variable

## Input Features

* CustomerID *(removed during preprocessing)*
* Age
* Gender
* Tenure
* Usage Frequency
* Support Calls
* Payment Delay
* Subscription Type
* Contract Length
* Total Spend
* Last Interaction

## Target Variable

* **Churn**

---

# Data Preprocessing Pipeline

The following preprocessing steps were performed:

* Loaded separate training and testing datasets.
* Checked dataset structure and data types.
* Identified and removed missing values.
* Encoded categorical variables using **LabelEncoder**.
* Removed the **CustomerID** column as it is not useful for prediction.
* Separated features and target variable.
* Applied **StandardScaler** for Logistic Regression.
* Used the provided training and testing datasets directly for model development and evaluation.

---

# Machine Learning Models Implemented

The following classification models were trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

---

# Evaluation Metrics

The models were evaluated using the following performance metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

---

# Model Performance Comparison

| Model               |   Accuracy |  Precision |     Recall |   F1 Score |
| ------------------- | ---------: | ---------: | ---------: | ---------: |
| Logistic Regression | **0.6325** |     0.9764 | **0.3607** | **0.5268** |
| Decision Tree       |     0.5838 | **0.9802** |     0.2717 |     0.4254 |
| Random Forest       |     0.5837 |     0.9811 |     0.2711 |     0.4249 |

---

# Best Model

### Logistic Regression

Logistic Regression achieved the best overall performance among the three models.

### Justification

* Highest Accuracy (**63.25%**)
* Highest Recall (**36.07%**)
* Highest F1-Score (**52.68%**)
* Very high Precision (**97.64%**)

Considering all evaluation metrics together, Logistic Regression provides the best balance between identifying churning customers and minimizing incorrect predictions.

---

# Key Observations

* Logistic Regression outperformed Decision Tree and Random Forest on this dataset.
* All three models achieved very high precision, indicating that predicted churn cases were usually correct.
* Recall values were comparatively lower, suggesting that several actual churn cases were not detected.
* The dataset may contain class imbalance, which can affect recall performance.
* Customer behavior, subscription details, and payment history appear to be useful predictors of churn.

---

# Business Recommendations

* Identify customers with a high probability of churning and engage them proactively.
* Offer personalized discounts or loyalty rewards to high-risk customers.
* Improve customer support for users with frequent support requests.
* Monitor customers with long payment delays and high usage patterns.
* Continuously retrain the model using newly collected customer data to improve prediction performance.

---

# Future Improvements

* Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
* Handle class imbalance using techniques such as SMOTE or class-weighted models.
* Explore advanced ensemble algorithms such as XGBoost, LightGBM, or CatBoost.
* Apply feature engineering to create more informative variables.
* Deploy the trained model as a web application for real-time customer churn prediction.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

# Conclusion

This project demonstrates the complete machine learning workflow for customer churn prediction, including data preprocessing, feature encoding, model development, evaluation, and comparison. Among the evaluated models, **Logistic Regression** achieved the best overall performance and was selected as the final model. Such predictive models can help organizations identify customers at risk of leaving and support data-driven customer retention strategies.

