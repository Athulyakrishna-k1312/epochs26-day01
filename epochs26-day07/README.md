# Customer Segmentation using K-Means Clustering

**Name:** Athulyakrishna K
**MUID:** *athulyakrishnak@mulearn*

## 📌 Project Overview

This project performs **Customer Segmentation** using the **K-Means Clustering** algorithm, an unsupervised machine learning technique. The objective is to group customers with similar characteristics based on their demographic and spending behavior.

The project also uses **Principal Component Analysis (PCA)** to reduce the dataset to two dimensions for visualization, making it easier to interpret the identified customer segments.

---

## 📂 Dataset

**Dataset:** Mall Customer Segmentation Dataset

### Features

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📋 Project Workflow

### 1. Data Loading
- Loaded the Mall Customer Segmentation dataset using Pandas.

### 2. Data Preprocessing
- Checked dataset structure and statistics.
- Verified that there were no missing values.
- Removed the `CustomerID` column since it does not contribute to clustering.
- Encoded the `Gender` column into numerical values.
- Applied **StandardScaler** to standardize all features before clustering.

### 3. Elbow Method
- Used the Elbow Method to determine the optimal number of clusters.
- The elbow point was observed at **k = 4**.
- Therefore, the K-Means model was trained using **4 clusters**.

### 4. K-Means Clustering
- Trained the K-Means clustering model.
- Assigned each customer to one of the four clusters.
- Generated cluster profiles by calculating the average characteristics of each cluster.

### 5. Principal Component Analysis (PCA)
- Reduced the dataset from multiple dimensions to two principal components.
- Visualized the customer segments using a scatter plot.
- Reported the variance explained by the principal components.

---

# 📊 Cluster Summary

## Cluster 0 – Mature Average Spenders

**Characteristics**
- Older customers
- Moderate annual income
- Moderate spending score

**Business Strategy**
- Improve customer retention through loyalty programs.
- Recommend products suitable for mature customers.

---

## Cluster 1 – High Income, Low Spending Customers

**Characteristics**
- High annual income
- Low spending score

**Business Strategy**
- Encourage purchases using personalized offers.
- Promote premium products and exclusive memberships.

---

## Cluster 2 – Young Male High Spenders

**Characteristics**
- Mostly male customers
- Young age group
- High spending score

**Business Strategy**
- Promote trendy products.
- Use digital marketing campaigns and seasonal offers.

---

## Cluster 3 – Young Female High Spenders

**Characteristics**
- Mostly female customers
- Young age group
- High spending score

**Business Strategy**
- Advertise fashion and lifestyle products.
- Introduce loyalty programs and personalized recommendations.

---

# 📈 Results

- Successfully identified **4 customer segments** using K-Means Clustering.
- Used PCA to visualize customer clusters in two dimensions.
- PCA Explained Variance Ratio: **[0.33690046 0.26230645]**
- Total Explained Variance: **0.5992069019819846**

---

# 💡 Key Observations

- Customers can be grouped into distinct segments based on age, annual income, and spending behavior.
- High-income customers do not always spend more.
- Young customers generally exhibit higher spending behavior.
- Customer segmentation helps businesses design personalized marketing strategies and improve customer engagement.

---

# ✅ Conclusion

This project successfully demonstrated the use of **Unsupervised Machine Learning** for customer segmentation using **K-Means Clustering**.

The Elbow Method helped determine the optimal number of clusters, while PCA provided an effective two-dimensional visualization of customer groups.

The identified customer segments can help businesses:
- Improve targeted marketing.
- Enhance customer satisfaction.
- Increase customer retention.
- Optimize promotional strategies based on customer behavior.

---

## 📷 Output

The notebook includes:
- Data preprocessing
- Elbow Method graph
- K-Means clustering
- Cluster profiling
- PCA visualization
- Business insights

---


## ⭐ Assignment

**Epochs '26 – Assignment 7**

**Topic:** Customer Segmentation using K-Means Clustering and PCA
# Conclusion

This project demonstrates the complete machine learning workflow for customer churn prediction, including data preprocessing, feature encoding, model development, evaluation, and comparison. Among the evaluated models, **Logistic Regression** achieved the best overall performance and was selected as the final model. Such predictive models can help organizations identify customers at risk of leaving and support data-driven customer retention strategies.

