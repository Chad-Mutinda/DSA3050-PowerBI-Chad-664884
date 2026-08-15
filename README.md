# DSA3050-PowerBI-Chad-664884

## Project Overview

### Dataset
- Source: Kaggle (hamza0027)
- File:real_world_sales_dataset_5000.csv
- Rows: 5,000
- Columns: 16

### Business Problem
To analyze retail sales performance across countries, categories, and channels to identify growth opportunities and profitability patterns.

### Power Query Transformations
1. Data type corrections
2. Removed duplicate records
3. Trimmed text columns
4. Replaced null values with 0
5. Created Year column from Date
6. Created Month Name from Date
7. Created Quarter from Date
8. Created Revenue column (Quantity × Unit Price)
9. Created Profit Margin column
    <img width="330" height="744" alt="PHOTO-2026-08-15-03-11-02 5" src="https://github.com/user-attachments/assets/57601265-1bec-4897-a937-7ebb53b87b2b" />


### Data Model
Star schema with:
- DimDate
- DimProduct
- DimCustomer
- DimChannel
- FactSales

  <img width="1058" height="741" alt="PHOTO-2026-08-15-03-11-02 6" src="https://github.com/user-attachments/assets/a85ee2ab-b4ea-4864-9c94-e2c10454d2d6" />


### DAX Measures
1. Total Revenue
2. Total Profit
3. Total Orders
4. Avg Revenue per Order
5. Profit Margin %
6. Discount Impact
7. Customer Count
8. Revenue Rank by Category
9. YoY Revenue Growth
10. Monthly Revenue
11. High-Value Customers
12. Profit Status
13. Revenue per Category Performance

 <img width="341" height="586" alt="PHOTO-2026-08-15-03-11-02 2" src="https://github.com/user-attachments/assets/83e6fdc2-6c42-4b3f-bb34-ead60e7d8f24" />


### Dashboard Pages
1. **Executive Overview**: KPI cards, revenue trend, category and country performance

  <img width="1396" height="810" alt="PHOTO-2026-08-15-03-11-02 7" src="https://github.com/user-attachments/assets/7ac8e321-92af-4c78-bc17-9dc521a75d4e" />
 
2. **Product & Customer Analysis**: Product matrix, customer age analysis, country scatter plot

  <img width="1384" height="809" alt="PHOTO-2026-08-15-03-11-02 8" src="https://github.com/user-attachments/assets/cd9511a5-cfa9-49b2-98cc-4374ba927750" />
 
3. **Diagnostic Analysis**: Discount impact, profit categorization, decomposition tree

  <img width="1361" height="812" alt="PHOTO-2026-08-15-03-11-02" src="https://github.com/user-attachments/assets/d91edfa3-8b68-46ae-8946-f79ec1272fde" />
 

### Key Insights
1. High-Discount Products Show Lower Profit Margins.
-My analysis revealed a clear negative correlation between discount rates and profit margins. Products with discount rates exceeding 15% show significantly lower profit margins, with some categories generating losses on discounted items.   

Business Recommendation;
Restructure discount strategy: Offer lower discounts on high-margin products.
Implement tiered discounts based on product profitability.
Consider removing discounts entirely from already-low-margin items.


2.Top 10% of Customers Drive 45% of Revenue.
Customer concentration reveals that the top 10% of customers generate 45% of total revenue, highlighting both a strength and a vulnerability.
Why This Matters;
-Business is highly dependent on a small customer base.
-Losing top customers would significantly impact revenue.
-The bottom segment shows potential for upselling.

Business Recommendation;
-Implement loyalty program for top customers.
-Create targeted campaigns to move middle segment customers into top tier.
-Use personalized offers to retain high-value customers.


3.Electronics Category Dominates Revenue Performance.
-The Electronics category generates 42% of total revenue but only 35% of total profits, indicating lower per-unit profitability compared to other categories.
Why This Matters;
-Heavy reliance on Electronics creates vulnerability.
-Clothing has higher margins but lower volume.
