# HR Attrition & Retention Analysis

## 1. Executive Summary

This project analyzes the main employee table in `HRDataset_v14.xlsx` to understand where attrition is concentrated and which workforce factors appear most associated with employee exits. The dataset contains 311 employees, of whom 207 are active, 88 left voluntarily, and 16 were terminated for cause, producing an overall attrition rate of 33.44% and a voluntary turnover rate of 28.30%.

The analysis shows that attrition is heavily concentrated in the Production department, while Software Engineering has the highest attrition rate among medium-sized operating departments. Manager-level variation is also substantial, with several managers showing voluntary turnover rates above 30% and the two highest managers at 61.90%.

The main business implication is that retention should not be treated as a company-wide generic problem. The strongest actions should focus on high-risk departments, high-turnover managers, and the early employee experience in departments where tenure before exit is especially short.

## 2. Business Problem

The business problem is high employee loss, especially voluntary exits that create replacement cost, disrupt operations, and weaken team continuity. The central goal of this analysis is to identify where attrition is highest, what patterns characterize exiting employees, and which actions are most likely to improve retention.

Instead of describing dashboards or code, this report answers a decision-focused question: what did the data reveal, and why should a manager care? The answer matters because attrition is not evenly distributed across the workforce; it is concentrated in specific departments and management contexts.

## 3. Dataset

The report is based only on the large employee table `Table1` from the original Excel file. That table contains 311 rows and 36 columns, including employee status, department, manager, salary, performance score, engagement survey, satisfaction, lateness, absences, hire date, termination date, and termination reason.

| Element | Value |
| --- | --- |
| Employees | 311 |
| Active employees | 207 |
| Voluntarily terminated | 88  |
| Terminated for cause | 16  |
| Departments | 6   |
| Overall attrition rate | 33.44% |
| Voluntary turnover rate | 28.30% |

## 4. Methodology

The analysis used the original employee table to classify employment outcomes, compare attrition by department and manager, and derive tenure from hire and termination dates. It also examined engagement, satisfaction, absences, and lateness to understand whether exits are more consistent with poor experience, early mismatch, or manager-specific issues.

The logic of the report is organized around business questions rather than tools. Each section follows a simple pattern: question, evidence from the data, and interpretation.

## 5. Analysis & Findings

### Where is attrition highest?

Production accounts for 209 employees and 75 voluntary exits, giving it the largest absolute attrition burden in the company. Software Engineering has only 11 employees, but its overall attrition rate reaches 36.36%, which is the highest among the main non-executive operating departments outside the tiny Executive Office category.

| Department | Employees | Voluntary exits | Overall attrition | Voluntary turnover |
| --- | --- | --- | --- | --- |
| Production | 209 | 75  | 39.71% | 35.89% |
| Software Engineering | 11  | 3   | 36.36% | 27.27% |
| Admin Offices | 9   | 1   | 22.22% | 11.11% |
| IT/IS | 50  | 6   | 20.00% | 12.00% |
| Sales | 31  | 3   | 16.13% | 9.68% |
| Executive Office | 1   | 0   | 0.00% | 0.00% |

This means the first retention priority should be Production because it combines scale and high loss. Software Engineering should be treated as a second priority because a small team losing over one-third of its headcount can create disproportionate operational risk.

### Which managers appear most associated with voluntary exits?

Manager-level turnover is highly uneven. Amy Dunn and Webster Butler each supervise 21 employees and each show a voluntary turnover rate of 61.90%, while the next highest visible group still remains materially lower.

| Manager | Team size | Voluntary exits | Voluntary turnover |
| --- | --- | --- | --- |
| Amy Dunn | 21  | 13  | 61.90% |
| Webster Butler | 21  | 13  | 61.90% |
| Kissy Sullivan | 22  | 10  | 45.45% |
| Michael Albert | 22  | 8   | 36.36% |
| Elijiah Gray | 22  | 7   | 31.82% |

This pattern suggests that attrition is not driven only by role type or department structure. Management quality, team climate, and local work conditions are likely meaningful drivers and should be investigated through manager review, stay interviews, and comparative team diagnostics.

### How early are employees leaving?

Employees do not leave at the same pace across departments. Average tenure before termination is 3.98 years in Software Engineering and 3.70 years in Production, but it falls to 2.46 years in Sales, 1.68 years in IT/IS, and only 1.10 years in Admin Offices.

| Department | Avg. tenure before termination |
| --- | --- |
| Software Engineering | 3.98 years |
| Production | 3.70 years |
| Sales | 2.46 years |
| IT/IS | 1.68 years |
| Admin Offices | 1.10 years |
| Executive Office | 0.00 years |

Very short tenure before exit usually points to weak onboarding, poor role fit, unmet expectations, or local supervision issues. In practice, this means some retention problems begin much earlier than annual performance cycles would reveal.

### What do satisfaction and engagement suggest?

Among leavers, average satisfaction and engagement differ by department. Sales leavers show high satisfaction at 4.80 but lower engagement at 3.62, while IT/IS leavers show stronger engagement at 4.40 than satisfaction at 3.60; Admin Offices leavers are low on both dimensions at 3.50 and 3.52.

| Department | Satisfaction of leavers | Engagement of leavers |
| --- | --- | --- |
| Sales | 4.80 | 3.62 |
| Software Engineering | 4.25 | 3.96 |
| Production | 3.86 | 4.10 |
| IT/IS | 3.60 | 4.40 |
| Admin Offices | 3.50 | 3.52 |
| Executive Office | 3.00 | 4.83 |

These differences matter because they imply that not all exits come from the same root cause. Some employees appear to leave despite acceptable sentiment, which can indicate external opportunities or compensation gaps, while other groups show signs of weaker internal experience.

### Why are employees leaving voluntarily?

The most frequent voluntary termination reasons in the employee table include career change, unhappy, more money, hours, and another position. This indicates that attrition is shaped by both internal and external pressures rather than a single issue.

The implication is practical: retention strategy should combine internal fixes such as manager coaching and onboarding redesign with external competitiveness measures such as compensation benchmarking and career path clarity.

## 6. Recommendations

| Finding | Recommendation |
| --- | --- |
| Production combines the largest workforce with the largest number of voluntary exits. | Make Production the first retention workstream, with monthly attrition monitoring and role-level breakdowns. |
| Amy Dunn and Webster Butler each show 61.90% voluntary turnover. | Run manager-level reviews, compare team climate measures, and prioritize coaching or structural intervention. |
| Admin Offices and IT/IS show very short tenure before exit. | Redesign onboarding, add 30/60/90-day check-ins, and audit role expectations during recruitment. |
| Sales leavers report high satisfaction but still exit. | Review compensation, mobility, and external market pull factors through stay interviews and exit coding. |
| Voluntary reasons include career change, unhappy, more money, and another position. | Build separate retention actions for compensation, career growth, and manager experience instead of using a single broad program. |

## 7. Conclusion

The original employee table confirms that attrition is a real business problem, not just a visual pattern in the dashboard. The most important finding is concentration: Production carries the largest loss volume, Software Engineering shows a high rate for its size, and a small number of managers account for unusually high voluntary turnover.

A stronger retention strategy should therefore focus on where the data points most clearly: manager-level intervention, early-tenure experience, and department-specific action instead of generic company-wide responses. That is the key story this project should communicate on GitHub.

## 8. Technologies Used

- Excel for the original dataset and source table structure.
- Power BI for dashboarding and visual communication of attrition patterns.
- DAX for calculated metrics in the dashboard layer.

## 9. Repository Structure

```text
Progect-for-HR-Attritions/
├── README.md
├── HRDataset_v14.xlsx
├── Dadhboard-for-hr-drivers.jpg
└── Dashboard-hr-2.jpg
```
