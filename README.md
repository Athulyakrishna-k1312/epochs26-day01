# Netflix Movies & TV Shows Dataset Exploration

## Objective

The objective of this assignment is to explore the Netflix Movies & TV Shows dataset, identify potential business problems, determine an appropriate Machine Learning problem, and perform basic exploratory data analysis using Pandas.

---

## Dataset Overview

The Netflix Movies & TV Shows dataset contains information about titles available on Netflix. Each record represents either a Movie or a TV Show and includes attributes such as:

- Title
- Type
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genre (Listed In)
- Description

The dataset can be used for content analysis, recommendation systems, market analysis, and predictive modeling.

---

## Business Problem

One potential business problem is:

**Predict whether a new title should be categorized as a Movie or a TV Show based on its attributes.**

This can help Netflix automate metadata generation and improve content management.

Another business problem is identifying trends in content production across different countries and years to support content acquisition decisions.

---

## Machine Learning Problem Framing

### Problem Type

**Classification**

### Justification

The target variable (**type**) contains two categories:

- Movie
- TV Show

Since the objective is to predict one of these categories, the problem is a Classification problem.

---

## Target Variable

**type**

---

## Key Features

Possible input features include:

- release_year
- rating
- duration
- listed_in
- country
- director
- cast

These features may help distinguish between Movies and TV Shows.

---

## Exploratory Data Analysis

The following analyses were performed:

- Dataset Shape
- Dataset Information
- Data Types
- Missing Values
- Summary Statistics
- Value Counts of Target Variable

---

## Key Observations

1. Movies are more common than TV Shows in the dataset.
2. Several columns such as **director**, **cast**, and **country** contain missing values.
3. Most titles were released during the last decade, showing a concentration of recent content.

---

## Tools Used

- Python
- Pandas
- Colab Notebook

---

## Conclusion

This dataset is suitable for exploratory data analysis and machine learning tasks. A Classification model can be developed to predict whether a title is a Movie or TV Show using its metadata.
