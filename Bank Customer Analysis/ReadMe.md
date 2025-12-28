# Bank Customer Churn Analysis

## Project Overview
This project focuses on analyzing customer churn behavior using an interactive dashboard. The dashboard provides a consolidated view of customer activity, churn trends, demographic insights, and credit profile analysis to help businesses understand why customers exit and how retention can be improved.

## Objectives
- Analyze overall customer churn and retention
- Compare active vs inactive members
- Identify churn patterns by month, gender, and credit type
- Enable data-driven decisions to improve customer retention strategies

## Project Highlights
- 10K total customers analyzed in a single dashboard
- Clear split between active (5,151) and inactive (4,849) members
- 2,037 exited customers with churn trends tracked over time
- Credit card ownership and credit score impact on churn
- Interactive slicers for dynamic analysis

## Dataset Used
- <a href="https://github.com/Saranes55/Power-Bi_project/blob/main/Bank%20Customer%20Analysis/Bank_Churn.csv">Bank_Churn</a> (Dataset)
- <a href="https://github.com/Saranes55/Power-Bi_project/blob/main/Bank%20Customer%20Analysis/CustomerInfo.csv">Customer_Info</a> (Dataset)

## Dashboard Visualization
![Screenshot (495)](https://github.com/Saranes55/Power-Bi_project/blob/main/Bank%20Customer%20Analysis/Dashboard.png)

## Key Performance Indicators (KPIs)
- Total Customers: 10,000
- Active Members: 5,151
- Inactive Members: 4,849
- Credit Card Holders: 7,055
- Exited Customers: 2,037
- Retained Customers: 7,963

## Dashboard Insights
## 1. Total Customers by Month
- Displays monthly distribution of active and inactive members
- Highlights seasonal fluctuations in customer engagement

## 2. Exited Customers by Gender
- Shows churn split between Male and Female customers
- Helps identify demographic-based churn patterns

## 3. Exited Customers by Month
- Tracks monthly churn trend
- Identifies peak churn periods and declining exit trends

## 4. Exited Customers by Credit Type
- Compares churn across Very Good, Excellent, Fair, Good, and Poor credit categories
- Reveals higher churn concentration among higher credit tiers

## Slicers & Interactivity
The dashboard includes interactive slicers to enhance user-driven analysis:
- Year
- Month
- Geography Location
- Active Member Status
- Gender Category (Male / Female)

## DAX Formulas Used
1. Total customer   = COUNT(CustomerInfo[CustomerId])
2. Exited customers = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[Exited]=1))
3. Retain customers = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[Exited]=0))
4. Active member    = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[IsActiveMember]=1))
5. Inactive member  = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[IsActiveMember]=0))
6. Credit card holders = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[HasCrCard]=1))
7. Non credit card holders = CALCULATE(COUNT(Bank_Churn[IsActiveMember]),KEEPFILTERS(Bank_Churn[HasCrCard]=0))

## Conclusion
- Customer churn is influenced by time, customer activity, gender, and credit profile.
- The dashboard enables quick identification of high-risk churn segments.
- Interactive filters support deeper exploration across demographics and behavior.
- Insights from this analysis can help improve retention strategies and customer lifetime value.

Overall, this dashboard delivers a clear, actionable view of churn drivers for decision-makers.






















