
# 📊 HR Analytics Dashboard | Power BI

## 📌 Project Overview

The HR Analytics Dashboard is an interactive Power BI solution designed to provide comprehensive insights into workforce demographics, employee performance, recruitment effectiveness, employee satisfaction, and organizational distribution.

This dashboard enables HR professionals and business stakeholders to make data-driven decisions by transforming raw HR data into meaningful visual insights.

---

## 🎯 Objectives

- Monitor workforce size and employee distribution.
- Track active and terminated employees.
- Analyze gender diversity across the organization.
- Evaluate recruitment channel effectiveness.
- Assess employee performance and satisfaction levels.
- Understand department-wise workforce allocation.
- Visualize employee locations geographically.

---

## 🛠️ Tools & Technologies Used

| Tool | Purpose |
|--------|---------|
| Power BI Desktop | Dashboard Development |
| DAX | Data Modeling & Calculations |
| Power Query | Data Cleaning & Transformation |
| Microsoft Excel / CSV | Data Source |
| PowerPoint | Dashboard Layout Design |

---

## 📂 Dataset Information

The dataset contains employee-related information, including:

- Employee Details
- Department Information
- Employment Status
- Gender
- Marital Status
- Salary Information
- Recruitment Source
- Performance Rating
- Employee Satisfaction Score
- Geographic Location

---

## 📊 Dashboard Features

### Interactive Filters

- Department Slicer
- Year Slicer

### KPI Cards

- Total Head Count
- Active Employees
- Terminated Employees
- Male Employees
- Female Employees

### Analytical Visualizations

- Salary Distribution by Department
- Marital Status Analysis
- Employee Distribution by Department
- Employee Performance Analysis
- Recruitment Source Analysis
- Employee Satisfaction Analysis
- State-wise Employee Distribution Map

---

## 📈 Key Metrics

### Total Head Count

Displays the total number of employees in the organization.

### Active Employees

Tracks currently active employees and their percentage contribution.

### Terminated Employees

Displays terminated employees and termination percentage.

### Gender Distribution

Shows workforce diversity through male and female employee counts and percentages.

### Salary Analysis

Provides department-wise salary expenditure.

---

## 📉 Dashboard Visualizations

### Marital Status Analysis

A donut chart showing employee distribution across:

- Single
- Married
- Divorced
- Separated

### Employee by Department

A bar chart displaying workforce allocation across departments such as:

- Production
- IT/IS
- Sales
- Software Engineering
- Admin Offices
- Executive Office

### Employee Performance

A pie chart categorizing employees into:

- Fully Meets Expectations
- Exceeds Expectations
- Needs Improvement
- Performance Improvement Plan (PIP)

### Recruitment Source Analysis

Evaluates hiring effectiveness from recruitment channels including:

- Indeed
- LinkedIn
- Google Search
- Employee Referral
- CareerBuilder
- Diversity Job Boards

### Employee Satisfaction Analysis

Employee satisfaction levels are categorized as:

| Rating | Category |
|----------|-----------|
| 1 | Very Low |
| 2 | Low |
| 3 | Acceptable |
| 4 | High |
| 5 | Very High |

### Geographic Distribution

A map visualization displaying employee locations across different states.

---

## 🧮 DAX Measures Used

### Head Count

```DAX
Head Count = COUNTROWS(HRData)
```

### Active Employees

```DAX
Active =
CALCULATE(
    [Head Count],
    HRData[Status] = "Active"
)
```

### Active Percentage

```DAX
Active % =
DIVIDE(
    [Active],
    [Head Count],
    0
)
```

### Terminated Employees

```DAX
Terminated =
CALCULATE(
    [Head Count],
    HRData[Status] = "Terminated"
)
```

### Male Employees

```DAX
Male =
CALCULATE(
    [Head Count],
    HRData[Gender] = "M"
)
```

### Female Employees

```DAX
Female =
CALCULATE(
    [Head Count],
    HRData[Gender] = "F"
)
```

---

## 🎨 Dashboard Development Process

1. Designed dashboard layout using PowerPoint.
2. Imported custom background into Power BI.
3. Added dashboard title and logo.
4. Created Department and Year slicers.
5. Developed DAX measures for KPI calculations.
6. Built interactive charts and visualizations.
7. Applied formatting and design enhancements.
8. Validated data accuracy and dashboard interactions.

---

## 💡 Business Insights Generated

This dashboard helps organizations:

- Monitor employee growth trends.
- Analyze workforce demographics.
- Improve recruitment strategies.
- Track employee performance.
- Measure employee satisfaction levels.
- Support strategic workforce planning.
- Improve HR decision-making.

## 📷 Dashboard Snapshot
![HR Dashboard](Screenshots/HR_Dashboard.pn)



