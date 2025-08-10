📌 Project Overview
This project applies RFM Analysis to segment customers based on their purchasing behavior using the Online Retail Dataset.
RFM stands for:

Recency (R): How recently a customer made a purchase.
Frequency (F): How often they make purchases.
Monetary (M): How much money they spend. The goal is to group customers into meaningful segments (e.g., Loyal, Regular, At Risk) to enable targeted marketing strategies.
📂 Dataset
Source: Chen, D. (2015). Online Retail [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33.
Contains transactional data from a UK-based online retailer between 2010 and 2011.
Key columns used:
InvoiceNo → Transaction ID
StockCode → Product code
Description → Product description
Quantity → Number of items purchased
InvoiceDate → Date of purchase
UnitPrice → Price per unit
CustomerID → Unique customer identifier
Country → Customer's country
🛠️ Tools & Libraries
Python
Pandas
Matplotlib
Seaborn
Datetime
📊 Project Workflow
Data Loading & Cleaning
Removed null values
Filtered out negative quantities (returns) and zero-priced items
Feature Engineering
Created TotalSum = Quantity × UnitPrice
RFM Calculation
Recency: Days since last purchase
Frequency: Number of unique invoices
Monetary: Total spending
Scoring & Segmentation
Assigned R, F, and M scores (1–5)
Created combined RFM_Segment and RFM_Score
Mapped customers into Loyal, Regular, and At Risk groups
Visualization
Bar plots of customer segments
RFM heatmap (Recency × Frequency)
📈 Example Visualizations
Segment Distribution
RFM Heatmap
💡 Marketing Ideas
Loyal Customers: Offer exclusive discounts and early access to sales.
Regular Customers: Encourage upselling/cross-selling.
At Risk Customers: Send win-back offers or re-engagement emails.
📜 How to Run
Open the notebook in Jupyter or VSCode.
Run the book step by step
