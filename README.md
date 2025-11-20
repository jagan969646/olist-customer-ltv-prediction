# Customer Lifetime Value Prediction – Olist E-Commerce Dataset

End-to-end data science project that predicts **Customer Lifetime Value (LTV)** for customers of the Olist Brazilian e-commerce platform and segments them into **Low / Medium / High value** buckets for targeted marketing.

---

## 🎯 Objective

- Build a **customer-level dataset** from raw Olist transaction data.
- Engineer **RFM-style features** (Recency, Frequency, Monetary, Tenure, AOV, Order Rate).
- Train and compare **regression models** to predict LTV.
- Create an **LTV-based customer segmentation** for business use cases.

---

## 🧰 Tech Stack

- **Language:** Python  
- **Libraries:**  
  - Data: `pandas`, `numpy`  
  - Modeling: `scikit-learn`, `xgboost`, `joblib`  
  - Visualization: `matplotlib`, `seaborn`  

---

## 📂 Project Structure

```text
.
├─ data_raw/                         # raw Olist CSVs (not committed)
│   ├─ olist_customers_dataset.csv
│   ├─ olist_orders_dataset.csv
│   ├─ olist_order_items_dataset.csv
│   └─ olist_order_payments_dataset.csv
├─ data_processed/
│   └─ olist_customer_ltv_predictions.csv   # final customer-level table with LTV & segment
├─ models/
│   ├─ olist_rf_ltv_model.joblib            # Random Forest model
│   └─ olist_xgb_ltv_model.joblib           # XGBoost model
├─ notebooks/                               # (optional) EDA / experiments
├─ src/
│   └─ train_ltv_model.py                   # main training & prediction pipeline
├─ README.md
├─ requirements.txt
└─ .gitignore

