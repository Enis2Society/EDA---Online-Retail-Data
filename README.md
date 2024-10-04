# EDA---Online-Retail-Data
Showcase of a simple Exploratory Data Analysis of Online Retail Data 

# Overview
This project focuses on performing an Exploratory Data Analysis (EDA) on a dataset to uncover insights and trends. The project involves various steps including data cleaning, transformation, and visualization. The dataset used in this analysis contains information such as transactions, customer details, and product sales.

# Steps Covered in the EDA:
1. Data Import
We started by importing the dataset (OnlineRetail.xlsx) into a pandas DataFrame using read_csv.
Specified encoding (ISO-8859-1) to avoid any character encoding issues.

2. Initial Data Inspection
Used head() to display the first few rows of the dataset.
The info() function provided column types and non-null counts, while describe() provided summary statistics for numerical columns.

3. Handling Missing Data
Checked for missing values using isnull().sum().
Rows with missing 'CustomerID' were removed as customer analysis requires complete data.

4. Data Type Conversion
Converted the 'InvoiceDate' column to datetime format to enable time series analysis.

5. Dealing with Negative Values
Negative values in 'Quantity' were identified as cancellations. These rows were flagged for further analysis.

6. Feature Engineering: Total Price
Created a new column TotalPrice calculated as Quantity * UnitPrice for each transaction.

7. Data Visualization

8. 
a. Revenue by Country
Grouped the data by country and plotted the total revenue per country using a bar chart.

b. Top 10 Products by Sales
Identified the top 10 best-selling products and visualized them using a bar chart.

c. Sales Trend Over Time
Resampled the data on a monthly basis to show the sales trend over time.

d. Purchases per Customer
Analyzed customer purchasing behavior and visualized the top 10 customers based on total revenue.

9. Cluster Analysis
Clustered customers based on total revenue and the number of purchases for customer segmentation.

10. Product Cancellations
Analyzed products with the most cancellations and visualized the top 10 products with the highest cancellation rates.

11. Revenue Analysis by Country
Visualized the top 10 countries with the highest revenue using bar charts.
Key Insights:
The majority of sales come from the UK, with significant peaks in November and December.
Some customers are responsible for a large portion of total sales, indicating opportunities for customer retention strategies.
Certain products show high cancellation rates, warranting further investigation.
Technologies Used:
Python: Core programming language
Pandas: Data manipulation and analysis
Matplotlib: Data visualization
Seaborn: Statistical data visualization
Jupyter Notebook: Development environment

License:
This project is licensed under the MIT License - see the LICENSE file for details.

Credits:
Data sourced from a publicly available dataset.
