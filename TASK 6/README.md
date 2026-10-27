# Healthcare Analytics Dashboard using Power BI

## Project Overview

This project focuses on developing an interactive Healthcare Analytics Dashboard in Power BI using the cleaned healthcare dataset prepared during Week 5. The dashboard provides insights into patient demographics, hospital admissions, billing patterns, medical conditions, insurance coverage, and overall healthcare performance metrics.

The primary objective is to enable healthcare stakeholders to monitor key performance indicators (KPIs), identify trends, analyze patient distributions, and support data-driven decision-making through interactive visualizations.

---

## Objectives

- Create healthcare KPI measures using DAX.
- Analyze patient demographics by age group and gender.
- Examine billing and hospital stay patterns.
- Visualize admission and medical condition distributions.
- Track admission trends over time.
- Enable interactive exploration using slicers and cross-filtering.
- Design a professional and user-friendly healthcare dashboard.

---

## Tools and Technologies

- Power BI Desktop
- DAX (Data Analysis Expressions)
- Healthcare Dataset (Cleaned Dataset from Week 5)
- DAX Measures

### Total Patients
```
Total Patients =
DISTINCTCOUNT(Healthcare[Patient ID])
```

### Average Billing Amount
```
Average Billing Amount =
AVERAGE(Healthcare[Billing Amount])
```

### Average Length of Stay
```
Average Length of Stay =
AVERAGE(Healthcare[Length of Stay])
```

---

## Dashboard Components

### 1. KPI Cards

#### The top section of the dashboard contains KPI cards displaying:

- Total Patients
- Average Billing Amount
- Average Length of Stay
- Readmission Rate

These metrics provide an instant overview of healthcare performance.

### 2. Patient Demographics Analysis

#### Visualizations used:

- Clustered Column Chart
- Stacked Bar Chart
- Pie Chart (Optional)

#### Analysis includes:

- Patient distribution by Age Group
- Patient distribution by Gender

### 3. Matrix Table

#### A matrix visualization is used to compare:

- Medical Conditions
- Age Groups
- Gender

#### Metric displayed:

- Patient Count

This allows easier comparison of disease prevalence across demographic groups.

### 4. Donut Chart

The Donut Chart displays patient distribution based on:

- Admission Type
- Medical Condition
- Insurance Provider

The visualization highlights the proportion of each category.

### 5. Admission Trend Analysis

#### Trend visualizations include:

- Line Charts
- Area Charts

#### Metrics analyzed:

- Number of Admissions Over Time
- Department-wise Admissions
- Monthly or Yearly Trends

### 6. Interactive Slicers

The dashboard includes slicers for:

- Insurance Provider
- Admission Type
- Age Group
- Gender
- Medical Condition

Users can dynamically filter dashboard visuals according to their requirements.

### 7. Cross-Filtering Features

Cross-filtering enables users to:

- Select an Insurance Provider and analyze patient counts.
- Select an Admission Type and examine billing trends.
- View changes in KPIs based on selected filters.

This improves dashboard interactivity and exploratory analysis.

---

## Dashboard Layout

### Top Section

#### KPI Cards:

- Total Patients
- Average Billing Amount
- Average Length of Stay
- Readmission Rate

### Middle Section

- Demographic Analysis
- Admission Distribution
- Medical Condition Analysis

### Bottom Section
- Trend Analysis
- Matrix Table
- Billing Distribution Charts
- Key Insights Generated

---

## The dashboard helps answer questions such as:

- Which age groups contribute the highest number of admissions?
- What medical conditions are most common among patients?
- Which insurance providers cover the largest patient population?
- How does billing vary across admission types?
- What is the average hospital stay duration?
- How frequently are patients readmitted?

---

## Features

- ✅ Dynamic KPI Monitoring
- ✅ Interactive Slicers
- ✅ Cross-Filtering Support
- ✅ Demographic Analysis
- ✅ Admission Trend Analysis
- ✅ Billing Insights
- ✅ Medical Condition Comparison
- ✅ Professional Dashboard Design

---

## Author

Madhumidha E
