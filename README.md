# HR Employee Attrition Analysis (SQL) 🧮

SQL analysis of employee attrition patterns — identifying which departments, roles, and factors are most linked to employees leaving the company.

## 🎯 The Problem
Employee turnover is expensive and disruptive. I wanted to use SQL to find out: which departments and roles lose the most people, and what factors (salary, overtime, tenure) are associated with attrition — the kind of analysis an HR or PM team would use to prioritize retention efforts.

## 📂 Dataset
**IBM HR Analytics Employee Attrition & Performance** — 1,470 employees, 35 attributes (department, role, income, satisfaction scores, overtime, tenure, etc.) — sourced from Kaggle.

## 📈 Key Findings
- **Overall attrition rate: 16.1%** (237 of 1,470 employees left)
- **Sales** has the highest departmental attrition rate (20.6%), while **Research & Development** — the largest department — has the lowest (13.8%)
- **Sales Representative** is the highest-risk role by far, with a **39.8%** attrition rate — nearly 6x higher than Manufacturing Director (6.9%), the most stable role
- Employees who left earned **$4,787/month on average**, vs. **$6,833/month** for those who stayed — a ~$2,000 gap
- Employees who work **overtime** leave at **almost 3x the rate** (30.5%) of those who don't (10.4%) — the strongest single factor found in this analysis

## 🖼️ Query Results

**Attrition by Department**

| Department | Total Employees | Attrition Rate |
|---|---|---|
| Sales | 446 | 20.6% |
| Human Resources | 63 | 19.0% |
| Research & Development | 961 | 13.8% |

**Attrition by Job Role**

| Job Role | Total Employees | Attrition Rate |
|---|---|---|
| Sales Representative | 83 | 39.8% |
| Laboratory Technician | 259 | 23.9% |
| Human Resources | 52 | 23.1% |
| Sales Executive | 326 | 17.5% |
| Research Scientist | 292 | 16.1% |
| Manufacturing Director | 145 | 6.9% |

**Overtime vs. Attrition**

| Works Overtime | Total Employees | Attrition Rate |
|---|---|---|
| Yes | 416 | 30.5% |
| No | 1,054 | 10.4% |

## 🧰 Built With
- SQL (SQLite via DB Browser for SQLite)
- Techniques: `GROUP BY`, `CASE WHEN`,
