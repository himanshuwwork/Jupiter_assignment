# Jupiter_assignment
# 📊 Predicting Credit Score Movement Using Machine Learning

## 🎯 Objective

To simulate a realistic dataset and build a machine learning model that predicts whether a customer's credit score will **increase**, **decrease**, or **remain stable** in the next 3 months. This enables financial institutions to take proactive decisions to manage credit risk and growth opportunities.

---

## 📋 Project Summary

### 1. Synthetic Data Generation
- Created a dataset of **27,000 customer-month records**
- Based on real-world financial logic:
  - **High DPD + High Utilization** → Score likely to decrease  
  - **Good repayment + Low EMI burden** → Score likely to increase

### 2. Exploratory Data Analysis (EDA)
- Class balance visualization
- Statistical summary of key features (DPD, utilization, etc.)
- Insights into target-wise behavior

### 3. Data Preprocessing
- Encoded categorical features
- Scaled numerical values
- Ensured model compatibility for SHAP/XGBoost

### 4. Model Building
- Trained 4 models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
- Evaluated using:
  - Accuracy
  - F1-Score
  - Precision
  - Recall

### 5. Feature Importance
- Identified key drivers using feature importance & SHAP:
  - `dpd_last_3_months`
  - `repayment_history_score`
  - `credit_utilization_ratio`

### 6. Business Insights
| Movement  | Suggested Action                         |
|-----------|------------------------------------------|
| Decrease  | Early alerts, restrict disbursal         |
| Increase  | Upsell offers, credit limit boost        |
| Stable    | Routine monitoring                       |

### 7. Final Conclusion
- **XGBoost** performed best in classification tasks
- Demonstrated domain-driven ML can help credit teams make informed decisions

---

## 📁 Files Included

| File Name                                 | Description                                |
|-------------------------------------------|--------------------------------------------|
| `synthetic_credit_score_data_generation.csv` | Simulated dataset (27,000 rows)           |
| `credit_score_prediction_notebook.ipynb`     | Full ML pipeline + EDA + insights         |
| `README.md`                                  | Project summary (this file)               |

---

## 🔮 Future Improvements

- Apply to real customer datasets from banks/NBFCs
- Incorporate time-series data to predict score change magnitude
- Integrate into a credit monitoring dashboard

---

## 👨‍💻 Author

**Himanshu**  
M.Tech, IIT Bombay
