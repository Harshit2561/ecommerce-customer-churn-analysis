# Customer Churn Prediction & Revenue Risk Dashboard

## 📌 Project Overview

This project builds a **time-aware customer churn prediction system** for an e-commerce business using transactional data.

Unlike rule-based churn analysis, this project implements:

* Time-aware feature engineering
* Supervised machine learning models
* Probability-based churn prediction
* Revenue-at-risk analysis

The final output is an **interactive Power BI dashboard** that translates ML predictions into business decisions.

---

## 🎯 Business Objectives

* Predict which customers are likely to churn
* Quantify revenue at risk from high-risk customers
* Understand churn risk distribution across customer groups
* Track overall revenue performance trends
* Enable targeted retention strategies

---

## 🧠 Project Highlights

### ✅ Time-Aware Modeling

* Features built using data before a cutoff date
* Churn defined using future 90-day purchase window
* No data leakage

### ✅ Machine Learning Models

* Logistic Regression
* Random Forest
* ROC-AUC ≈ 0.80
* Precision–Recall analysis
* Class imbalance handling

### ✅ Predictive KPIs

* Revenue at Risk (Top 25% churn probability)
* Average Churn Probability
* Risk Group Segmentation (Low / Medium / High)
* Customer distribution by churn risk

---

## 📊 Dashboard Features

* Executive KPI summary
* Revenue at Risk (Predictive)
* Revenue by Risk Group
* Customer Risk Distribution (Donut)
* Monthly Revenue Trend
* Interactive Risk Group & Date slicers

---

## 🛠 Tools & Technologies

* **Python**: Pandas, NumPy, Scikit-learn
* **Machine Learning**: Logistic Regression, Random Forest
* **Power BI**: Dashboard development
* **Jupyter Notebook**: End-to-end ML pipeline
* **GitHub**: Version control

---

## 📂 Project Structure

```
ecommerce-customer-churn-analysis/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_sales_metrics.ipynb
│   ├── 03_time_aware_churn_features.ipynb
│   ├── 04_churn_modeling.ipynb
│   ├── 05_Insights_and_Model_Interpretation.ipynb
│
├── data/
│   ├── raw/
│   └── cleaned/
│       ├── cleaned_retail.csv
│       ├── time_aware_churn_dataset.csv
│       └── model_predictions.csv
│
├── powerbi/
│   └── churn_prediction_dashboard.pbix
│
├── screenshots/
│   └── dashboard_preview.png
│
├── requirements.txt
└── README.md
```

---

## 📉 Churn Definition (Predictive Setup)

For a given cutoff date:

* Features are computed using historical data
* A customer is labeled as churned if they make **no purchase in the next 90 days**
* The model predicts churn probability for each customer

This simulates real-world deployment conditions.

---

## 📈 Model Evaluation

* ROC-AUC ≈ 0.80
* Recall optimized for churn detection
* Threshold selection using percentile logic
* Revenue impact analysis integrated into dashboard

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone <your-repository-url>
cd ecommerce-customer-churn-analysis
```

### 2️⃣ Download Dataset

Download **Online Retail II** dataset from:

* Kaggle
* UCI Machine Learning Repository

Place file in:

```
data/raw/online_retail_II.csv
```

### 3️⃣ Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

### 4️⃣ Run notebooks (in order)

1. `01_data_cleaning.ipynb`
2. `02_sales_metrics.ipynb`
3. `03_time_aware_churn_features.ipynb`
4. `04_churn_modeling.ipynb`

This will:

* Clean data
* Engineer time-aware features
* Train ML models
* Export predictions for Power BI

### 5️⃣ Open Dashboard

Open:

```
powerbi/churn_prediction_dashboard.pbix
```

Refresh data if needed.

---

## 🚀 Project Impact

This project demonstrates:

* End-to-end ML pipeline
* Time-aware supervised modeling
* Business-driven threshold tuning
* Translating ML predictions into BI insights

It positions the author for **entry-level Data Science and ML roles**.

---

## 📌 Author

**Harshit Singh**
B.Tech (CSE) – DTU

