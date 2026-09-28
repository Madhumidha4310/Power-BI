# README.md

# 📊 Superstore Sales Data Transformation in Power BI

## 📌 Introduction

This project focuses on cleaning and transforming the **Superstore Sales dataset** using **Microsoft Power BI Power Query Editor**.

The main objective is to transform the raw sales data into a clean and structured format by applying data cleaning, formatting, column transformation, and date-based operations.

---

## 🛠️ Software Used

* Microsoft Power BI Desktop
* Power Query Editor
* CSV File
* Power Query M Language

---

## 📂 Data Cleaning Process

### 1. Importing the Dataset

The Superstore Sales dataset was imported into Power BI using the **Text/CSV** option.

The dataset was then opened in the **Power Query Editor** for data cleaning and transformation.

---

### 2. Promoting Headers

The first row of the dataset was promoted as the column headers.

This helped to identify and organize the different fields available in the dataset.

---

### 3. Changing Data Types

The appropriate data types were assigned to the columns based on the data they contained.

Examples include:

| Column | Data Type |
|---|---|
| Order Date | Date |
| Ship Date | Date |
| Segment | Text |
| Category | Text |
| Sub-Category | Text |

Date columns were formatted appropriately to ensure correct date-based analysis.

---

### 4. Formatting Text Columns

Text values were standardized to maintain consistency throughout the dataset.

The following columns were formatted:

* Segment
* Category
* Sub-Category

The **Capitalize Each Word** transformation was applied wherever required.

### Example:

| Before | After |
|---|---|
| consumer | Consumer |
| furniture | Furniture |
| office supplies | Office Supplies |

---

### 5. Creating Custom Columns

Custom columns were created using the **Power Query Editor** to generate additional information from the existing dataset.

These transformations helped in preparing the data for further analysis and reporting.

---

### 6. Duplicating Columns

Required columns were duplicated before applying further transformations.

This allowed the original data to be preserved while creating modified versions for analysis.

---

### 7. Renaming Columns

The duplicated and newly created columns were renamed with meaningful names.

This improved the readability and organization of the transformed dataset.

---

### 8. Calculating Week of the Year

A new column was created to determine the **week of the year** from the date information.

This can be used for:

* Weekly sales analysis
* Comparing sales performance
* Identifying weekly trends
* Time-based reporting

---

### 9. Removing Unnecessary Columns

Unnecessary columns were removed after completing the required transformations.

The final dataset contains the relevant fields required for further analysis and visualization.

---

## 🔄 Transformation Workflow

```text
Raw Superstore CSV Data
          ↓
Import into Power BI
          ↓
Promote Headers
          ↓
Change Data Types
          ↓
Apply Date Formatting
          ↓
Standardize Text Values
          ↓
Create Custom Columns
          ↓
Duplicate and Rename Columns
          ↓
Calculate Week of the Year
          ↓
Remove Unnecessary Columns
          ↓
Cleaned and Transformed Dataset
```

👩‍💻 Author

Madhumidha E

Project: Superstore Sales Data Cleaning and Transformation
Tool: Microsoft Power BI
