# 🧠 Customer Segmentation Analytics

**End-to-End Machine Learning + Business Intelligence Project**

---

## 📌 Project Overview

This project delivers an **end-to-end customer segmentation solution** using **unsupervised machine learning (K-Means)** and **Power BI** to enable **data-driven marketing strategies** for a retail mall.

The objective is to **increase revenue without increasing footfall** by identifying **distinct customer segments** based on **income and spending behavior** and translating those segments into **actionable business recommendations**.

This project demonstrates the ability to move beyond descriptive analytics and apply **advanced analytical thinking**, **machine learning**, and **business strategy alignment**.

---

## 🏬 Business Problem Statement

Retail businesses often treat all customers uniformly, leading to:

* Inefficient discounting
* Poor marketing ROI
* Missed revenue opportunities

**Problem:**
How can a retail mall increase revenue **without increasing customer footfall**?

**Key business questions addressed:**

* Are all customers equally valuable?
* Which customers should receive discounts vs premium treatment?
* Where should marketing investments be prioritized for maximum ROI?

---

## 🎯 Analytical Objective

To **segment customers using unsupervised machine learning** based on **income and spending behavior**, enabling:

* Targeted promotions
* Personalized engagement strategies
* Optimal allocation of marketing resources

---

## 📊 Dataset Information

* **Dataset:** Mall Customers Dataset
* **Source:** Kaggle
* **Records:** 200 customers
* **Features Used for Clustering:**

  * Age
  * Annual Income (k$)
  * Spending Score (1–100)

The dataset contains **no missing values**, allowing direct application of clustering algorithms without imputation bias.

---

## 🛠 Tools & Technologies

**Programming & ML**

* Python
* pandas, numpy
* scikit-learn (StandardScaler, K-Means)

**Visualization & BI**

* matplotlib, seaborn
* Power BI

**Data Handling**

* CSV / Excel exports
* GitHub for version control

---

## 🔍 Methodology

1. **Business Problem Framing**
   Defined revenue optimization goals under fixed footfall constraints.

2. **Manual Data Audit**
   Verified data quality, value ranges, and feature relevance before modeling.

3. **Data Cleaning & Feature Selection**

   * Removed identifier columns (CustomerID)
   * Retained behaviorally meaningful variables
   * Encoded demographics for post-cluster interpretation

4. **Feature Standardization**

   * Applied `StandardScaler` to ensure fair distance computation
   * Prevented income dominance in distance-based clustering

5. **K-Means Clustering**

   * Applied unsupervised learning to discover latent customer groups
   * Used the **Elbow Method** to select optimal number of clusters (K = 5)

6. **Cluster Interpretation**

   * Inverse-transformed centroids to original business units
   * Profiled each segment using age, income, and spending patterns

7. **Power BI Dashboard**

   * Integrated ML outputs into BI
   * Built segment-wise KPI visuals for decision-making

---

## 📈 Key Metrics & Results

* **Number of Customer Segments Identified:** 5
* **High-Value Customers (Premium Loyalists):** ~20% of customers
* **Low-Income High-Spending Customers:** ~13% (deal-driven behavior)
* **High-Income Low-Spending Customers:** ~15% (highest growth opportunity)

This distribution reflects the **Pareto Principle**, where a small subset of customers drives disproportionate revenue.

---

## 🧩 Customer Segments Identified

| Segment Name              | Income | Spending | Strategic Value         |
| ------------------------- | ------ | -------- | ----------------------- |
| 🟢 Premium Loyalists      | High   | High     | Core revenue drivers    |
| 🟡 Untapped Potential     | High   | Low      | Highest ROI opportunity |
| 🔴 Deal-Driven Shoppers   | Low    | High     | Promotion-sensitive     |
| ⚪ Average Customers       | Mid    | Mid      | Upsell potential        |
| 🔵 Low Priority Customers | Low    | Low      | Minimal ROI             |

---

## 💡 Business Insights

* **Customer value is highly uneven** — customer volume does not equal revenue contribution.
* **Premium Loyalists (~20%)** drive a disproportionate share of revenue (Pareto effect).
* **Untapped Potential customers** have the highest income but lowest spending, representing the **largest revenue growth opportunity**.
* Blanket discounting reduces margins and should be avoided.
* Targeted strategies outperform one-size-fits-all marketing.

---

## 📌 Business Recommendations

### 🎯 Discount Strategy

* Apply discounts **only** to **Deal-Driven Shoppers**
* Use coupons, bundles, and loyalty rewards

### 👑 Premium Strategy

* Offer exclusivity to **Premium Loyalists**
* Focus on retention via VIP access and early launches

### 🚀 Growth Strategy

* Activate **Untapped Potential** customers through personalized engagement
* Avoid discounts; focus on relevance and premium positioning

### 🔻 Cost Optimization

* Deprioritize **Low Priority Customers**
* Minimize marketing spend with low expected ROI

---

## 📊 Power BI Dashboard

The Power BI dashboard visualizes:

* Segment-wise customer distribution
* Average income by segment
* Average spending by segment
* Demographic (age) composition per segment

This enables **executive-level decision-making** using ML-driven insights.

---

## 📂 Repository Structure

```
customer-segmentation-analytics/
│
├── data/
│   ├── raw/
│   │   └── Mall_Customers.csv
│   └── processed/
│       └── customer_segmentation_output.csv
│
├── notebooks/
│   └── customer_segmentation_analysis.ipynb
│
├── dashboards/
│   └── customer_segmentation_powerbi.pbix
│
├── images/
│   └── (EDA & dashboard visuals)
│
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run This Project

1. Clone the repository

   ```bash
   git clone https://github.com/your-username/customer-segmentation-analytics.git
   ```
2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook

   ```bash
   jupyter notebook notebooks/customer_segmentation_analysis.ipynb
   ```
4. Load the processed CSV into **Power BI** to explore the dashboard

---
