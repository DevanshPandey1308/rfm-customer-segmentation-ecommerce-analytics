**Customer Segmentation Using RFM Analysis**

**Problem Statement:-*
•Raw transaction data does not directly tell a business:
•Who their best customers are
•Who is about to churn
•Where marketing money should be spent
This project solves that using RFM-based customer segmentation.

**Dataset**
E-commerce transactional dataset containing:
•Invoice details
•Product information
•Quantity and price
•Customer IDs
•Transaction timestamps

**Project Workflow**

**1. Data Cleaning & Preprocessing**
Performed using Pandas:
•Removed records with missing CustomerID
•Detected and removed duplicate rows
•Isolated cancelled transactions (negative quantity)
•Cleaned inconsistent product descriptions
•Ensured correct data types for dates and numeric fields

**2. Exploratory Data Analysis (EDA)**
Analyzed:
•Revenue trends over months
•Sales behavior by day of the week
•Customer purchasing patterns
•Distribution of order frequency

**Libraries used:**
Matplotlib, Seaborn

**3. RFM Feature Engineering**
For each customer:
Metric 	--   Definition
Recency	     Days since last purchase
Frequency    Number of unique invoices
Monetary	   Total revenue generated

**4. RFM Scoring**
Used quantile-based scoring (1–5 scale):
•Low Recency → Higher score
•High Frequency → Higher score
•High Monetary → Higher score
Converted R, F, M into customer segments.

5. Customer Segmentation Logic
Segment  --  	Meaning
High Value	  Most recent, frequent, and high-spending customers
Loyal	        Consistent repeat buyers
At Risk	      Previously active, now inactive
Dormant	      Low activity and low revenue

**Business Insights**
This model helps businesses:
•Identify top customers for retention
•Detect potential churn early
•Personalize marketing strategies
•Optimize customer acquisition cost

**Tech Stack**
•Python
•Pandas
•NumPy
•Matplotlib
•Seaborn
•Jupyter Notebook
•Power BI (for dashboard visualization)

**Files in Repository**
•Ecommerce_Data_Analysis.ipynb → Full EDA + RFM modeling
•Dashboard visuals → Customer segmentation insights
•Raw datasets
•Customer Segmentation Using RFM Analysis in E-Commerce.pptx → Project presentation covering methodology, insights, segments, and business recommendations
