# E-commerce Customer Churn & Sales Analytics Dashboard

## 📌 Project Overview
This project analyzes e-commerce sales performance and customer churn using **RFM (Recency, Frequency, Monetary) segmentation**.  
The goal is to identify high-value customers, understand revenue trends, and detect customer segments at risk of churn using data analysis and business intelligence techniques.

The final output is an **interactive Power BI dashboard** that presents actionable insights for business decision-making.

---

## 🧠 Business Questions Answered
- How is overall sales performance trending over time?
- Which customer segments generate the most revenue?
- Which customer segments are most likely to churn?
- How does customer behavior differ across segments?

---

## 📊 Key Features
- Sales KPIs: Total Revenue, Orders, Customers
- Monthly Revenue Trend Analysis
- RFM-based Customer Segmentation
- Churn Identification using inactivity logic
- Revenue contribution by customer segment
- Churn rate comparison across segments
- Interactive slicers for country and customer segment

---

## 🛠 Tools & Technologies
- **Python**: Pandas, NumPy, Matplotlib (data cleaning, analysis & visualization)
- **Power BI**: Dashboard development
- **Jupyter Notebook**: Analysis workflow
- **GitHub**: Version control & project sharing

---

## 📂 Project Structure
ecommerce-customer-churn-analysis/
│
├── notebooks/
│ ├── 01_data_cleaning.ipynb
│ ├── 02_sales_metrics.ipynb
│ ├── 03_rfm_churn_analysis.ipynb
│
├── powerbi/
│ └── dashboard.pbix
│
├── screenshots/
│ ├── dashboard_overview.png
│ ├── revenue_by_segment.png
│ ├── churn_by_segment.png
│
├── requirements.txt
└── README.md


---

## 📈 Dashboard Preview
Screenshots of the Power BI dashboard are available in the `screenshots/` folder.

The dashboard includes:
- Executive KPI summary
- Monthly revenue trend
- Revenue by customer segment
- Churn rate by customer segment
- Interactive filters for country and segment

---

## 📉 Churn Definition
A customer is classified as **churned** if they have not made a purchase in the **last 90 days** relative to the dataset’s end date.

This rule-based approach reflects common retail churn analysis practices.

---

## 📊 RFM Segmentation Logic
Customers are segmented using RFM scores:
- **Recency**: Days since last purchase
- **Frequency**: Number of unique orders
- **Monetary**: Total spend

Segments include:
- Champions
- Loyal
- At Risk
- Others

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository
```bash
git clone <your-repository-url>
cd ecommerce-customer-churn-analysis
```

### 2️⃣ Download the dataset
Download the **Online Retail II** dataset from one of the following sources:
- **Kaggle**: https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset
- **UCI Machine Learning Repository**

### 3️⃣ Place the dataset
After downloading, place the dataset file in the following local directory (not tracked by Git):
```
data/raw/online_retail_II.csv
```
⚠️ **Note**: The dataset is intentionally not included in this repository due to size considerations.

### 4️⃣ Install required Python packages
Ensure Python is installed, then run:
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 5️⃣ Run the analysis notebooks
Start Jupyter Notebook:
```bash
jupyter notebook
```

Run the notebooks in the following order from the `notebooks/` folder:
1. `01_data_cleaning.ipynb`
2. `02_sales_metrics.ipynb`
3. `03_rfm_churn_analysis.ipynb`

These notebooks will:
- Clean the raw data
- Generate sales KPIs
- Perform RFM segmentation
- Identify churned customers
- Prepare BI-ready datasets

### 6️⃣ Open the Power BI dashboard
1. Open **Power BI Desktop**
2. Load the dashboard file:
```
powerbi/ecommerce_customer_churn_dashboard.pbix
```
---

## 📌 Author
**Harshit Singh**  
B.Tech (CSE), DTU



