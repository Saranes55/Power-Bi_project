# Personal Finance Management Analysis

## Project Overview
The Finance Report Dashboard provides a comprehensive view of income, expenses, and spending behavior across months and categories. This interactive dashboard helps track financial performance, monitor expenses, and compare income against predefined targets to support better financial planning and control.

## Objectives
- Track total income and total expenses
- Monitor monthly expense trends
- Analyze expenses by category and sub-category
- Compare actual income vs income target
- Identify areas of high spending and cost leakage

## Project Highlights
- 798K Total Income tracked across the year
- 548K Total Expenses analyzed by category and month
- Monthly expense patterns clearly visualized
- Detailed sub-category level expense breakdown
- Interactive month-wise navigation for quick insights

## Dataset Used
- <a href="https://github.com/Saranes55/Power-Bi_project/blob/main/Personal%20Finance%20Management%20Analysis/Finance%20Dataset.xlsx">Finances_Datasets</a> (Dataset)

## Dashboard Visualization
![Screenshot (495)](https://github.com/Saranes55/Power-Bi_project/blob/main/Personal%20Finance%20Management%20Analysis/Dashboard.png)

## Key Performance Indicators (KPIs)
- Total Income: 798K
- Total Expenses: 548K
- Income vs Target: Visual progress indicator
- Expense Categories: Housing, Personal, Transportation
- Expense Sub-categories: Cleaning, Internet, Insurance, Loans, Subscriptions, etc.

## Dashboard Insights

## 1. Status by Category – Paid vs Unpaid
- Breaks down expenses by category:
  - Housing
  - Personal
  - Transportation
- Each category is split into:
  - Paid expenses
  - Unpaid expenses
- Helps identify:
  - Payment discipline
  - Pending liabilities
  - Categories with higher unpaid amounts
- Supports cash flow and dues management.

## 2. Total Income vs Income Target
- Compares actual income (798K) against a fixed target (2M).
- Clearly visualizes:
  - Progress achieved
  - Remaining income gap
- Ideal for goal tracking and performance monitoring.
- Enables quick evaluation of whether financial targets are on track.

## 3. Monthly Expense by Category
- Displays month-wise expenses across the year (Jan–Dec).
- Expenses are stacked by category:
  - Housing
  - Personal
  - Transportation
- Helps identify:
  - Monthly spending patterns
  - Seasonal expense spikes
  - Categories driving high monthly costs
- Useful for trend analysis and future planning.

## 4. Total Expenses by Sub-category
- Provides a granular breakdown of expenses into sub-categories such as:
  - Internet
  - Insurance
  - School Loans
  - TV Subscription
  - Cleaning
  - Toll
  - Registration
  - Other recurring costs
- Highlights which sub-categories consume the largest share of expenses.
- Supports cost optimization and prioritization decisions.

## Slicer (Month Selector)
- Allows users to filter data month-wise (Jan–Dec).

## DAX Formulas Used
1. **Total Income** = CALCULATE(SUM('Main Data'[Amount]), 'Main Data'[Main Type] = "Income")
2. **Total Expenses** = CALCULATE(SUM('Main Data'[Amount]), 'Main Data'[Main Type] = "Expenses")
3. **Monthly Income** = CALCULATE(SUM('Main Data'[Amount]), 'Main Data'[Main Type] = "Income")
4. **Monthly Expense** = CALCULATE(SUM('Main Data'[Amount]), 'Main Data'[Main Type] = "Expenses")
5. **Paid Bills** = CALCULATE(COUNTROWS('Main Data'), 'Main Data'[Status] = "Paid", 'Main Data'[Main Type] = "Expenses")
6. **Unpaid Bills** = CALCULATE(COUNTROWS('Main Data'), 'Main Data'[Status] = "Unpaid", 'Main Data'[Main Type] = "Expenses")
7. **Expense Target** = SUM('Income Goal'[Income Target])

## Conclusion
- This Finance Report Dashboard provides a clear view of income, expenses, and spending behavior.
- It enables effective tracking of monthly expenses and financial performance.
- Category and sub-category insights help identify cost optimization opportunities.
- Interactive visuals support informed financial decision-making.

Overall, the dashboard serves as a powerful personal and business finance monitoring tool.





















