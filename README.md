# HR-Attrition-Analytics
SQL + Power BI analysis of IBM HR employee attrition dataset.
Dashboard Preview:
<img width="991" height="555" alt="image" src="https://github.com/user-attachments/assets/2b24be7c-2058-4db1-9b98-5da1751c5950" />

Key Insights

- Sales has the highest attrition rate at 21%, followed by HR (19%) and R&D (14%)
- Overtime triples attrition risk — employees working overtime leave at ~31% vs ~10% for those who don't
- Employees who left earned 30% less on average than those who stayed ($4,787 vs $6,833)
- Under-25s are the highest flight risk, with a 38% attrition rate — the highest of any age group
- Sales employees have the longest average tenure (7.3 years), narrowly ahead of HR (7.2) and R&D (6.9)
- Sales Executives have the highest count of dissatisfied employees (JobSatisfaction = 1)
- Managers earn the most on average ($17,182); Sales Representatives earn the least ($2,626)
- Highest-risk profile: Sales Representatives working overtime on low income are the group most likely to leave


Tools & Techniques

- MySQL

Aggregate functions (COUNT, AVG, SUM) with GROUP BY
Window functions — RANK() OVER, SUM() OVER for running percentages
Conditional aggregation with CASE WHEN
HAVING clauses for filtered group-level conditions


- Power BI


DAX measures using CALCULATE, DIVIDE, RANKX, ALLEXCEPT
Calculated columns for custom age-band grouping
Conditional formatting on matrix visuals (job satisfaction heatmap)
Interactive department slicer
Color-coded visuals to highlight risk vs. safe categories


Validation Note

Every insight in this project was cross-validated between the SQL output and the Power BI dashboard to ensure both artifacts tell the same, accurate story — a step taken specifically to catch and correct discrepancies between exploratory SQL comments and the final live dataset.



Dataset

IBM HR Analytics Employee Attrition dataset — 1,470 employees, 9 job roles, 3 departments.
