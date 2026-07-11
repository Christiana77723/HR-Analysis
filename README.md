## Project Structure

| Page | Nav Button | Content |
|------|------------|---------|
| 1 | **Home** | KPI cards (Total Employees, Male/Female split), stacked bar — Due for Promotion vs. Will be Retrenched by Department, bar chart — Employees by Job Satisfaction, pie chart — Employees by OverTime, JobRole summary table, Gender/Employee Name slicers |
| 2 | **Detail** | Due for Promotion KPI (72, 4.9%), Undue Promotion KPI (1,398, 95.1%), bar chart — Employees by Service Year, bar chart — Employees by Job Level, donut chart — Employees by Distance Status, "In Service" KPI (1,353) |
| 3 | **Action** | Gauges — Performance Rating, Monthly Income, Distance From Home, KPI — JobInvolvement & Promotion Bench (vs. goal), pie — Job Satisfaction by OverTime, funnel — Monthly Income by Job Role, bar — Due for Promotion by Department, Employee Name search/filter |

## Data Summary

| File | Records | Fields | Content |
|------|---------|--------|---------|
| `HR_Analytics_Data.csv` | 1,470 | 35 | Core HR dataset — demographics, pay, satisfaction, performance, tenure |
| `HR_employee_data.csv` | 1,470 | 2 | EmployeeNumber → Employee Name lookup |
| `data_csv_promomtion.csv` | 72 | 2 | Employees flagged as due for promotion |
| `data_csv_Retrenchment.csv` | 1,470 | 2 | Retrenchment flag (117 = at risk, 1,353 = not) |

No missing values in the core dataset; the three supporting files are designed to join back to it via employee name/number to power the promotion and retrenchment visuals.
