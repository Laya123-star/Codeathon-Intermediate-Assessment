# 🚗 Car Price Prediction – Regression Model Building

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/MachineLearning-Regression-orange)
![Model](https://img.shields.io/badge/Model-RandomForest-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A supervised machine learning project focused on implementing and comparing multiple **regression algorithms** to predict car prices in the American automobile market.

---

## 🚀 Run Notebook in Google Colab

Click below to open the notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E6Ly_71RE6L3qYvuHoF_AMV8sBa_gzxZ)

---

# 📘 Project Overview

This project is based on a business problem where an automobile company plans to enter the US market and aims to understand key factors influencing car prices.

The complete pipeline includes:

* Data Cleaning
  
* Exploratory Data Analysis (EDA)
  
* Feature Engineering
  
* Feature Scaling
  
* Model Building
  
* Model Evaluation
  
* Hyperparameter Tuning
  
* Model Comparison

The goal is to build an accurate regression model to predict car prices and support data-driven pricing strategies.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Identify variables affecting car price

🔹 Analyze relationships between features and price

🔹 Build multiple regression models

🔹 Compare model performances

🔹 Optimize the best model using hyperparameter tuning

🔹 Provide business insights for pricing strategy

---

# 📂 Dataset Description

| Component       | Description               |
| --------------- | ------------------------- |
| Records         | 205 cars                  |
| Features        | 25+ independent variables |
| Target Variable | price                     |
| Data Type       | Numerical and Categorical |

### Key Features:

* Engine size
  
* Horsepower
  
* Fuel type
  
* Drive wheel type
  
* Car dimensions
  
* Brand
  
* Mileage
  
* Technical specifications

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

✔ Loaded dataset using Pandas

✔ Initial exploration (shape, info, summary statistics)

✔ Handled missing values

✔ Removed duplicate records

✔ Detected and handled outliers

✔ Feature engineering (brand extraction)

✔ Encoded categorical variables

✔ Split dataset into **Training (80%) and Testing (20%)**

✔ Scaled features using **StandardScaler**

---

# 📊 Exploratory Data Analysis (EDA)

Visualizations used:

* Histogram
  
* Box Plot
  
* Heatmap Correlation
  
* Scatter Plot

### Insights:

* Identified strong relationships between engine size, horsepower, and price
  
* Detected outliers affecting model performance
  
* Understood feature distributions

---

# 🤖 Regression Models Implemented

The following models were trained and evaluated:

* Linear Regression
  
* Decision Tree Regressor
  
* Random Forest Regressor
  
* Gradient Boosting Regressor
  
* Support Vector Regressor (SVR)
  
* Pruned Decision Tree

---

# 📊 Model Performance (Before Tuning)

| Model                       | R² Score | MSE    | MAE    |
| --------------------------- | -------- | ------ | ------ |
| Random Forest Regressor     | 0.913    | 0.0136 | 0.0882 |
| Gradient Boosting Regressor | 0.908    | 0.0143 | 0.0838 |
| Linear Regression           | 0.879    | 0.0189 | 0.1054 |
| Decision Tree Regressor     | 0.860    | 0.0219 | 0.1062 |
| Support Vector Regressor    | 0.831    | 0.0263 | 0.1051 |
| Pruned Decision Tree        | 0.831    | 0.0263 | 0.0958 |

✅ **Best Model:** Random Forest Regressor

❌ **Worst Model:** Pruned Decision Tree

---

# ⚙️ Hyperparameter Tuning

* Applied **GridSearchCV**
  
* Used **Pipeline** to prevent data leakage
  
* Performed **5-Fold Cross Validation**

### Parameters Tuned:

* n_estimators
  
* max_depth
  
* min_samples_split

---

# 📊 Model Performance (After Tuning)

| Model                   | R² Score | MSE    | MAE    |
| ----------------------- | -------- | ------ | ------ |
| Random Forest (Untuned) | 0.9129   | 0.0136 | 0.0882 |
| Random Forest (Tuned)   | 0.9131   | 0.0136 | 0.0847 |

🏆 **Best Model:** Tuned Random Forest Regressor

### Final Metrics:

* R² Score: **0.9131**
  
* MSE: **0.0136**
  
* MAE: **0.0847**

✅ Model performance improved after hyperparameter tuning

---

# 🏆 Final Model

✔ **Random Forest Regressor selected**

✔ Optimized using hyperparameter tuning

✔ Provides stable and accurate predictions

---

# 🔍 Feature Importance Analysis

Important features influencing car price:

* Engine size
  
* Curb weight
  
* Horsepower
  
* Car width
  
* highwaympg

These features play a major role in determining car pricing strategy.

---

# 📊 Evaluation Metrics

* R² Score
  
* Mean Squared Error (MSE)
  
* Mean Absolute Error (MAE)

---

# ⚠️ Limitations

* Dataset size is relatively small (205 records)
  
* Limited features may not capture all real-world pricing factors
  
* Market dynamics and external economic factors are not included
  
* Model may not generalize well to different regions or time periods
  
* Performance may vary for unseen or highly diverse car categories

---

# 🛠 Tech Stack

| Tool                 | Purpose                   |
| -------------------- | ------------------------- |
| Python               | Programming language      |
| Pandas               | Data handling             |
| NumPy                | Numerical computation     |
| Matplotlib / Seaborn | Visualization             |
| Scikit-learn         | ML models & preprocessing |
| Google Colab         | Development               |

---

# 📁 Repository Structure

car-price-prediction/

│

├── CarPrice_Assignment.csv

├── Car_Price_Prediction.ipynb

├── README.md

---

# 🚀 How to Run the Project

### 1️⃣ Open Notebook

Click the **Google Colab link above**

---

### 2️⃣ Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

### 3️⃣ Run the Notebook

* Execute all cells step-by-step
  
* Analyze model performance

---

# 📌 Business Insight

This project helps:

* Identify key drivers of car pricing
  
* Optimize product features
  
* Support strategic pricing decisions
  
* Enable data-driven business planning

---

# 👤 Author

**Name:** Laya Mary Joy

**Organization:** Entri Elevate

**Date:** February 14, 2026

---

# ⭐ Acknowledgment

Thanks to **Entri Elevate** for guidance and support.

---

# 📌 Future Improvements

* Use larger and more diverse datasets
  
* Include real-time market data
  
* Try advanced models (XGBoost, LightGBM)
  
* Deploy as a web application

---
