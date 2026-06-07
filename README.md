# HR Attrition & Retention Analysis

## 1. Executive Summary

This project analyzes employee attrition data for a company of 311 employees to identify the key drivers behind a high overall attrition rate of **33.44%**. The analysis reveals that attrition is concentrated in specific departments and is strongly linked to short tenure, low engagement, and managerial performance. The primary recommendation is to focus retention efforts on the Production and Software Engineering departments, address management practices with the highest turnover rates, and implement early-tenure onboarding improvements to reduce exits within the first 3 years.

---

## 2. Business Problem

The company is experiencing a critical employee retention challenge. With an overall attrition rate of **33.44%** and a voluntary turnover rate of **28.30%**, the organization is losing a significant portion of its workforce — most of it willingly. This raises two core questions:

- **Where** is attrition happening the most?
- **Why** are employees choosing to leave?

Understanding the root causes is essential to reduce hiring costs, protect institutional knowledge, and improve workforce stability.

---

## 3. Dataset

| Element | Value |
|---|---|
| Total Employees | 311 |
| Active Headcount | 207 |
| Terminated Employees | 104 |
| Departments Covered | 5 (Production, Software Engineering, Sales, IT/IS, Admin Offices) |
| Key Metrics Tracked | Attrition rate, voluntary turnover, absences, lateness, satisfaction, engagement, tenure |

---

## 4. Methodology

- Calculated overall and voluntary attrition rates
- Segmented attrition by department and by manager
- Measured average tenure before termination per department
- Analyzed satisfaction and engagement scores for employees who left
- Compared satisfaction vs. engagement to detect silent disengagement

---

## 5. Analysis & Findings

### Q1: Which departments have the highest attrition?

The **Production** and **Software Engineering** departments show the highest attrition bars on the dashboard, both significantly above the 50% reference line visually. **Sales**, **IT/IS**, and **Admin Offices** follow with progressively lower rates.

> **Insight:** Production and Software Engineering together likely account for the majority of voluntary exits, making them the highest-priority departments for retention intervention.

---

### Q2: Which managers have the highest voluntary turnover?

The top 10 managers by voluntary turnover rate reveal a striking concentration:

| Manager | Voluntary Turnover Rate |
|---|---|
| Amy Dunn | 61.90% |
| Webster Butler | 61.90% |
| Kissy Sullivan | 45.45% |
| Michael Albert | 36.36% |
| Elijah Gray | 31.82% |

> **Insight:** Two managers alone — Amy Dunn and Webster Butler — each have a voluntary turnover rate of nearly **62%**, which is almost double the company average. This suggests that managerial behavior or team environment is a significant driver of attrition, not just role or department.

---

### Q3: How long do employees stay before leaving?

Average tenure before termination varies sharply across departments:

| Department | Avg. Tenure Before Termination (years) |
|---|---|
| Software Engineering | 3.98 |
| Production | 3.70 |
| Sales | 2.46 |
| IT/IS | 1.68 |
| Admin Offices | 1.10 |

> **Insight:** Employees in Admin Offices and IT/IS are leaving very early — within **1 to 1.7 years** on average. This indicates a likely failure in onboarding, role-fit, or early employee experience rather than long-term dissatisfaction.

---

### Q4: Are employees satisfied and engaged when they leave?

The average satisfaction score for leavers is **3.88 / 5**, and the average engagement score is also moderate. Breaking this down by department:

| Department | Avg. Satisfaction (Leavers) | Avg. Engagement (Leavers) |
|---|---|---|
| Sales | 4.80 | 3.62 |
| Software Engineering | 4.25 | 3.96 |
| Production | 3.86 | 4.10 |
| IT/IS | 3.60 | 4.40 |
| Admin Offices | 3.50 | 3.52 |

> **Insight:** Sales employees report high satisfaction (4.80) but leave anyway — this is a classic signal of **push factors** (e.g., better opportunities elsewhere, compensation gaps) rather than internal dissatisfaction. IT/IS employees show high engagement (4.40) but low satisfaction (3.60), suggesting they care about their work but face environmental or management issues. Admin Offices scores low on both dimensions, indicating a fundamentally poor experience.

---

## 6. Recommendations

| Finding | Recommendation |
|---|---|
| Amy Dunn & Webster Butler have ~62% turnover rates | Conduct managerial review; consider coaching, reassignment, or team restructuring |
| Admin Offices avg. tenure is only 1.10 years | Redesign onboarding and 90-day check-in process to catch early dissatisfaction |
| IT/IS employees are engaged but unsatisfied | Investigate work environment, compensation, and direct management quality |
| Sales employees are satisfied but still leave | Conduct stay interviews; review compensation benchmarking against market |
| Overall attrition at 33.44% | Set a 12-month target to reduce voluntary turnover to below 20% through structured retention programs |

---

## 7. Conclusion

The company faces a serious attrition problem that is not caused by a single factor. Analysis shows that **managerial performance**, **early employee experience**, and **department-level conditions** are the three main levers driving the 33.44% attrition rate. The most urgent actions are addressing the two managers with ~62% turnover rates and redesigning the onboarding experience for Admin Offices and IT/IS — where employees are leaving within the first 1-2 years.

---

## 8. Technologies Used

- **Power BI** — Dashboard design and data visualization
- **DAX** — Calculated measures (attrition rate, voluntary turnover, averages)
- **Excel** — Data preparation and cleaning

---

## 9. Repository Structure

```
Progect-for-HR-Attritions/
│
├── README.md                        ← Project report (this file)
├── Dashboard-hr-overview.jpg        ← Overview dashboard screenshot
└── Dashboard-hr-drivers.jpg         ← Drivers dashboard screenshot
```
