# HR Attrition & Retention Analysis

## 1. Executive Summary

This project analyzes the main employee table in `HRDataset_v14.xlsx` to understand where attrition is concentrated and which workforce factors appear most associated with employee exits. The dataset contains 311 employees, of whom 207 are active, 88 left voluntarily, and 16 were terminated for cause, producing an overall attrition rate of 33.44% and a voluntary turnover rate of 28.30%. [1]

The analysis shows that attrition is heavily concentrated in the Production department, while Software Engineering has the highest attrition rate among medium-sized operating departments. Manager-level variation is also substantial, with several managers showing voluntary turnover rates above 30% and the two highest managers at 61.90%. [1]

The main business implication is that retention should not be treated as a company-wide generic problem. The strongest actions should focus on high-risk departments, high-turnover managers, and the early employee experience in departments where tenure before exit is especially short. [1]

## 2. Business Problem

The business problem is high employee loss, especially voluntary exits that create replacement cost, disrupt operations, and weaken team continuity. The central goal of this analysis is to identify where attrition is highest, what patterns characterize exiting employees, and which actions are most likely to improve retention. [1]

Instead of describing dashboards or code, this report answers a decision-focused question: what did the data reveal, and why should a manager care? The answer matters because attrition is not evenly distributed across the workforce; it is concentrated in specific departments and management contexts. [1]

## 3. Dataset

The report is based only on the large employee table `Table1` from the original Excel file. That table contains 311 rows and 36 columns, including employee status, department, manager, salary, performance score, engagement survey, satisfaction, lateness, absences, hire date, termination date, and termination reason. [1]

| Element | Value |
|---|---|
| Employees | 311 [1] |
| Active employees | 207 [1] |
| Voluntarily terminated | 88 [1] |
| Terminated for cause | 16 [1] |
| Departments | 6 [1] |
| Overall attrition rate | 33.44% [1] |
| Voluntary turnover rate | 28.30% [1] |

## 4. Methodology

The analysis used the original employee table to classify employment outcomes, compare attrition by department and manager, and derive tenure from hire and termination dates. It also examined engagement, satisfaction, absences, and lateness to understand whether exits are more consistent with poor experience, early mismatch, or manager-specific issues. [1]

The logic of the report is organized around business questions rather than tools. Each section follows a simple pattern: question, evidence from the data, and interpretation. [1]

## 5. Analysis & Findings

### Where is attrition highest?

Production accounts for 209 employees and 75 voluntary exits, giving it the largest absolute attrition burden in the company. Software Engineering has only 11 employees, but its overall attrition rate reaches 36.36%, which is the highest among the main non-executive operating departments outside the tiny Executive Office category. [1]

| Department | Employees | Voluntary exits | Overall attrition | Voluntary turnover |
|---|---:|---:|---:|---:|
| Production | 209 [1] | 75 [1] | 39.71% [1] | 35.89% [1] |
| Software Engineering | 11 [1] | 3 [1] | 36.36% [1] | 27.27% [1] |
| Admin Offices | 9 [1] | 1 [1] | 22.22% [1] | 11.11% [1] |
| IT/IS | 50 [1] | 6 [1] | 20.00% [1] | 12.00% [1] |
| Sales | 31 [1] | 3 [1] | 16.13% [1] | 9.68% [1] |
| Executive Office | 1 [1] | 0 [1] | 0.00% [1] | 0.00% [1] |

This means the first retention priority should be Production because it combines scale and high loss. Software Engineering should be treated as a second priority because a small team losing over one-third of its headcount can create disproportionate operational risk. [1]

### Which managers appear most associated with voluntary exits?

Manager-level turnover is highly uneven. Amy Dunn and Webster Butler each supervise 21 employees and each show a voluntary turnover rate of 61.90%, while the next highest visible group still remains materially lower. [1]

| Manager | Team size | Voluntary exits | Voluntary turnover |
|---|---:|---:|---:|
| Amy Dunn | 21 [1] | 13 [1] | 61.90% [1] |
| Webster Butler | 21 [1] | 13 [1] | 61.90% [1] |
| Kissy Sullivan | 22 [1] | 10 [1] | 45.45% [1] |
| Michael Albert | 22 [1] | 8 [1] | 36.36% [1] |
| Elijiah Gray | 22 [1] | 7 [1] | 31.82% [1] |

This pattern suggests that attrition is not driven only by role type or department structure. Management quality, team climate, and local work conditions are likely meaningful drivers and should be investigated through manager review, stay interviews, and comparative team diagnostics. [1]

### How early are employees leaving?

Employees do not leave at the same pace across departments. Average tenure before termination is 3.98 years in Software Engineering and 3.70 years in Production, but it falls to 2.46 years in Sales, 1.68 years in IT/IS, and only 1.10 years in Admin Offices. [1]

| Department | Avg. tenure before termination |
|---|---:|
| Software Engineering | 3.98 years [1] |
| Production | 3.70 years [1] |
| Sales | 2.46 years [1] |
| IT/IS | 1.68 years [1] |
| Admin Offices | 1.10 years [1] |
| Executive Office | 0.00 years [1] |

Very short tenure before exit usually points to weak onboarding, poor role fit, unmet expectations, or local supervision issues. In practice, this means some retention problems begin much earlier than annual performance cycles would reveal. [1]

### What do satisfaction and engagement suggest?

Among leavers, average satisfaction and engagement differ by department. Sales leavers show high satisfaction at 4.80 but lower engagement at 3.62, while IT/IS leavers show stronger engagement at 4.40 than satisfaction at 3.60; Admin Offices leavers are low on both dimensions at 3.50 and 3.52. [1]

| Department | Satisfaction of leavers | Engagement of leavers |
|---|---:|---:|
| Sales | 4.80 [1] | 3.62 [1] |
| Software Engineering | 4.25 [1] | 3.96 [1] |
| Production | 3.86 [1] | 4.10 [1] |
| IT/IS | 3.60 [1] | 4.40 [1] |
| Admin Offices | 3.50 [1] | 3.52 [1] |
| Executive Office | 3.00 [1] | 4.83 [1] |

These differences matter because they imply that not all exits come from the same root cause. Some employees appear to leave despite acceptable sentiment, which can indicate external opportunities or compensation gaps, while other groups show signs of weaker internal experience. [1]

### Why are employees leaving voluntarily?

The most frequent voluntary termination reasons in the employee table include career change, unhappy, more money, hours, and another position. This indicates that attrition is shaped by both internal and external pressures rather than a single issue. [1]

The implication is practical: retention strategy should combine internal fixes such as manager coaching and onboarding redesign with external competitiveness measures such as compensation benchmarking and career path clarity. [1]

## 6. Recommendations

| Finding | Recommendation |
|---|---|
| Production combines the largest workforce with the largest number of voluntary exits. [1] | Make Production the first retention workstream, with monthly attrition monitoring and role-level breakdowns. [1] |
| Amy Dunn and Webster Butler each show 61.90% voluntary turnover. [1] | Run manager-level reviews, compare team climate measures, and prioritize coaching or structural intervention. [1] |
| Admin Offices and IT/IS show very short tenure before exit. [1] | Redesign onboarding, add 30/60/90-day check-ins, and audit role expectations during recruitment. [1] |
| Sales leavers report high satisfaction but still exit. [1] | Review compensation, mobility, and external market pull factors through stay interviews and exit coding. [1] |
| Voluntary reasons include career change, unhappy, more money, and another position. [1] | Build separate retention actions for compensation, career growth, and manager experience instead of using a single broad program. [1] |

## 7. Conclusion

The original employee table confirms that attrition is a real business problem, not just a visual pattern in the dashboard. The most important finding is concentration: Production carries the largest loss volume, Software Engineering shows a high rate for its size, and a small number of managers account for unusually high voluntary turnover. [1]

A stronger retention strategy should therefore focus on where the data points most clearly: manager-level intervention, early-tenure experience, and department-specific action instead of generic company-wide responses. That is the key story this project should communicate on GitHub. [1]

## 8. Technologies Used

- Excel for the original dataset and source table structure. [1]
- Power BI for dashboarding and visual communication of attrition patterns. [1]
- DAX for calculated metrics in the dashboard layer. [1]

## 9. Repository Structure

```text
Progect-for-HR-Attritions/
├── README.md
├── HRDataset_v14.xlsx
├── Dadhboard-for-hr-drivers.jpg
└── Dashboard-hr-2.jpg
```
