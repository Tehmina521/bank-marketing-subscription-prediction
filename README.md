# 📊 Bank Marketing Term Deposit Prediction

## 📌 Project Overview

This project builds a machine learning model to predict whether a customer will subscribe to a term deposit after a bank marketing campaign. 

The goal is to help financial institutions:
- Reduce marketing costs
- Improve campaign targeting
- Increase conversion rates
- Make data-driven decisions

---

## 🎯 Problem Statement

Banks conduct direct marketing campaigns to promote term deposits. However, contacting every customer is inefficient and expensive.

The objective of this project is to:
- Predict customer subscription (`yes` / `no`)
- Compare multiple classification models
- Evaluate performance using proper metrics
- Explain model predictions using SHAP

---

## 📂 Dataset Description

The dataset used is the **Bank Marketing Dataset**, which contains customer information such as:

- Age
- Job
- Marital status
- Education
- Balance
- Contact type
- Call duration
- Previous campaign outcome
- Target variable (`y`) – Term deposit subscription (Yes/No)

Target Variable:
- `1` → Subscribed
- `0` → Not Subscribed

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

- Removed duplicate rows
- Encoded target variable (`yes` → 1, `no` → 0)
- Separated categorical and numerical features
- Applied:
  - OneHotEncoding (categorical features)
  - StandardScaler (numerical features)
- Used Pipeline and ColumnTransformer for clean processing

---

## 📊 Exploratory Data Analysis (EDA)

EDA was performed using visualizations only:

- Target distribution analysis
- Age vs Subscription distribution
- Job type vs Subscription
- Call duration vs Subscription
- Previous campaign outcome vs Subscription

Key observations:
- The dataset is imbalanced (fewer subscribers)
- Longer call duration strongly correlates with subscription
- Previous successful campaigns increase probability of subscription

---

## 🤖 Model Building

Two classification models were implemented:

### 1️⃣ Logistic Regression
- Baseline model
- Linear decision boundary
- Interpretable coefficients

### 2️⃣ Random Forest
- Ensemble model
- Captures non-linear relationships
- Handles feature interactions better

---

## 📈 Model Evaluation

Models were evaluated using:

- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- ROC Curve
- ROC-AUC Score
- Combined ROC comparison

### Result:
Random Forest achieved a higher ROC-AUC score compared to Logistic Regression, indicating better classification performance.

---

## 🔍 Model Explainability (SHAP)

To ensure transparency:

- SHAP (SHapley Additive Explanations) was used
- 5 individual predictions were explained
- Waterfall plots showed feature contributions
- Confirmed impact of call duration, previous outcome, and demographics

This satisfies explainability requirements for model interpretation.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SHAP

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn shap
3. Run the Jupyter Notebook step by step

----

## 📌 Key Insights

- Random Forest outperformed Logistic Regression in overall predictive performance.
- Class imbalance impacts accuracy interpretation; accuracy alone is not a reliable metric.
- ROC-AUC provides a better evaluation measure for imbalanced classification problems.
- SHAP enhances model transparency by explaining individual predictions.
- Data-driven targeting can significantly improve marketing campaign efficiency and reduce operational costs.

---

## 📎 Conclusion

This project demonstrates how machine learning models, combined with appropriate evaluation metrics and explainability techniques, can be used to build reliable and interpretable marketing prediction systems. 

By leveraging predictive modeling and model interpretation tools, financial institutions can make more informed strategic decisions, optimize customer targeting, and improve campaign effectiveness.

---

## 👩‍💻 Author

**Tehmina Afzal**  
AI & Data Science Intern at ITSOLERA PVT LTD

