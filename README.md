# AI Job Hiring Analytics Dashboard (Power BI Project)
## Role: Data Analyst
This project demonstrates my practical work as a Data Analyst: I collected, cleaned, and visualized job-listing data to reveal hiring trends for AI roles across companies, locations, and time. The dashboard was built end-to-end in Power BI, focusing on actionable insights for job seekers, hiring managers, and data-savvy professionals.

## Project Objective
The objective is to create an interactive dashboard that answers business questions about the AI hiring market and helps users quickly understand:

•	Which companies are actively hiring for AI roles and when

•	Salary trends by experience and role

•	Remote vs on-site hiring patterns

•	Skills, experience and benefit expectations across roles and industries

•	Urgent / time-sensitive opportunities (based on application deadlines)

## Dataset Used
- <a href="https://github.com/Atif20004/AI-Job-Hiring-Analytics-Dashboard/blob/main/Ai_hiring_data.xlsx">Dataset</a>

# Key Questions & Expanded KPIs
## Primary KPIs
1.	Total Jobs Posted (overall and by month/year)
2.	Average Salary (USD) by experience level and by job title
3.	Average Experience Required (years) across roles
4.	Average Benefits Score by company and role
## Additional KPIs & Analytical Questions
5.	Top Hiring Companies (by number of postings and by industry)
6.	Work Mode Distribution (On-site / Hybrid / Remote) — counts and percentages
7.	Top Roles with Highest Demand (Total_Jobs_Posted, earliest deadlines)
8.	Skill Frequency — most commonly required skills across roles
9.	Job Description Length — correlation with salary or benefits (longer descriptions → more senior roles?)
10.	Benefits vs Salary — is higher benefits_score correlated with higher salaries?
11.	Remote Ratio by Job Title — which roles are more remote-friendly?
12.	Company Size Effects — how salary, benefits and experience requirements vary by company_size
13.	Urgency / Closing Window — identify roles with near application_deadlines for fast action

# Project Process
## 1. Data Understanding
•	Reviewed each column to decide which KPIs could be derived.

•	Identified categorical vs numeric features and columns needing standardization (job titles, company names, location codes).

## 2. Data Cleaning & Transformation (Power Query)
•	Removed duplicates and empty/invalid rows.

•	Standardized text fields (lower/upper case and consistent naming).

•	Parsed posting_date and application_deadline into Date type and created days_to_deadline for urgency calculations.

•	Converted salary fields to a consistent salary_usd column (where currency conversion was possible/assumed).

•	Extracted year and month fields for time-series analysis.

## 3. Calculated Fields & DAX Metrics
•	Total_Jobs_Posted (count of job_id)

•	Avg_Salary (average of salary_usd)

•	Avg_Exp_Required (average years_experience)

•	Avg_Benefits_Score (average of benefits_score)

•	Jobs_Near_Deadline (count where days_to_deadline <= 7)

•	Skills_Count (count of skills in required_skills — used for scatter/insight)

4. Dashboard Design & Iteration
•	Selected visuals to answer the KPIs above: Map, Line chart, Bar chart, Donut chart, Treemap, Scatter plot, and a ranked Table.

•	Iterated on layout for clarity and storytelling: top KPI cards, central time-series, geographic map, role-level table and scatter for deeper analysis.

