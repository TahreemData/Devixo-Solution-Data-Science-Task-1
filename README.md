# Devixo-Solution-Data-Science-Task-1
Superstore Sales Exploratory Data Analysis (EDA)
Devixo Solutions — Data Science Internship | Task 01

A Python-based exploratory data analysis project that investigates Superstore sales data to uncover patterns in sales, profit, product categories, customer segments, regions, discounts, and shipping time.
Table of Contents
- Project Overview
- Objectives
- Dataset
- Tools and Libraries
- Key Analyses
- Repository Structure
- Getting Started
- Reported Metrics
- Data Quality Notes
- Recommendations
- Conclusion
Project Overview
Exploratory Data Analysis (EDA) is used to understand a dataset before drawing conclusions or building models. In this project, Python libraries are used to inspect and clean the Superstore data, calculate summary statistics, explore relationships, and create visualizations that can support business decisions.
Objectives
- Understand the dataset structure, columns, and data types.
- Detect missing values and duplicate records.
- Prepare date and numeric fields for analysis.
- Summarize sales, profit, quantity, discounts, orders, and customers when the corresponding source columns are available.
- Compare performance across categories, sub-categories, regions, states, customer segments, and products.
- Examine monthly sales patterns and shipping duration.
- Visualize numerical distributions, relationships, and potential outliers.
- Translate the verified results into business insights and recommendations.
Dataset
The analysis uses a Superstore CSV file, expected to be named:
Depending on the dataset version, columns may include:
- Order information: Order ID, Order Date, Ship Date, Ship Mode
- Customer information: Customer ID, Customer Name, Segment
- Location: Country, City, State, Postal Code, Region
- Product information: Product ID, Category, Sub-Category, Product Name
- Metrics: Sales, Quantity, Discount, Profit
Dataset note: Superstore datasets can vary by source and version. Analyses involving Profit, Quantity, or Discount should only be run when those columns contain valid values from the original data. Do not create random or guessed values to fill missing business metrics.
Tools and Libraries
- Python — analysis and scripting
- Pandas — loading, cleaning, grouping, and summarizing data
- NumPy — numerical operations
- Matplotlib — charts and visualizations
- Seaborn — statistical plots and correlation heatmaps
- Jupyter Notebook — documenting and running the analysis
Key Analyses
The notebook may include the following analyses, depending on which columns are available:
1. Dataset preview, dimensions, data types, and descriptive statistics
2. Missing-value and duplicate checks
3. Sales distribution histogram with KDE curve
4. Monthly sales trends and area chart by category
5. Sales and profit by category and sub-category
6. Sales and profit by region and state
7. Sales by customer segment and shipping mode
8. Top customers and products by sales
9. Products with negative total profit
10. Quantity and discount analysis
11. Shipping duration calculated from order and ship dates
12. Correlation heatmap and pairplot for numerical variables
13. Violin plots and boxplots to examine distributions and potential outliers
Repository Structure
A suggested GitHub repository layout is:
superstore-sales-eda/
├── README.md
├── Superstore_EDA.ipynb
├── Sample - Superstore.csv
└── outputs/
    ├── Superstore_Cleaned.csv
    ├── EDA_Summary.csv
    ├── Category_Analysis.csv
    ├── Region_Analysis.csv
    └── charts/
Reported Metrics
The following figures were reported during the current analysis. Recalculate and verify them against the final dataset before submitting or publishing the repository.
Metric	Reported value
Total Sales	1,064,046.0419
Total Profit	120,000.7178
Total Quantity Sold	17,407
Average Discount	0.1566863 (approximately 15.67%)
Profit Margin	Approximately 11.28%


Profit margin is calculated as total profit divided by total sales, multiplied by 100. These metrics describe the values in the analyzed file and may differ from other versions of the Superstore dataset.
Data Quality Notes
- Verify that Sales, Profit, Quantity, and Discount contain real source values.
- Adding an empty column does not restore missing information.
- Do not replace unknown values with zero or random numbers unless the data meaning justifies that treatment.
- Inspect invalid or missing dates before calculating monthly trends or shipping duration.
- Investigate outliers instead of automatically deleting them.
- Treat correlations as associations; correlation alone does not establish causation.
- Base business conclusions on outputs from the complete, verified dataset.
Recommendations
Use the completed analysis to investigate the following opportunities:
- Maintain availability for products and categories with strong sales demand.
- Compare profit as well as sales when evaluating product and regional performance.
- Review discount policies if higher discounts coincide with lower profit.
- Investigate products that show repeated or substantial losses.
- Use monthly trends to support inventory and promotional planning.
- Improve data quality checks so that business reporting is reliable.
These are general recommendations. Prioritize them only when the project's actual outputs support them.
Conclusion
This project demonstrates how Python can be used to inspect, clean, summarize, and visualize retail sales data. The analysis explores patterns across product categories, regions, customer segments, sales trends, and numerical variables. The resulting findings can support further investigation into profitability, discounts, product performance, and shipping operations.
Internship
Organization: Devixo Solutions
Program: Data Science Internship
Task: Task 01 — Exploratory Data Analysis (EDA)
