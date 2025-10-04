# HR Analysis Project – MMZY Company

**Author:** Ahmed Satti  
**Tools Used:** Python, Excel (Power Query), Plotly, Pandas 
**Dataset:** [HRDataset_v14_cleaned_Full.csv](https://www.kaggle.com/datasets/rhuebner/human-resources-data-set)

---

## Introduction

This capstone project analyzes HR data to uncover insights into employee turnover, recruitment efficiency, absence trends, and leadership impact. The goal is to empower MMZY Company with data-driven strategies to improve retention, hiring, and performance management.

---

## Mission Statement

Leverage HR analytics to identify key workforce trends and provide actionable recommendations that reduce costs and enhance operational efficiency.

---

## Stakeholders

- **HR Department:** Improve hiring and retention strategies  
- **Department Managers:** Understand team performance and leadership impact  
- **Employees:** Benefit from better management and increased satisfaction

---

## Dataset Overview

- **Source:** Kaggle  
- **Rows:** 311 (excluding header)  
- **Columns:** 36  
- **ETL Tool:** Power Query (Excel)

### Data Preparation

- Removed duplicates across all columns  
- Converted `Zip` column to text  
- Fixed `DOB` column formatting and created a new date-based `Age` column  
- Age formula:  
  ```excel
  Age = Duration.Days(Date.From(DateTime.LocalNow()) - Date.From([DOB])) / 365



Value Proposition
- Cost Reduction: Lower turnover saves millions annually
- Efficiency Gains: Streamlined recruitment improves productivity
- Workforce Stability: Addressing absence and leadership gaps boosts engagement

Project Scope
- Employee Turnover
- Recruitment Efficiency
- Employee Absence Analysis
- Leadership and Retention

Analytical Methods
- Data Visualization: Bar charts, area charts, interactive plots (Plotly)
- Aggregation & Grouping: pandas.groupby()
- Preprocessing: Type conversion, missing values, tenure calculations
- Interactive Dashboards: Plotly Express

Challenges
- Historical data may not reflect recent changes
- Departmental differences limit generalization

Business Questions & Insights
1. Employee Turnover
- High turnover in Production and IT/IS
- Lower satisfaction correlates with exits
- Entry-level roles (e.g., Production Technician I/II) most affected
- Estimated cost per exit: $5,000–$10,000
Recommendations:
- Improve conditions in high-turnover departments
- Conduct exit interviews
- Support entry-level staff with development programs

2. Recruitment Efficiency
- Website and Employee Referrals yield longer tenures
- Indeed and LinkedIn produce high performers but shorter stays
- CareerBuilder shows lower retention
- Potential savings: 15–20% by reducing external agency use
Recommendations:
- Invest in retention strategies for LinkedIn/Indeed hires
- Prioritize Website recruitment
- Investigate short tenure among high performers

3. Employee Absence Analysis
- Satisfaction inversely related to absence
- High performers have fewer absences
- Some departments show excessive absence
- Productivity loss: ~$2,000 per employee annually
Recommendations:
- Boost satisfaction to reduce absences
- Support high performers
- Investigate departments with unexplained absence trends

4. Leadership and Retention
- Managers like Brannon Miller and Brian Champaigne drive performance
- Others show low team scores (e.g., Debra Houlihan, John Smith)
- Strong leadership correlates with retention
- Poor leadership may increase turnover by 20%
Recommendations:
- Leadership training for low-performing managers
- Share best practices from top managers
- Implement 360-degree feedback


Deliverables
- AhmedSatti_HR_Final.pbix – Interactive Power BI dashboard
- AhmedSatti_HRDataset_v14_cleaned.xlsx – Cleaned dataset
- AhmedSatti_HR_FinalDoc.docx – Documentation outlining business logic and steps

Conclusion
- Turnover linked to department, satisfaction, and role
- Website and referrals are top hiring sources
- Absence tied to satisfaction and performance
- Manager quality drives team success and retention

## About the Author  
Ahmed Satti  
Business & Data Analyst  
Calgary, Alberta  
Email: aihsatti@gmail.com  
LinkedIn: https://www.linkedin.com/in/ahmed-satti-53063470/
