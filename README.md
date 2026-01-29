# Customer Segmentation Using RFM Analysis

**Problem Statement :-**

•Raw transaction data does not directly tell a business:
•Who their best customers are
•Who is about to churn
•Where marketing money should be spent
This project solves that using RFM-based customer segmentation.

**Dataset :-**

**E-commerce transactional dataset containing :-**
•Invoice details
•Product information
•Quantity and price
•Customer IDs
•Transaction timestamps

**Project Workflow :-**

**1. Data Cleaning & Preprocessing :-**

Performed using Pandas:
•Removed records with missing CustomerID
•Detected and removed duplicate rows
•Isolated cancelled transactions (negative quantity)
•Cleaned inconsistent product descriptions
•Ensured correct data types for dates and numeric fields

**2. Exploratory Data Analysis (EDA) :-**

Analyzed:
•Revenue trends over months
•Sales behavior by day of the week
•Customer purchasing patterns
•Distribution of order frequency

**Libraries used:**

Matplotlib, Seaborn

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

***5. Customer Segmentation Logic:-**

| Segment    | Characteristics                          | Business Action                  |
|-----------|-------------------------------------------|----------------------------------|
| High Value| Recent, frequent, high spenders           | Retention & premium offers       |
| Loyal     | Consistent repeat buyers                  | Loyalty rewards & upselling      |
| At Risk   | Previously active, now inactive           | Re-engagement campaigns          |
| Dormant   | Low activity and low spending             | Win-back or low-cost targeting   |


**Business Insights :-**

This model helps businesses:
•Identify top customers for retention
•Detect potential churn early
•Personalize marketing strategies
•Optimize customer acquisition cost

**Tech Stack :-**

•Python
•Pandas
•NumPy
•Matplotlib
•Seaborn
•Jupyter Notebook
•Power BI (for dashboard visualization)

**Files in Repository :-**

•Ecommerce_Data_Analysis.ipynb → Full EDA + RFM modeling
•Dashboard visuals → Customer segmentation insights
•Raw datasets
•Customer Segmentation Using RFM Analysis in E-Commerce.pptx → Project presentation covering methodology, insights, segments, and business recommendations
