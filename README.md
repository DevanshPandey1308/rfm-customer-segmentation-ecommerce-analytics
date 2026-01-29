# Customer Segmentation Using RFM Analysis

**Problem Statement**

| Challenge | Description |
|-----------|-------------|
| Customer visibility gap | Raw transaction data does not clearly show who the best customers are |
| Churn detection | Businesses struggle to identify customers who are about to churn |
| Marketing allocation | Difficult to decide where marketing budget should be spent |

This project addresses these problems using RFM-based customer segmentation.

---

**Dataset**

| Type | Details |
|------|--------|
| Data Source | E-commerce transactional dataset |
| Contents | Invoice details, product information, quantity, price, customer IDs, transaction timestamps |

---

**Project Workflow**

**1. Data Cleaning & Preprocessing**

| Task | Purpose |
|------|--------|
| Remove missing Customer IDs | Ensure valid customer-level analysis |
| Remove duplicate rows | Prevent data inflation |
| Isolate cancelled transactions | Avoid revenue distortion |
| Clean product descriptions | Improve data consistency |
| Correct data types | Enable accurate analysis |

---

**2. Exploratory Data Analysis (EDA)**

| Analysis | Insight Goal |
|----------|--------------|
| Revenue trends over months | Understand sales growth patterns |
| Sales by day of week | Identify behavioral timing patterns |
| Customer purchasing behavior | Detect buying trends |
| Order frequency distribution | Understand repeat vs one-time buyers |

**Libraries Used:** Matplotlib, Seaborn


**3. RFM Feature Engineering:-**

| Metric     | Definition                   | Business Meaning                |
|-----------|------------------------------|---------------------------------|
| Recency   | Days since last purchase     | How recently a customer bought  |
| Frequency | Number of unique invoices    | How often the customer buys     |
| Monetary  | Total revenue generated      | How much the customer spends    |

**4. RFM Scoring:-**

| Rule       | Scoring Logic                         |
|-----------|----------------------------------------|
| Recency   | Lower recency → Higher score           |
| Frequency | Higher frequency → Higher score        |
| Monetary  | Higher spending → Higher score         |
| Method    | Quantile-based scoring (1–5 scale)     |

**5. Customer Segmentation Logic:-**

| Segment    | Characteristics                          | Business Action                  |
|-----------|-------------------------------------------|----------------------------------|
| High Value| Recent, frequent, high spenders           | Retention & premium offers       |
| Loyal     | Consistent repeat buyers                  | Loyalty rewards & upselling      |
| At Risk   | Previously active, now inactive           | Re-engagement campaigns          |
| Dormant   | Low activity and low spending             | Win-back or low-cost targeting   |

---

**Business Insights**

| Capability | Impact |
|------------|--------|
| Identify top customers | Focus retention efforts on high-value users |
| Detect churn risk | Enable early re-engagement strategies |
| Personalize marketing | Target segments based on value and behavior |
| Optimize acquisition cost | Avoid spending on low-value customers |

---

**Tech Stack**

| Category | Tools |
|----------|------|
| Programming | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Power BI |
| Environment | Jupyter Notebook |
| BI Tool | Power BI |

---

**Files in Repository**

| File | Description |
|------|-------------|
| Ecommerce_Data_Analysis.ipynb | Full data cleaning, EDA, RFM modeling, and segmentation |
| online_retail_data.csv | Transactional dataset used for analysis |
| Customer Segmentation Using RFM Analysis in E-Commerce.pptx | Project presentation covering methodology, insights, segments, and business recommendations |
| Dashboard Visuals | Power BI dashboard screenshots showing segment insights |

