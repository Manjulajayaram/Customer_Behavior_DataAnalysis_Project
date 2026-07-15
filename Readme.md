#  Customer Churn Prediction

##  Project Overview
Customer churn is a critical problem for businesses, as losing customers directly impacts revenue.  
This project analyzes customer behavior and builds a machine learning model to predict whether a customer is likely to churn.

---

##  Objective
- Analyze customer data to identify churn patterns
- Build a predictive model to detect customers at risk of leaving
- Provide actionable business insights to reduce churn

---

##  Dataset
- Telco Customer Churn Dataset
- Contains customer demographics, services, billing, and churn information

---

##  Data Preprocessing
- Handled missing values in `TotalCharges`
- Converted categorical variables using one-hot encoding
- Dropped unnecessary columns like `customerID`
- Converted target variable (`Churn`) into binary format

---

##  Exploratory Data Analysis (EDA)

Key insights:
-  ~26% of customers churned (class imbalance)
-  Customers with low tenure churn more
-  Higher monthly charges increase churn probability
-  Month-to-month contracts have the highest churn
-  Lack of tech support and security services increases churn
-  Electronic check users show higher churn rates

---

##  Model Building

### Models Used:
- Logistic Regression
- Logistic Regression (with class balancing)
- Random Forest

---

##  Model Evaluation

| Model | Accuracy | Recall (Churn) |
|------|---------|----------------|
| Logistic Regression | ~79% | 52% |
| Logistic (Balanced) | ~73% | **80%**  |
| Random Forest | ~78% | 46% |

---

##  Final Model Selection

**Logistic Regression with class_weight="balanced"**

### Why?
- Higher recall for churn customers (80%)
- Better for business use-case (detecting at-risk customers)
- Simple and interpretable

---

## 💡 Business Insights

- Customers with short tenure are more likely to churn
- High monthly charges increase churn risk
- Long-term contracts reduce churn significantly
- Service quality (support/security) impacts retention
- Payment methods influence customer behavior

---

##  Business Recommendations

- Offer incentives for long-term contracts
- Improve onboarding for new customers
- Provide better customer support services
- Target high-risk customers with retention offers

---

##  Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

##  Conclusion

This project demonstrates how machine learning and data analysis can help businesses identify churn patterns and take proactive steps to improve customer retention.
