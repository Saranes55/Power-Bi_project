# Employees Attrition Analysis

## Objective
- To analyze employee workforce data and identify attrition patterns across age groups, gender, departments, and education fields.
- To measure overall employee satisfaction and workforce stability.
- To provide actionable insights that help HR teams improve employee retention and engagement strategies.
- To support data-driven HR decision-making using interactive visual analytics.

## Project Highlights
Interactive HR dashboard with key workforce KPIs. Detailed attrition analysis by age, gender, department, and education
Clear comparison of current vs. exited employees. Visual identification of high-risk attrition segments.
Business-ready dashboard suitable for executive and HR review Clean. Structured layout with filters for department, gender, and age group

## Dataset Used
- <a href="https://github.com/Saranes55/Power-Bi_project/blob/main/Attrition%20Analysis/HR%20Data.xlsx">HR_Data</a> (Dataset)

## Dashboard Visualization
![Screenshot (495)](https://github.com/Saranes55/Power-Bi_project/blob/main/Attrition%20Analysis/Dashboard.png)

## Key Performance Indicators (KPIs)
- Total Employees: 1,470
- Current Employees: 1,233
- Employees Quit: 237
- Attrition Rate: 16%
- Average Employee Age: 36.92 years
- Average Satisfaction Score: 2.73

## Dashboard Insights

## 1. Workforce Overview Cards
- Displays Total Employees, Average Age, Attrition Rate, Current Employees, and Employees Quit
- Provides an instant snapshot of workforce health

## 2. Attrition by Age Group & Gender
- Shows employee attrition distribution across different age bands
- Highlights gender-based differences in attrition
- Highest attrition observed in 25–34 and 35–44 age groups

## 3. Employee Quit by Education Field
- Compares employee exits across education backgrounds
- Life Sciences and Medical fields show higher quit counts
- Helps identify education groups needing targeted retention efforts

## 4. Attrition by Department
- Visualizes attrition share across R&D, Sales, and HR
- R&D accounts for the largest portion of employee exits
- Supports department-specific workforce planning

## 5. Average Satisfaction Score
- Represents overall employee satisfaction level
- Indicates moderate satisfaction, suggesting scope for engagement improvement

## 6. Employees Count by Department & Attrition Status 
- Compares employees who stayed vs. exited across departments
- Helps identify departments with higher attrition risk

## 7. Attrition by Gender (Donut
- Displays overall attrition split between male and female employees
- Highlights gender-related workforce trends

## Interactive Filters (Slicers)
- Department: HR, R&D, Sales
- Gender: Male, Female
- Age Group: Under 25, 25–34, 35–44, 45–54, Over 55
- Enables deep-dive analysis and dynamic insights

## DAX Formulas Used
1. Total employees      = COUNT('HR data'[emp no])
2. Avg age              = AVERAGE('HR data'[Age])
3. Attrition %          = DIVIDE('HR data'[Employee Quit],'HR data'[Total employees],100)
4. Average satisfaction = AVERAGE('HR data'[Job Satisfaction])
5. Current Employee     = CALCULATE(COUNT('HR data'[CF_attrition label]),KEEPFILTERS('HR data'[CF_attrition label]="current
   employees"))
6. Employee Quit        = CALCULATE(COUNT('HR data'[CF_attrition label]),KEEPFILTERS('HR data'[CF_attrition label]="Ex-
   employees"))

## Conclusion
The HR dashboard highlights a 16% attrition rate, with higher exits among 25–44 age groups.
R&D and Sales departments contribute the most to employee turnover.
- Employees from Life Sciences and Medical backgrounds show higher quit rates.
- Male employees account for a larger share of attrition.
- The average satisfaction score (2.73) indicates moderate employee engagement.
- Younger and mid-career employees require focused retention strategies.

Overall, the dashboard supports data-driven HR decisions to improve workforce stability.





