# 🛒 Online Shoppers Purchase Intentions Prediction

## 📌 Project Overview
This project analyzes **user browsing behavior** and **session-level data** to predict whether a customer will make a purchase during an online shopping session.  
We use **Exploratory Data Analysis (EDA)** and **XGBoost** to uncover insights and build a high-performance predictive model.

**Dataset:** [UCI Online Shoppers Purchasing Intention Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset)

---

## 🎯 Objectives
- Understand how browsing patterns influence online purchase decisions.
- Compare sessions that resulted in purchases vs. those that didn’t.
- Build and optimize a **binary classification** model using **XGBoost**.
- Evaluate model performance using multiple metrics.
- Identify the most influential features affecting purchase likelihood.

---

## 📂 Dataset Details
- **Rows:** 12,330 sessions
- **Columns:** 18 behavioral features + 1 target variable (`Revenue`)
- **Key Features:**
  - `Administrative`, `Administrative_Duration`
  - `Informational`, `Informational_Duration`
  - `ProductRelated`, `ProductRelated_Duration`
  - `BounceRates`, `ExitRates`, `PageValues`, `SpecialDay`
  - `OperatingSystems`, `Browser`, `Region`, `TrafficType`
  - `VisitorType`, `Weekend`, `Month`
  - **Target:** `Revenue` (1 = Purchase, 0 = No Purchase)

---

## 🛠️ Project Workflow

### 1. Data Cleaning & Preprocessing
- Handle missing values
- Encode categorical variables (`VisitorType`, `Weekend`, `Month`)
- Convert boolean to integer where needed
- Prepare features and target variables

### 2. Exploratory Data Analysis (EDA)
- Compare purchase vs. non-purchase sessions
- Visualize trends with histograms, bar plots, and heatmaps
- Identify correlations between features

### 3. Modeling with XGBoost
- Train-test split (80-20)
- Train an **XGBoost Classifier**
- Hyperparameter tuning with `GridSearchCV`
- Feature importance extraction

### 4. Model Evaluation
- **Accuracy**
- **Precision, Recall, F1-Score**
- **ROC-AUC Score**
- Confusion Matrix

---

## 📊 Key Insights
- Returning visitors are more likely to make purchases than new visitors.
- Higher `PageValues` strongly correlates with completed purchases.
- Special days and weekends have varying effects on purchase rates.

---

## 📈 Results
| Metric       | Score |
|--------------|-------|
| Accuracy     | XX%   |
| Precision    | XX%   |
| Recall       | XX%   |
| F1-Score     | XX%   |
| ROC-AUC      | XX%   |

*(Replace XX% with your actual model scores after training)*
