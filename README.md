# Finance Dashboard

An interactive Power BI dashboard for tracking personal income, expenses, account activity and transaction status, with all amounts in PKR.

## Table of Contents

1. Project Overview
2. Objectives
3. Dashboard Layout
4. KPI Cards
5. Visuals
6. KPI Definitions
7. Interactive Features
8. Key Insights
9. Recommendations
10. Tools and Technologies
11. Data Preparation and Workflow
12. How to Use
13. Repository Structure
14. Future Enhancements

## 1. Project Overview

The Finance Dashboard gives a clear view of where money comes from and where it goes. It combines income and expense transactions into a single report so that spending habits, account usage, payment methods and pending payments can be analyzed quickly.

The dashboard helps answer questions such as:

- How much income was received and how much was spent?
- Is net income positive or negative?
- Which categories take up the largest share of the total amount?
- Which accounts and payment methods are used the most?
- How much money and how many transactions are still pending?
- How do amounts change from month to month?

## 2. Objectives

- Track total income, total expense and net income in one place.
- Break down amounts by category, month, account, payment method and status.
- Compare income and expense for each account.
- Monitor pending and completed transactions.
- Allow filtering by category, month and type for focused analysis.

## 3. Dashboard Layout

The report is a single page with:

- A header with the dashboard title and three filters: Category, Month and Type (Expense / Income buttons).
- A row of six KPI cards.
- Six visuals showing amounts by month, category, account, payment method and status.

## 4. KPI Cards

| KPI | Value |
|-----|-------|
| Total Expense | 2M |
| Total Income | 2M |
| Net Income | -329K |
| Pending Amount | 962K |
| Pending Transactions | 66 |
| Completed Transactions | 184 |

Note: Total Expense and Total Income are both shown rounded to 2M. The exact difference between them is the Net Income of -329K.

## 5. Visuals

| Visual | Chart Type | Description |
|--------|-----------|-------------|
| Amount By Month | Column chart | Shows the total amount for each month, sorted from highest to lowest. November is the highest and April is the lowest. Includes a zoom slider. |
| Amount By Category | Pie chart | Shows each category's share of the total amount, including Salary, Education, Freelance, Rent, Bills, Transport and Other Income. |
| Amount By Category and Type | Clustered column chart | Compares Expense and Income for each account: Main Account, Credit Card and Savings. |
| Expense and Income by Payment Method | Ribbon chart | Compares Expense and Income across the payment methods: Debit Card, Mobile Wallet, Bank Transfer and Cash. |
| Amount By Status | Pie chart | Shows the split between Completed and Pending amounts. |
| Sum of Amount (PKR) by Account and Status | Line chart | Shows the Completed and Pending amounts for each account (Credit Card, Main Account and Savings). |

## 6. KPI Definitions

- Total Expense: sum of the amount of all transactions with type Expense.
- Total Income: sum of the amount of all transactions with type Income.
- Net Income: Total Income minus Total Expense. A negative value means spending is higher than income.
- Pending Amount: sum of the amount of all transactions with status Pending.
- Pending Transactions: number of transactions with status Pending.
- Completed Transactions: number of transactions with status Completed.

## 7. Interactive Features

- Category, Month and Type filters update all KPI cards and visuals.
- Cross-filtering: selecting an item in one visual filters the others.
- A zoom slider on the monthly chart allows closer inspection of specific months.
- Tooltips show exact values and percentages on hover.
- KPI cards update dynamically with every filter selection.

## 8. Key Insights

These insights are based on the unfiltered view of the dashboard and will change when filters are applied.

1. Spending is higher than income. Net income is -329K, which means the total expense exceeds the total income for the period.
2. Salary is the largest category, making up about 28.62% (990K) of the total amount. Education (about 11.68%), Freelance (about 10.22%) and Rent (about 8.13%) follow.
3. Expense is higher than income in every account. The gap is largest in the Credit Card account.
4. Debit Card is the most used payment method by amount, and Cash is the least used.
5. About 72.19% of the total amount is completed and about 27.81% is still pending.
6. There are 66 pending transactions worth 962K, compared with 184 completed transactions.
7. Monthly amounts range from the highest in November to the lowest in April, so activity is not evenly spread across the year.
8. Completed amounts are consistently higher than pending amounts in all three accounts.

## 9. Recommendations

- Review and reduce expenses, since spending currently exceeds income.
- Follow up on the 66 pending transactions to clear the 962K pending amount.
- Review Credit Card spending, as it shows the largest gap between expense and income.
- Set monthly budgets for the major categories such as Education, Rent and Bills.
- Look at the high-spending months, especially November, and plan for them in advance.
- Look for ways to increase income through Freelance and other income sources.

## 10. Tools and Technologies

- Microsoft Power BI Desktop: report design and visualization
- Power Query: data cleaning and transformation
- DAX: measures and KPI calculations

## 11. Data Preparation and Workflow

1. Data collection: load the income and expense transaction data into Power BI.
2. Data cleaning: fix data types, remove duplicates and null values, and standardize text fields in Power Query.
3. Date preparation: create a Month column for time-based analysis.
4. Measures: create DAX measures for Total Expense, Total Income, Net Income, Pending Amount, Pending Transactions and Completed Transactions.
5. Visualization: build the KPI cards and the six visuals.
6. Interactivity: add the Category, Month and Type filters and enable cross-filtering.
7. Validation: check the KPI values against the source data.

## 12. How to Use

1. Clone or download this repository.
2. Install Power BI Desktop, which is free from Microsoft.
3. Open the .pbix file in Power BI Desktop.
4. If asked, update the data source path under Home > Transform data > Data source settings.
5. Click Refresh to load the data.
6. Use the Category, Month and Type filters to explore the dashboard.

## 13. Repository Structure

- Finance_Dashboard.pbix : Power BI report file
- data/ : source dataset files
- README.md : project documentation

## 14. Future Enhancements

- Add budget vs actual tracking for each category.
- Add a savings goal tracker.
- Add forecasting for monthly income and expenses.
- Add drill-through pages for transaction-level details.
- Add alerts for overspending and overdue pending payments.
- Publish to Power BI Service with scheduled data refresh.
