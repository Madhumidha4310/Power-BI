# 📊 Shopify Stock - Financial Analytics Dashboard

## 📌 Project Overview

This project is an interactive **Financial Analytics Dashboard developed using Microsoft Power BI**.

The dashboard analyzes **Shopify stock price and trading volume data** and provides a visual view of stock performance across different time periods.

The report focuses on important financial metrics such as the latest closing price, average closing price, previous-year closing price, year-to-date closing price, previous-month closing price, and trading volume.

## 🎯 Project Objectives

The main objectives of this project are:

* Analyze Shopify stock price performance.
* Track the latest closing price.
* Calculate and display the average closing price.
* Compare current performance with previous-year values.
* Analyze year-to-date closing performance.
* Compare current values with previous-month closing values.
* Analyze stock performance by year and quarter.
* Monitor total trading volume.
* Present financial information through an interactive Power BI dashboard.

## 🛠️ Tools & Technologies

* **Microsoft Power BI**
* **Power Query**
* **DAX**
* Data Modeling
* Data Visualization

## 📊 Dashboard Title

### Shopify Stock - Financial Analytics Dashboard

The dashboard contains KPI cards, a date filter, charts, and a detailed table for analyzing Shopify stock performance.

## 📌 Key Performance Indicators

The dashboard contains the following KPI cards:

### 1. Latest Close

Displays the **latest closing price** of Shopify stock.

### 2. Average Close

Displays the **average closing price**.

### 3. Close LY

Represents the closing value from the **previous year (LY)**.

### 4. Close YTD

Displays the **year-to-date closing value**.

### 5. Trading Volume

Displays the total stock **trading volume**.

## 🎛️ Interactive Date Filter

The dashboard includes a date hierarchy slicer.

Users can analyze the data by:

* Year
* Quarter
* Month
* Day

This allows the dashboard to be explored at different levels of time.

## 📈 Dashboard Visualizations

### 1. Stock Performance by Quarter and Year

A **Line Chart** is used to analyze stock-related measures across:

* Quarter
* Year

The chart includes:

* Average Close
* Close LY
* Close Previous Month
* Close YTD
* Latest Close

This allows users to compare multiple financial measures across different time periods.

### 2. Average Closing Price by Quarter

A **Pie Chart** shows the distribution of the **Average Close** across different quarters.

This provides a visual representation of quarterly average closing-price values.

### 3. Year-wise Closing Price Analysis

A **Column Chart** compares stock performance across different years using:

* Average Close
* Latest Close

This helps visualize changes in Shopify's closing price over the available years.

### 4. Year-wise YTD and Previous Month Comparison

A **Clustered Bar Chart** compares:

* Close YTD
* Close Previous Month

across different years.

This provides a comparison between year-to-date performance and previous-month closing values.

### 5. Detailed Stock Table

A **Matrix/Table visual** provides date-level information using:

* Date
* Close LY
* Close YTD
* Average Close
* Latest Close

This allows users to inspect the financial measures in greater detail.

## 📐 Measures Used

The Power BI report contains financial measures including:

```text
Latest close
Avg Close
close LY
close YTD
Close Previous Month
```

These measures are used throughout the KPI cards, charts, and detailed table.

## 📊 Data Used

The report contains a **StockPrice** data entity with stock-related information, including a `volume` field.

A separate **Date** entity is used for time-based analysis, including:

* Date
* Year
* Quarter

The report also contains a **Measure** entity containing the calculated financial measures used throughout the dashboard.

## 🔍 Business Questions Addressed

The dashboard can be used to explore questions such as:

* What is the latest Shopify closing price?
* What is the average closing price?
* How does the current closing performance compare with the previous year?
* What is the year-to-date closing performance?
* How does the closing value compare with the previous month?
* How does Shopify's stock performance vary by year?
* How does the average closing price vary by quarter?
* What is the total trading volume?
* How do different financial measures change over time?

## 📁 Project Structure

```text
PBI 3/
│
├── ShopifySales.pbix
└── Finacial Dashboard.png
└── Stock Modelling.png
└── shopify_stock.csv
└── README.md
```

## 🚀 How to Run the Project

### Step 1: Install Power BI Desktop

Install **Microsoft Power BI Desktop** on your computer.

### Step 2: Open the PBIX File

Open the `.pbix` file using Power BI Desktop.

### Step 3: Explore the Dashboard

Use the date hierarchy filter to explore the data by:

* Year
* Quarter
* Month
* Day

### Step 4: Interact with the Visualizations

Select different data points in the charts to interact with the other dashboard visuals.

## 💡 Project Highlights

* Interactive financial analytics dashboard
* Shopify stock price analysis
* Latest closing price KPI
* Average closing price KPI
* Previous-year comparison
* Year-to-date analysis
* Previous-month comparison
* Quarterly analysis
* Year-wise analysis
* Trading volume analysis
* Interactive date hierarchy
* Detailed financial data table
* Power BI data visualization

## 🎓 Skills Demonstrated

This project demonstrates practical knowledge of:

* Power BI Dashboard Development
* Data Visualization
* Financial Data Analysis
* DAX Measures
* Time-Based Analysis
* KPI Development
* Data Modeling
* Interactive Filters
* Business Intelligence
* Dashboard Design

## 👩‍💻 Author

**Madhumidha**
