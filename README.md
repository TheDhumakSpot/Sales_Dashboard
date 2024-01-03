# Sales Dashboard using MySQL Database to store data and Looker Studio and PowerBI for Report

Reference : codebasics yt

Data source : db_dumb.sql ( [https://codebasics.io/resources/sales...)](https://codebasics.io/resources/sales-insights-data-analysis-project)https://codebasics.io/resources/sales-insights-data-analysis-project )

# Import Data to MySQL Workbench

![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/76780aa4-7be0-4935-82e2-480ab6262234)

# Analyse Data

View All Tables and Clean Data

( eg: Sales amount should be positive , No NULL values , currency should be in one form (USD or INR) etc.)

SELECT * FROM transactions ;

![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/41b7da35-a2a8-487e-916e-8e3cabe7fb81)


JOIN tables based on a common key (column)
Since there are multiple common keys, you can join multiple tables together

SELECT *
FROM transactions
JOIN customers ON transactions.customer_code = customers.customer_code
JOIN products ON transactions.product_code = products.product_code
JOIN markets ON transactions.market_code = markets.markets_code
JOIN date ON transactions.order_date = date.date;

![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/f4be3047-7a41-4cc5-a735-63fa44325e9f)

# CSV file and Google Sheets
- Export Data from MySQL to 'CSV file'
- From CSV file convert to  'Google Sheets'
 https://docs.google.com/spreadsheets/d/1_d7wAgR6SJbS38GQsjNRDQ1oaXxJCASWRbLa_QMBiRk/edit#gid=886642676

# Looker Studio

Looker Studio is a free tool that turns your data into informative, easy to read, easy to share, and fully customizable dashboards and reports.


# Dashboard using Looker Studio

Import Google Sheets data to 'Looker Studio'
Create Insights from imported data and make a Dashboard

https://lookerstudio.google.com/s/i7hjujjk3Uk
![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/6853471b-72a9-4eea-bee3-4bda83ce1253)

https://lookerstudio.google.com/reporting/bd54bccd-63d8-427d-b27b-94252e1c7cca/page/6yYmD

# Dashboard using PowerBI

- Import Data from MySQL to PowerBI
- Link tables using common column and deplay relationship between them in 'Model View'

![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/ced3258d-4194-425c-bd64-2918592acecb)

- Clean and Analyse Imported Data in 'Table View'
- Make a report

  ![image](https://github.com/TheDhumakSpot/Sales_Dashboard/assets/118016094/49214656-898c-4f94-bf1f-657f6f2e2c6d)


