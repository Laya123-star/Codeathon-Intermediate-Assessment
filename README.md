# 🚗 Car Price Prediction – Regression Model Building

A supervised machine learning project focused on implementing and comparing  
multiple **regression algorithms** to model and predict car prices in the American market.

---

## 📘 Project Overview

This project is based on a business problem where a Chinese automobile company  
plans to enter the US market and wants to understand:

- Which variables significantly affect car price  
- How well these variables explain price variation  
- How pricing strategy can be optimized  

The goal of this project is to build and evaluate multiple regression models  
to identify the most accurate and reliable model for predicting car prices.

---

## 📂 Dataset Description

| Component | Description |
|------------|-------------|
| Records | 205 cars |
| Features | 25+ independent variables |
| Target Variable | `price` |
| Data Type | Numerical and Categorical |

The dataset includes attributes such as:

- Engine size
- Horsepower
- Fuel type
- Drive wheel type
- Car dimensions
- Brand
- Mileage
- Technical specifications

---

## 🎯 Project Objectives

This project fulfills the following academic requirements:

1. **Loading and Preprocessing (5 marks)**  
2. **Model Implementation (10 marks)**  
3. **Model Evaluation (5 marks)**  
4. **Feature Importance Analysis (2 marks)**  
5. **Hyperparameter Tuning (2 marks)**  
6. **Timely Submission (1 mark)**  

**Total: 25 Marks**

---

# 🧹 Data Preprocessing Steps

✔ Dataset loading into Pandas DataFrame  
✔ Initial exploration (shape, info, summary statistics)  
✔ Missing value verification  
✔ Duplicate record check  
✔ Outlier detection using boxplots  
✔ Feature engineering (brand extraction and cleaning)  
✔ Categorical variable encoding  
✔ Train–Test split (80–20)  
✔ Feature scaling using `StandardScaler`  

---

# 🤖 Regression Models Implemented

The following five regression algorithms were implemented:

## 1️⃣ Linear Regression
- Baseline linear model
- Assumes linear relationship between features and price

## 2️⃣ Decision Tree Regressor
- Captures non-linear relationships
- May overfit without pruning

## 3️⃣ Random Forest Regressor
- Ensemble of decision trees
- Reduces overfitting
- Delivered the best performance

## 4️⃣ Gradient Boosting Regressor
- Sequential boosting approach
- Minimizes prediction errors iteratively

## 5️⃣ Support Vector Regressor (SVR)
- Margin-based regression model
- Requires feature scaling

---

# 📊 Model Evaluation Metrics

Each model was evaluated using:

- **R-squared (R² Score)**  
- **Mean Squared Error (MSE)**  
- **Mean Absolute Error (MAE)**  

These metrics help measure:

- Variance explained by the model  
- Prediction accuracy  
- Error magnitude  

---

# 📈 Model Comparison

All models were trained and evaluated on the same dataset.

Key findings:

- Random Forest Regressor achieved the highest R² score.
- It produced the lowest MSE and MAE.
- It handled non-linear feature interactions effectively.

---

# 🏆 Best Performing Model

### ✅ Random Forest Regressor

**Reasons for best performance:**

- Captures complex relationships
- Reduces variance through ensemble averaging
- Provides stable and reliable predictions
- Handles feature interactions efficiently

---

# 🔍 Feature Importance Analysis

Feature importance was extracted using the Random Forest model.

Significant variables influencing car price include:

- Engine size  
- Curb weight  
- Horsepower  
- Car width  
- Brand  

This insight helps management understand pricing dynamics in the US market.

---

# ⚙ Hyperparameter Tuning

Hyperparameter tuning was performed using:

- `Pipeline`
- `GridSearchCV`
- 5-Fold Cross Validation

Parameters tuned:

- `n_estimators`
- `max_depth`
- `min_samples_split`

After tuning:

- R² score improved slightly  
- Prediction error reduced  
- Model generalization improved  

---

# 🛠 Tech Stack

| Tool | Purpose |
|------|----------|
| Python | Programming language |
| Pandas | Data manipulation |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Seaborn | Statistical plotting |
| Scikit-learn | Machine learning models |
| Google Colab | Development environment |

---

# 📁 Repository Structure

```
Car-Price-Prediction-Regression/
│
├── CarPrice_Assignment.csv
├── Car_Price_Prediction.ipynb
├── README.md
```

---

# 🚀 How to Run the Project

1. Open the notebook in **Google Colab**
2. Upload the dataset if required
3. Run all cells sequentially
4. Review model comparison results

---

# 📌 Business Insight

This project enables management to:

- Identify key pricing drivers
- Optimize product features
- Align pricing strategy with market demand
- Make data-driven business decisions

---

# 📚 Academic Submission Note

This repository is submitted as part of a Machine Learning module assignment.  
It demonstrates regression modeling, evaluation, feature analysis, and hyperparameter tuning  
on a real-world automobile pricing dataset.
