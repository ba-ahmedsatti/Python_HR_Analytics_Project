HR Analytics for MMZY Company | Python


Ahmed Satti


Introduction:


This project aims to analyze HR data to provide actionable insights into employee turnover, recruitment efficiency, employee absence, and leadership impact. Using Python based data analytics, we explore trends to enhance decision making for MMZY Company.


Phase 1: Mission Statement and Stakeholder Analysis

Mission Statement:

The objective is to utilize HR data analytics to help MMZY Company identify key workforce trends and provide recommendations to optimize retention, hiring, and performance management, ultimately leading to cost savings and improved operational efficiency.

Stakeholders:

•	HR Department: Improve hiring and retention strategies.

•	Department Managers: Gain insights into team performance and leadership impact.

•	Employees: Benefit from better management, and improve satisfactions.

Dataset:

•	Dataset: HRDataset_v14_cleaned_Full.csv (Open-source dataset from Kaggle).

•	Dataset URL: https://www.kaggle.com/datasets/rhuebner/human-resources-data-set 

•	ETL: Power Query using Excel – Contains 36 Columns & 311 Rows “Excluding Header”.


Data Preparation:

•	Remove Duplicates in all columns.

•	Change the data type of “Zip” column from Whole Number to Text.

•	Change the data type of “DOB” column from Text to Date data type, but an error occurred, therefore I created a column from examples/selections to make sure the year is 4 digits instead of 2 to capture year’s dates without an error, then removed the original “DOB” column and renamed the new custom column to DOB and then reorder it, and changed its type to date data type.

•	Add custom column named “Age” to capture the date without the time and calculate the duration between current date and employee’s DOB divided by the number of days within a year 365 to get their current Age in years, then reorder the new column.

•	Formula used: Age = Duration.Days(Date.From(DateTime.LocalNow()) - Date.From([DOB])) / 365.


Value Proposition:

•	Cost Reduction: Employee turnover is costly due to recruitment, training, and lost productivity. Reducing turnover by even 10% can save MMZY Company millions annually in hiring and onboarding costs.

•	Efficiency Gains: Improved recruitment processes lead to better hiring decisions, reducing hiring time and improving employee productivity.

•	Workforce Stability: Addressing absence and leadership gaps can enhance operational efficiency leading to a more engaged workforce.


Phase 2: Project Scope Statement:

•	Employee Turnover: Factors influencing employee exits, and associated costs.

•	Recruitment Efficiency: Impact of hiring sources on retention, and performance.

•	Employee Absence Analysis: Exploring the relationship between performance, and satisfaction.

•	Leadership and Retention: How Managers Influence Employee Success and the Costs of Keeping Them.


Analytical Methods:

•	Data Visualization: Bar charts, area charts, and interactive plots using Plotly.

•	Data Aggregation and Grouping: Using pandas groupby and aggregation functions to summarize and sort data.

•	Data Preprocessing: Type conversion, handling missing values, and date calculations for tenure.

•	Interactive Plots: Creating interactive visualizations with Plotly Express.


Challenges:

•	Data is historical: The data is historical and may not capture recent changes in the organization.

•	Department Differences: Department differences can make it hard to use these findings for the whole organization.


Phase 3: Business Question Analysis & Insights

1. Employee Turnover: What factors drive employees to leave?


Findings:

•	High turnover in Production, and IT/IS Departments.

•	Employees with lower satisfaction scores tend to leave the company more frequently.

•	Positions like Production Technician I and II experience higher turnover rates.


Financial Impact:

•	Average turnover cost per employee is estimated at $5,000–$10,000.

•	Reducing turnover by 10% could save the company $500,000–$1 million annually.


Recommendations:

•	Enhance work conditions and benefits in high-turnover departments like Production and IT/IS.

•	Establish a process for conducting exit interviews to analyze why employees are leaving.

•	Provide more support and development opportunities for entry level employees to improve their retention such as Production Technicians.


2. Recruitment Efficiency: Which hiring sources produce long tenured, high performing employees?
Findings:

•	Employees hired through Website, and Employee Referrals have longer tenures, and high performance.

•	Hires from Indeed, and LinkedIn intend to have higher performance score, but with shorter tenures compared to website.

•	CareerBuilder and Online Web Application show lower average tenures, suggesting the need to re-evaluate recruitment strategies for these Recruitment sources.


Financial Impact:

•	Reducing reliance on external agencies could cut hiring costs by 15-20%.


Recommendations:

•	Invest in training and development programs for employees recruited via Indeed, and LinkedIn to explore ways to increase their retention.

•	Prioritize the Website recruitment source for long tenured, high performing employees.

•	Investigate why high performers with "Exceeds" performance scores have shorter tenures and implement retention strategies.


3. Employee Absence Analysis: How does absence relate to satisfaction and performance?
Findings:

•	Higher satisfaction generally leads to fewer absences, but there's a slight increase in absences at the highest satisfaction level.

•	Employees with higher performance scores tend to have fewer absences. High performers show lower absence rates across various departments.

•	Certain departments experience excessive absence, indicating possible department issues.


Financial Impact:

•	Absence related productivity loss costs $2,000 per employee annually.

•	Addressing absence could save $200,000+ annually for MMZY Company.


Recommendations:

•	Focus on increasing employee satisfaction to reduce absences.

•	Provide additional support and resources to high performers to maintain their low absence rates and high productivity.

•	Investigate departments with high absence rates despite good satisfaction scores, and implement targeted improvements to address issues.


4. Leadership and Retention: How do managers impact performance?
Findings:

•	Managers like Brannon Miller, and Brian Champaigne show consistently high-performance scores.

•	Some managers such as Debra Houlihan and John Smith, have employees with low performance scores. This could mean those employees are more likely to leave.

•	Managers with higher overall performance scores generally have better team performance and retention.


Financial Impact:

•	Poor leadership can increase turnover by 20%, leading to significant hiring and training costs.
Recommendations:

•	Conduct leadership training for managers with high turnover rates.

•	Encourage high-performing managers to share their strategies and best practices with other managers to promote consistent high performance across all teams.

•	Implement a 360-degree feedback process, a method that gathers feedback from multiple workplace sources to evaluate how effective managers are.


Conclusion

•	Employee turnover is influenced by department, satisfaction, and position

•	Website and Employee Referrals are the most effective hiring sources

•	Satisfaction and performance are inversely related to absence rates

•	Manager quality significantly impacts team performance and retention






