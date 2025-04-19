# week7-pythonassignment
1. Data Generation & Loading
Process: The script generates synthetic sales data programmatically

Features Created:

date: Random dates from Jan-Mar 2023

product: 4 categories (Electronics, Clothing, Home, Beauty)

region: 4 sales regions

sales: Normally distributed values (
500
−
500−1500 range)

customers: Random customer visits (50-300)

Imperfections Added:

Missing values in sales (6 entries)

Missing customer data (6 entries)

Missing product categories (3 entries)

Error Handling: If data generation fails, script exits gracefully

2. Data Cleaning
Missing Value Treatment:

Sales: Filled with median sales value

Customers: Filled with mean customer visits

Products: Rows with missing categories dropped

Data Type Conversion: Automatic type inference by pandas

3. Exploratory Analysis
Initial Inspection:

First 5 rows displayed

Dataset shape (rows × columns)

Data types verification

Missing Values Report:

Shows count of missing values per column

Displays cleaning results

4. Statistical Analysis
Basic Statistics:

Count, mean, std, min/max for sales/customers

Product Analysis:

Mean, median, and count per product category

Sales performance comparison

5. Visualizations
a. Daily Sales Trend (Line Chart)

Aggregates daily sales totals

Shows temporal patterns and outliers

Reveals weekly cyclical patterns

b. Product Performance (Bar Chart)

Horizontal bars for easy comparison

Viridis color scheme for accessibility

Sorted by average sales

c. Sales Distribution (Histogram)

Shows frequency of sales amounts

Normal distribution verification

Red dashed line marks mean value

d. Customer-Sales Relationship (Scatter Plot)

Multivariate analysis (sales vs customers)

Color-coded by region

Bubble size represents sales amount

Reveals correlation patterns

6. Key Findings
Automatically generated insights:

Data quality issues addressed

Top performing product category

Sales distribution characteristics

Customer-sales correlation

Regional performance differences

Temporal patterns in sales


Expected Output
Terminal Output:

Dataset preview

Structural information

Missing value reports

Statistical summaries

Business insights

Visual Output:

Four sequential pop-up windows with charts

Interactive matplotlib figures

Exportable visualization files

Customization Options
Data Generation:

Modify date ranges in pd.date_range()

Adjust sales/customer distributions

Add new product categories/regions

Analysis:

Change grouping columns

Add percentiles to describe()

Calculate new metrics (ROI, conversion rates)

Visualization:

Modify color palettes

Adjust figure sizes

Add trend lines

Change chart types

Error Recovery
Data Generation Errors: Script exits with error code

Visualization Errors: Skips failed plots but continues execution

Common Failures Handled:

Missing dependencies

Display driver issues

Memory allocation problems
