# 🛍️ Retail Transaction Data Analysis Report (2009–2011)

## 📌 Overview

This project dives deep into retail transaction data spanning two fiscal years (2009–2011) to uncover hidden patterns in customer behavior, seasonal sales trends, product performance, and market opportunities. Using Python (pandas, matplotlib, seaborn, sklearn), we combined exploratory data analysis and customer clustering to offer strategic business recommendations.

---

## 🎯 Business Objectives

- Track sales performance across two consecutive years.
- Understand seasonal patterns and quarterly dynamics.
- Identify best-selling and underperforming products.
- Segment customers for targeted marketing.
- Analyze regional sales to highlight growth markets.
- Leverage clustering techniques to uncover high-impact customer groups.

---

## 📂 Data Summary

- **Source:** Retail transaction dataset (Excel, 2 sheets)
- **Period Covered:** 2009–2010 and 2010–2011
- **Size:** ~793,000 transactions
- **Structure:** Invoice No., Product ID, Customer ID, Quantity, Price, Invoice Date, Country

---

## 🔧 Data Processing & Feature Engineering

- Combined both time periods into one DataFrame.
- Cleaned missing values and dropped entries without customer IDs.
- Filtered out negative/return transactions.
- Created new features:  
  - `Revenue = Quantity × Price`  
  - Time dimensions: Year, Month, Quarter, YearMonth  
  - Flags for repeat and top-tier customers

---

## 📊 Exploratory Data Analysis (EDA)

### 📈 Sales Trends
- **Peak month:** November (holiday shopping)
- **Lowest month:** February and July (post-holiday slumps)
- **Biggest growth:** 1263% increase in sales from 2009 to 2010
- **Q4** always outperformed other quarters.

### 👥 Customer Behavior
- Top 25% of customers brought in most revenue.
- 80% were repeat buyers, yet most were low- to mid-tier in spend.
- Key opportunity: Upsell mid-tier buyers.

### 📦 Product Performance
- Products like StockCode `84077` dominated sales.
- Several items had only 1 unit sold (need review or removal).
- Action: Bundle or discontinue underperformers, focus marketing on top-sellers.

### 🌍 Regional Sales
- **UK:** 89% of total sales — main market.
- **France, Germany, Netherlands:** Moderate sales — room to grow.
- Action: Localized campaigns in mid-tier markets.

---

## 🤖 Clustering Analysis

### A. **K-Means Clustering**
- 3 segments:
  - Low-value, high-frequency buyers (target with loyalty discounts)
  - Occasional high spenders (push loyalty perks)
  - High-frequency, high-value (retain at all costs)

### B. **DBSCAN**
- Identified outliers (big spenders with few transactions).
- Noise: Low-engagement customers — trigger reactivation campaigns.

### C. **Hierarchical Clustering**
- Reinforced 3 major customer types.
- Dendrograms helped visualize nested clusters.

---

## 📌 Key Business Recommendations

1. **Boost Q1 Performance**
   - Seasonal offers and Q1-specific promotions.
   - Optimize stock planning for slow months.

2. **Retain High-Value Buyers**
   - Loyalty programs & personalized email campaigns.

3. **Target Mid-Tier Regions**
   - France, Germany, Netherlands need tailored strategies.

4. **Optimize Product Portfolio**
   - Focus on bestsellers, investigate low-performing SKUs.

5. **Use Clusters for Campaigns**
   - Segment-specific messaging = higher ROI.

6. **Real-Time Monitoring**
   - Set up live KPI dashboards to track churn, sales, and CLV.

---

## 🧠 Conclusion

By combining robust EDA with advanced clustering techniques, this analysis uncovered clear patterns and customer insights that could directly inform smarter marketing, inventory control, and sales strategies.

The result? A data-backed roadmap to sustainable retail growth.

---

## 🧑‍💻 Author

**David Afolayan**  
Data Analyst | Operations Tech Lead  

---

## 📝 Tech Stack

- Python (pandas, matplotlib, seaborn, scikit-learn)
- Jupyter Notebook
- Excel
- GitHub
