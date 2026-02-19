# 🏠 King County Housing Price Prediction
[![Python Version](https://img.shields.io)](https://www.python.org)
[![ML Framework](https://img.shields.io)](https://scikit-learn.org)

## 📌 Project Overview
In this project, I acted as a **Data Analyst for a Real Estate Investment Trust (REIT)**. My objective was to build a predictive model to estimate residential property values in King County, USA. By analyzing structural and geographical features, this project provides data-driven insights to assist the trust in making informed investment decisions.

---

## 📑 Table of Contents
* [About the Dataset](#about-the-dataset)
* [Data Processing Pipeline](#data-processing-pipeline)
* [Exploratory Data Analysis](#exploratory-data-analysis)
* [Model Development & Evaluation](#model-development--evaluation)
* [Key Findings](#key-findings)
* [Project Structure](#project-structure)
* [Dependencies](#dependencies)

---

## 📊 About the Dataset
The dataset contains historical sales data from **May 2014 to May 2015** for King County, Washington. It consists of **21,613 observations** with features including:
* **Target:** `price`
* **Key Features:** `sqft_living`, `waterfront`, `grade`, `bedrooms`, and `bathrooms`.

---

## 🛠 Data Processing Pipeline

### 1. Data Wrangling
* **Feature Selection:** Removed non-predictive identifiers to reduce noise.
* **Imputation:** Cleaned the dataset by handling missing values in structural features using mean-based imputation.

### 2. Exploratory Data Analysis (EDA)
* Developed **Correlation Heatmaps** to isolate the most impactful price predictors.
* Conducted **Categorical Analysis** (e.g., waterfront vs. inland) using boxplots to identify premium market segments.
* Validated linear assumptions using **Regression plots** for square footage attributes.

### 3. Model Development & Evaluation
I implemented a tiered modeling approach to find the most accurate prediction:
* **Scikit-Learn Pipelines:** Integrated `StandardScaler` and `PolynomialFeatures` for a clean, reproducible workflow.
* **Ridge Regression:** Applied L2 Regularization ($\alpha = 0.1$) to optimize the model and prevent overfitting, ensuring better performance on real-world test data.

---

## 🏆 Key Findings
* **Primary Driver:** `sqft_living` remains the strongest predictor of price across all models.
* **Premium Assets:** Properties with a waterfront view show a significantly higher median value, representing a niche investment opportunity for the Trust.
* **Model Optimization:** Using **Polynomial Features** allowed the model to capture complex, non-linear relationships that a standard linear model could not.

---

## 📂 Project Structure
* `House_Sales_King_County.ipynb`: The primary Jupyter Notebook containing the full analysis, code, and visualizations.
* `README.md`: Project summary and technical documentation.

---

## 📦 Dependencies
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`

---
**Author:** [Abhishek Maurya]  
**Course:** Data Analysis with Python (Coursera/IBM)
