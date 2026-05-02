# Breast Cancer Diagnosis Analysis

## Project Overview

This project focuses on analyzing breast cancer data to identify key factors that influence diagnosis and to build predictive models that classify tumors as **malignant** or **benign**.

The goal is to combine **data analysis, visualization, and machine learning** to extract meaningful insights and support decision-making in a healthcare context.

---

## Objectives

* Perform data cleaning and preprocessing
* Explore relationships between medical features
* Identify key predictors of cancer diagnosis
* Build and evaluate classification models
* Interpret results from a data analysis perspective

---

## Dataset

* **Source:** Breast Cancer Wisconsin Dataset
* **Samples:** 569 patients
* **Features:** 30 numerical features (radius, texture, perimeter, area, etc.)
* **Target Variable:**

  * `0` → Benign
  * `1` → Malignant

---

## Data Analysis & Insights

### Key Observations:

* Features such as **concave points**, **radius**, and **perimeter** show strong correlation with malignant tumors
* Malignant tumors tend to have:

  * Larger size-related measurements
  * Higher irregularity in shape

### Correlation Analysis:

* High multicollinearity detected among size-related features
* Feature reduction applied to improve model performance and interpretability

---

## Methodology

### 1. Data Cleaning

* Removed irrelevant columns (`id`, empty columns)
* Converted categorical diagnosis into numerical format
* Checked for missing values and duplicates

### 2. Feature Selection

* Removed highly correlated features (threshold > 0.92)

### 3. Data Preparation

* Train-test split (80/20)
* Feature scaling using StandardScaler

---

## Models Used

### 🔹 Logistic Regression

* Simple, interpretable baseline model

### 🔹 Random Forest Classifier

* Ensemble model to capture non-linear relationships

---

## 📈 Model Performance

| Model               | Accuracy | Precision | Recall   |
| ------------------- | -------- | --------- | -------- |
| Logistic Regression | 97.3%    | High      | Strong   |
| Random Forest       | 95.6%    | High      | Moderate |

### Key Insight:

* Logistic Regression performed slightly better on test data
* It achieved **higher recall**, meaning fewer missed cancer cases

In medical diagnosis, minimizing **false negatives** is critical

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* Confusion Matrix
* Cross-validation (Random Forest)

---

## Key Takeaways

* Certain geometric features of cells are strong indicators of malignancy
* Simpler models like Logistic Regression can outperform complex models when data is well-structured
* Model evaluation should prioritize **recall** in healthcare applications

---

## Tools & Technologies

* Python
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn

---





