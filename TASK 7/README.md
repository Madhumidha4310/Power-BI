# Student Performance Analysis and Feature Engineering

## Project Overview

This project focuses on analyzing the Student Performance in Exams Dataset to identify academic performance patterns based on demographic characteristics and examination scores. The dataset is cleaned, validated, statistically analyzed, and enhanced through feature engineering to provide meaningful insights into student achievement.

The project includes data cleaning, statistical analysis, feature creation, outlier detection, visualization, validation, and performance reporting.

---

## Problem Statement

Educational institutions need to identify students who may be at academic risk and understand the factors affecting performance.

By analyzing student demographics and examination scores, institutions can:

- Monitor academic performance.
- Identify high-performing and low-performing students.
- Detect performance gaps across subjects.
- Support decision-making for academic improvement programs.

---

## Dataset Description

### Original Dataset Columns

| Column | Description |  
|---------|-------------|
| gender	| Gender of the student |
| race/ethnicity | Ethnic group classification |
| parental level of education	| Parents' highest education level |
| lunch	| Lunch category |
| test preparation course	| Test preparation completion status |
| math score	| Mathematics score |
| reading score	| Reading score |
| writing score	| Writing score |

---

## Feature Engineering

The following new features are created:

Total Score
total_score = math_score + reading_score + writing_score


Maximum possible score = 300

Average Score
average_score = total_score / 3

Percentage
percentage = (total_score / 300) * 100

Pass/Fail Status

Example Rule:

Pass = Average Score >= 40
Fail = Average Score < 40

Performance Category
Average Score	Category≥ 80	High
50 - 79	Average
< 50	Low
Data Cleaning Tasks
Categorical Data Cleaning

Columns:

gender
race/ethnicity
parental level of education
lunch
test preparation course

Activities:

Remove extra spaces.
Convert text to consistent format.
Correct inconsistent category labels.
Standardize categorical values.
Score Validation

Columns:

math score
reading score
writing score

Validation Checks:

Missing values
Incorrect data types
Scores below 0
Scores above 100

Only valid scores within the range 0–100 are retained.

Statistical Analysis

Performed for:

Mathematics Score
Reading Score
Writing Score

Metrics Calculated:

Mean
Median
Standard Deviation
Minimum
Maximum
First Quartile (Q1)
Third Quartile (Q3)
Interquartile Range (IQR)
Outlier Detection

Outliers are identified using:

IQR Method
Lower Bound = Q1 − 1.5 × IQR

Upper Bound = Q3 + 1.5 × IQR


Scores outside these limits are flagged for review.

Data Visualization
1. Mathematics Score Distribution

Chart Type: Histogram

X-Axis: Math Score Intervals
Y-Axis: Student Count

Purpose:

Understand distribution of mathematics scores.
2. Reading Score Distribution

Chart Type: Histogram

X-Axis: Reading Score Intervals
Y-Axis: Student Count

Purpose:

Analyze reading performance.
3. Writing Score Distribution

Chart Type: Histogram

X-Axis: Writing Score Intervals
Y-Axis: Student Count

Purpose:

Analyze writing performance.
4. Subject Comparison Box Plot

Chart Type: Box Plot

X-Axis: Subject Name
Y-Axis: Subject Score

Purpose:

Compare score distributions across all subjects.
5. Mathematics Outlier Analysis

Chart Type: Box Plot

Purpose:

Identify unusual mathematics scores.
6. Reading Outlier Analysis

Chart Type: Box Plot

Purpose:

Identify unusual reading scores.
7. Writing Outlier Analysis

Chart Type: Box Plot

Purpose:

Identify unusual writing scores.
8. Total Score Distribution

Chart Type: Histogram

X-Axis: Total Score
Y-Axis: Student Count

Purpose:

Understand overall academic performance.
9. Average Score Distribution

Chart Type: Histogram

X-Axis: Average Score
Y-Axis: Student Count

Purpose:

Analyze average student achievement.
10. Pass/Fail Analysis

Chart Type: Bar Chart

X-Axis: Pass/Fail Status
Y-Axis: Student Count

Purpose:

Compare passing and failing students.
11. Performance Category Analysis

Chart Type: Bar Chart

X-Axis: Performance Category
Y-Axis: Student Count

Categories:

High
Average
Low

Purpose:

Compare performance levels.
12. Subject Mean Comparison

Chart Type: Bar Chart

X-Axis: Subject Name
Y-Axis: Mean Score

Purpose:

Identify highest and lowest performing subjects.
Data Validation

The cleaned dataset undergoes the following validation checks:

Missing Values
Detect missing records.
Handle null values appropriately.
Duplicate Records
Identify duplicate student entries.
Remove duplicates if necessary.
Score Validation

All subject scores must satisfy:

0 ≤ Score ≤ 100

Total Score Verification
total_score =
math_score +
reading_score +
writing_score

Average Score Verification
average_score =
total_score / 3

Percentage Verification
percentage =
(total_score / 300) * 100

Pass/Fail Verification

Validate according to predefined passing criteria.

Performance Category Verification

Ensure category assignment matches average score ranges.

Student Performance Analysis
Subject Performance

Evaluate average performance across:

Mathematics
Reading
Writing

Identify:

Highest-performing subject
Lowest-performing subject
Score Distribution Analysis

Study:

Score concentration
Variability
Distribution shape
Overall Performance Summary

Analyze:

Total Scores
Average Scores
Percentages

to understand overall academic achievement.

Pass/Fail Summary

Calculate:

Number of Passed Students
Number of Failed Students
Pass Percentage
Fail Percentage
Performance Category Summary

Count student distribution among:

High Performers
Average Performers
Low Performers
Outlier Insights

Review unusual scores and determine:

Whether they are genuine observations.
Their impact on statistical summaries.
Data Quality Summary

Document:

Missing values found
Duplicate records found
Invalid score corrections
Feature engineering validations
Deliverables
Task 7 Deliverables

✅ Cleaned Dataset

✅ Validated Dataset

✅ Feature-Engineered Dataset

✅ Statistical Summary Report

✅ Outlier Detection Report

✅ Feature Validation Report

Task 8 Deliverables

✅ Student Performance Analysis Report

✅ Performance Visualizations

✅ Subject-wise Performance Summary

✅ Overall Academic Performance Summary

✅ Recommendations for Academic Improvement

✅ Final Conclusion Report

Expected Outcomes

After completing this project, users will be able to:

Identify academic risk factors.
Understand student performance trends.
Compare performance across subjects.
Detect unusual score patterns.
Evaluate pass/fail rates.
Categorize students based on achievement levels.
Produce a reliable dataset for future predictive modeling and analysis.
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook / Google Colab
Conclusion

This project transforms raw student examination data into a validated and feature-engineered dataset suitable for educational analytics. Through statistical analysis, visualizations, outlier detection, and performance categorization, the study provides valuable insights into student achievement and establishes a strong foundation for future predictive analysis and academic support initiatives.
