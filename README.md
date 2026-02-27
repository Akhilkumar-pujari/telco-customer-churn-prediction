# Telco Customer Churn Prediction

## 📌 Project Overview
This project builds an end-to-end machine learning system to predict customer churn for a telecommunications company. The goal is to identify at-risk customers early and estimate potential revenue savings through targeted retention strategies.

---

## 🎯 Business Objective
Customer churn directly impacts revenue. By identifying customers likely to churn, the company can proactively engage them with retention offers.

This model helps:
- Identify high-risk customers
- Understand key churn drivers
- Estimate potential financial impact

---

## 📊 Dataset
- 7,043 customer records
- 33 features including demographics, services, contract type, tenure, and billing details
- Target variable: **Churn Value (0 = No, 1 = Yes)**

---

## 🛠️ Methodology

### 1️⃣ Data Cleaning
- Removed leakage variables (Churn Label, Churn Score, Churn Reason)
- Converted Total Charges to numeric
- Dropped high-cardinality geographic features
- Handled categorical variables using OneHotEncoding

### 2️⃣ Modeling
Models implemented:
- Logistic Regression (with class balancing)
- Random Forest

Preprocessing:
- StandardScaler for numeric features
- OneHotEncoder for categorical features
- Pipeline-based architecture

---

## 📈 Model Performance

### Logistic Regression (Primary Model)
- Accuracy: 74%
- Recall (Churn class): 78%
- ROC-AUC: **0.85**

### Random Forest
- Accuracy: 81%
- Recall (Churn class): 53%

Although Random Forest had higher accuracy, Logistic Regression was chosen due to significantly higher recall for churn customers.

---

## 🔍 Key Churn Drivers

### Factors Increasing Churn:
- Month-to-month contracts
- Fiber optic internet service
- Higher total charges
- Electronic check payment method

### Factors Decreasing Churn:
- Two-year contracts
- Longer tenure
- Tech support & online security
- Customers with dependents

---

## 💰 Estimated Business Impact

Assuming:
- $70 average monthly revenue
- 30% retention success rate

The model could potentially save:

**~87 customers annually**  
**~$73,000 in annual revenue**

---

## 📊 Behavioral Insights

- Month-to-month customers have ~42% churn rate
- Customers in first year show ~47% churn rate
- Two-year contracts show <3% churn rate

This suggests early-stage customers and flexible contracts require targeted retention strategies.

---

## 🚀 Tools & Technologies

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 📂 Files Included

- `telco_churn_prediction.ipynb` – Full analysis notebook
- `telco_churn_prediction.html` – Rendered notebook for quick viewing

---

## 📌 Author
Akhil Kumar Pujari  
Master’s in Business Analytics  
