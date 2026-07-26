# 🚗 Car Price Prediction using Machine Learning

## 📌 Business Objective

The objective of this project is to build and compare multiple machine learning regression models to predict the selling price of used cars based on their specifications. Accurate price prediction helps buyers, sellers, and dealerships estimate a fair market value for used vehicles.

---

## 📂 Dataset Overview

This project uses the **CarDekho Used Car Dataset**, which contains information about used cars, including their brand, model, age, mileage, engine specifications, fuel type, transmission type, and selling price.

- **Source:** CarDekho Used Car Dataset
- **Total Records:** 11,905 (before preprocessing)
- **Target Variable:** `selling_price`

---

## 🎯 Features and Target Variable

### Target Variable

- `selling_price`

### Numerical Features

- vehicle_age
- km_driven
- mileage
- engine
- max_power
- seats

### Categorical Features

- car_name
- brand
- model
- seller_type
- fuel_type
- transmission_type

---

## 🛠 Data Preprocessing

The following preprocessing steps were performed:

- Removed the unnecessary `Unnamed: 0` column.
- Removed rows containing missing values.
- Applied One-Hot Encoding to categorical features.
- Split the dataset into training and testing sets (80:20).

---

## 📊 Exploratory Data Analysis (EDA)

EDA was performed to better understand the dataset using:

- Selling Price Distribution
- Brand Distribution
- Fuel Type Distribution
- Transmission Type Distribution
- Vehicle Age vs Selling Price
- Kilometers Driven vs Selling Price
- Correlation Heatmap

### Key Observations

- Most cars belong to the lower selling price range.
- Maruti and Hyundai are the most common brands.
- Petrol and Diesel vehicles dominate the dataset.
- Older vehicles generally have lower selling prices.
- Higher engine capacity and maximum power positively influence selling price.

---

## 🤖 Regression Models Implemented

The following regression models were trained and evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

---

## 📈 Model Performance Comparison

| Model | MAE | MSE | RMSE | R² Score |
|------|------:|------:|------:|------:|
| Linear Regression | 176056.27 | 1.5589e+11 | 394830.06 | 0.7929 |
| Decision Tree Regressor | 122317.67 | 9.3946e+10 | 306506.12 | 0.8752 |
| Random Forest Regressor | **96925.20** | **5.3207e+10** | **230667.14** | **0.9293** |

---

## 🏆 Best Performing Model

The **Random Forest Regressor** achieved the best performance among all models.

### Why Random Forest?

- Highest R² Score (**0.9293**)
- Lowest Mean Absolute Error (MAE)
- Lowest Mean Squared Error (MSE)
- Lowest Root Mean Squared Error (RMSE)

Random Forest combines multiple decision trees, enabling it to capture complex relationships within the data while reducing overfitting. This results in more accurate and robust predictions.

---

## 📌 Strengths and Limitations

### Linear Regression

**Strengths**

- Simple and easy to interpret
- Fast training and prediction

**Limitations**

- Assumes a linear relationship
- Performs poorly on complex nonlinear data

---

### Decision Tree Regressor

**Strengths**

- Captures nonlinear relationships
- Easy to understand and visualize

**Limitations**

- Can overfit the training data
- Sensitive to small changes in the dataset

---

### Random Forest Regressor

**Strengths**

- High prediction accuracy
- Reduces overfitting
- Handles nonlinear relationships effectively

**Limitations**

- Higher computational cost
- Less interpretable than a single decision tree

---

## 🔍 Key Observations

- Engine power (`max_power`) has a strong positive relationship with selling price.
- Vehicle age negatively affects selling price.
- One-Hot Encoding successfully converted categorical variables into numerical features.
- Ensemble learning (Random Forest) significantly improved prediction accuracy over individual models.

---

## 🚀 Future Improvements

- Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Apply cross-validation for more reliable model evaluation.
- Remove outliers to improve model performance.
- Experiment with advanced boosting algorithms such as XGBoost, LightGBM, or CatBoost.
- Engineer additional features to improve predictive performance.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## 📌 Conclusion

Three regression models were developed and compared to predict used car selling prices. Among them, the **Random Forest Regressor** delivered the best performance with an **R² Score of 0.9293**, indicating that it explains approximately **92.93%** of the variation in car prices. Based on the evaluation metrics, Random Forest was selected as the final model for this project.

---

## 👨‍💻 Author

**Athulyakrishna K**

Final Year B.Tech Information Technology Student

Government Engineering College Sreekrishnapuram
