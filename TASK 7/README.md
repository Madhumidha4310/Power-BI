# Student Performance Analytics Dashboard using Power BI

## Project Overview

This project analyzes the Student Performance in Exams dataset containing 1,000 student records. The objective is to clean, transform, model, and visualize student performance data using Power BI.

---

## Dataset Description

The dataset contains student demographic information and examination scores.

### Source Columns

- Parental Level of Education
- Lunch
- Test Preparation Course
- Math Score
- Reading Score
- Writing Score
  
### Total Records

- Student Performance Table: 1,000 records
- Student Subject Scores Table: 3,000 records (after unpivoting)

---

## Step 1: Data Import

The dataset was imported into Power BI using:

Home → Get Data

The data was loaded into Power Query Editor for preprocessing.

## Step 2: Data Inspection

The following checks were performed:

- Column Quality
- Column Distribution
- Column Profile
- Null Value Detection
- Data Type Verification

### Score ranges observed:

| Subject	| Minimum	| Maximum	|Average |
|--------|---------|--------|----------|
| Math	| 0	| 100	|66.1 |
|Reading | 17	| 100	| 69.2 |
| Writing	| 10	| 100	| 68.1 |

## Step 3: Data Cleaning

The following transformations were applied:

- Trim
- Clean
- Standardized text formatting
- Removed unnecessary spaces
- Verified category values

### Categorical columns cleaned:

- Parental Education
- Lunch Type
- Test Preparation Course

## Step 4: Data Type Assignment

| Column	| Data Type |
|---------|-----------|
| Parental Education	| Text |
| Lunch | Text |
| Test Preparation Course | Text |
| Math Score	| Whole Number |
| Reading Score	| Whole Number |
| Writing Score	| Whole Number |

## Step 5: Adding Column

Custom Column:
`[Math Score] + [Reading Score] + [Writing Score]`

Column Name:
`Total Score`

Custom Column:
`Number.Round(
([Math Score] + [Reading Score] + [Writing Score]) / 3,
2
)`

Column Name:
`Average Score`

Custom Column:
`if [Average Score] >= 80 then "A"
else if [Average Score] >= 60 then "B"
else if [Average Score] >= 40 then "C"
else "F"`

Column Name:
`Performance Grade`

Custom Column:
`if [Math Score] >= 40
and [Reading Score] >= 40
and [Writing Score] >= 40
then "Pass"
else "Fail"`

Column Name:
`Pass Status`

Custom Column:
`List.Max({
[Math Score],
[Reading Score],
[Writing Score]
}) -
List.Min({
[Math Score],
[Reading Score],
[Writing Score]
})`

Column Name:
`Score Range`

## Step 6: Unpivot Subject Scores

### Selected Columns:

- Math Score
- Reading Score
- Writing Score

### Transformation:

Right Click → Unpivot Columns

### Renamed Columns:

| Original	| New |
|-----------|-----|
| Attribute	| Subject |
| Value	| Subject Score |

Created Table:

`Student Subject Scores`

## Student ID Creation

An Index Column was added before unpivoting:

`Add Column → Index Column → From 1`

Renamed As:

`Student ID`

## DAX Measures

### Total Students
`Total Students =
DISTINCTCOUNT('Student Performance'[Student ID])`

### Avg Math Score
`Avg Math Score =
AVERAGE('Student Performance'[Math Score])`

### Avg Reading Score
`Avg Reading Score =
AVERAGE('Student Performance'[Reading Score])`

### Avg Writing Score
`Avg Writing Score =
AVERAGE('Student Performance'[Writing Score])`

### Overall Average Score
`Overall Average Score =
AVERAGE('Student Performance'[Average Score])`

### Passed Students
`Passed Students =
CALCULATE(
[Total Students],
'Student Performance'[Pass Status]="Pass"
)`

### Overall Pass %
`Overall Pass % =
DIVIDE(
[Passed Students],
[Total Students],
0
)`

### Grade A Students
`Grade A Students =
CALCULATE(
[Total Students],
'Student Performance'[Performance Grade]="A"
)`

### Test Preparation Measures
`Avg Score by Student =
AVERAGE('Student Performance'[Average Score])`

### Completed Prep Avg =
`CALCULATE(
[Avg Score by Student],
'Student Performance'[Test Prep Course]="completed"
)`

### No Prep Avg =
`CALCULATE(
[Avg Score by Student],
'Student Performance'[Test Prep Course]="none"
)`

### Test Prep Score Difference
`Test Prep Score Difference =
[Completed Prep Avg] - [No Prep Avg]`

---

## Data Model

### Student Performance

#### Contains:

- Student ID
- Subject Scores
- Total Score
- Average Score
- Grade
- Pass Status

#### Rows:

- 1000
- Student Subject Scores

#### Contains:

- Student ID
- Subject
- Subject Score

#### Rows:

3000

### Relationship

`Student Performance[Student ID]
        1
        |
        |
        *
Student Subject Scores[Student ID]`

#### Relationship Type:

`One to Many (1:*)`

## Cross Filter:

### Additional Measures

#### Average Subject Score
`Average Subject Score =
AVERAGE('Student Subject Scores'[Subject Score])`

#### Subject Score Count
`Subject Score Count =
COUNT('Student Subject Scores'[Subject Score])`

## Author

Madhumidha E
