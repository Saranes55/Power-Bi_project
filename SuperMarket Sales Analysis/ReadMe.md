# Supermarket-data-analysis (Interactive Dashboard creation using PowerBI)

## Objective

The main objective of this project is to analyze the supermarket’s sales performance across different product lines, customer segments, payment methods, and branches. This analysis helps to understand customer behavior, identify sales trends, and support better decision-making for marketing, operations, and inventory management.

## Dataset used
- <a href="https://github.com/Saranes55/Power-Bi_project/blob/main/SuperMarket%20Sales%20Analysis/supermarket_sales%20data.csv">Supermarket_Sales</a> (Dataset)

## Dashboard Visualization
![Screenshot (495)](https://github.com/Saranes55/Power-Bi_project/blob/main/SuperMarket%20Sales%20Analysis/Dashboard.png)


## Key Performance Indicators (KPIs)

-	Total Sales: ₹322.97K
-	Total Gross Income: ₹15.38K
-	Total Products Sold: 5,510 units
-	Time Period: Jan 2019 – Mar 2019
  
## Dashboard Insights

## 1. Product Performance
-	Top Selling Product Line: Electronic Accessories (971 units)
-	Highest Rated Product Line: Food & Beverages (7.11)
-	Health & Beauty recorded the lowest quantity sold, indicating growth potential.
  
## 2. City-Level Analysis
-	Highest Sales & Profit City: Naypyitaw
-	Yangon and Mandalay show consistent and balanced performance.
  
## 3. Customer Segmentation
-	Member Customers: 50.85% of total sales
-	Normal Customers: 49.15% of total sales

➡️ Loyalty membership programs positively impact revenue.
 	
## 4. Gender Insights
-	Female Customers: 51.98% of revenue
-	Male Customers: 48.02% of revenue

➡️ Female customers contribute slightly higher sales.
 	
## 5. Payment Method Analysis
-	Highest Average Quantity per Transaction: Credit Card
-	Followed closely by Cash and E-wallet payments.
  
## DAX Formulas Used
1. **Profit** = SUM(supermarket_sales[Total]) - SUM(supermarket_sales[cogs])
2. **Total sales** = SUM('supermarket_sales'[Total])

## Conclusion

- The supermarket shows stable and healthy sales performance with strong total sales, gross income, and product volume.
- Electronic Accessories and Food & Beverages are the top-performing product lines in terms of quantity, revenue, and customer ratings.
- Naypyitaw is the highest sales and profit–generating city, making it a key focus area for business expansion.
- Member customers contribute slightly more revenue than normal customers, highlighting the success of loyalty programs.
- Female customers generate marginally higher sales compared to male customers.
- Credit card payments result in the highest average quantity per transaction.
- Sales and income peak during afternoon to evening hours, indicating the best time for promotions and offers.
  
Overall, the dashboard provides actionable insights to improve marketing strategy, inventory planning, and customer engagement.
