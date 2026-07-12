<img width="945" height="535" alt="Screenshot 2026-07-09 123248" src="https://github.com/user-attachments/assets/52bafe8b-6141-4963-a0af-dcca3b14faa1" />

<img width="951" height="535" alt="Screenshot 2026-07-09 123318" src="https://github.com/user-attachments/assets/4c1db640-52d2-4aef-bb6c-5f601b70f689" />

<img width="953" height="536" alt="Screenshot 2026-07-09 123400" src="https://github.com/user-attachments/assets/7fd6958a-ce7a-4726-a08e-1fd3c9026037" />




## Data Summary

| File | Records | Fields | Content |
|------|---------|--------|---------|
| `HR_Analytics_Data.csv` | 1,470 | 35 | Core HR dataset — demographics, pay, satisfaction, performance, tenure |
| `HR_employee_data.csv` | 1,470 | 2 | EmployeeNumber → Employee Name lookup |
| `data_csv_promomtion.csv` | 72 | 2 | Employees flagged as due for promotion |
| `data_csv_Retrenchment.csv` | 1,470 | 2 | Retrenchment flag (117 = at risk, 1,353 = not) |


## Project Structure

| Page | Nav Button | Content |
|------|------------|---------|
| 1 | **Home** | KPI cards (Total Employees, Male/Female split), stacked bar — Due for Promotion vs. Will be Retrenched by Department, bar chart — Employees by Job Satisfaction, pie chart — Employees by OverTime, JobRole summary table, Gender/Employee Name slicers |
| 2 | **Detail** | Due for Promotion KPI (72, 4.9%), Undue Promotion KPI (1,398, 95.1%), bar chart — Employees by Service Year, bar chart — Employees by Job Level, donut chart — Employees by Distance Status, "In Service" KPI (1,353) |
| 3 | **Action** | Gauges — Performance Rating, Monthly Income, Distance From Home, KPI — JobInvolvement & Promotion Bench (vs. goal), pie — Job Satisfaction by OverTime, funnel — Monthly Income by Job Role, bar — Due for Promotion by Department, Employee Name search/filter |

## Key Insights

**Workforce:** 1,470 employees total — 882 male (60%), 588 female (40%).

**Attrition risk (retrenchment):** 117 employees (~8%) flagged "will be retrenched"; 1,353 in service.

**Promotion pipeline:** Only 72 employees (4.9%) are due for promotion — 95.1% are not due, suggesting a fairly static promotion cycle.

**Department risk concentration:** Research & Development carries by far the largest combined promotion/retrenchment load (~120+ on the stacked bar), disproportionate to its headcount — worth flagging as a hotspot.

**Manager role stands out:** Of 102 managers, 22 are due for promotion and 44 are flagged for retrenchment — a notably high churn/mobility rate for a single role vs. e.g. Laboratory Technician (259 employees, only 3 promotion / 5 retrenchment).

**OverTime correlation:** 71.7% of employees work no overtime; the 28.3% who do overtime appear disproportionately represented in the "will be retrenched" and lower job-satisfaction slices — worth testing statistically since OverTime is a known attrition driver in this dataset family.

**Job levels are bottom-heavy:** Level 1 and Level 2 dominate headcount (500+ each), tapering sharply by Level 5 — a typical individual-contributor-heavy pyramid.

**Distance from home:** 64% of employees live "very close" to work, only ~16% "very far" — commute distance likely isn't a major attrition lever here.

**Compensation:** Sales Executive and Manager have the highest cumulative MonthlyIncome contribution; Human Resources and Sales Representative are lowest.

## Tool Used

**Power BI —** the dashboard itself (visuals, DAX measures like "Sum of Due for promotion," slicers, gauge/KPI cards, drill-through pages via bookmarks/buttons)

**CSV/Excel —** source data layer, structured for relational joins (EmployeeNumber as key)

# 👩‍💻 Author

**Sarkodie Christiana Gyemfua**

Accounting Graduate | Data Analyst


