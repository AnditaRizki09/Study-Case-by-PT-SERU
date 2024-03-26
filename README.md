I have a file named Power BI for the study case from PT SERU. Below are the steps I followed to create a framework for data visualization:

Step 1: Understanding the Data
- I chose two tables over three tables as the table "budget" was too ambiguous for analysis.

Step 2: Data Cleaning
- I checked the data type as it is important while using it with charts.
- I cleaned blank rows which contained one row of blank space.

Step 3: Connecting the Tables
- I connected the table details and order with order ID as the primary key.

Step 4: Data Visualization
- I made the first matrix "Sales by Segment" using the X-axis with the column Order Date[Month] and the Y-axis with the column Amount[Sum].
- I made the second matrix "Orders by Month" using the X-axis with the column Order Date[Month] and the Y-axis with the column Quantity[Sum].
- I made the third matrix "Total Category Growth by Year" by using the formula:
"Total Category Growth per Year = (CALCULATE(SUM(Details_1[Amount]),YEAR(Orders_1[Order Date])=2023)-CALCULATE(SUM(Details_1[Amount]),YEAR(Orders_1[Order Date])=2022))/CALCULATE(SUM(Details_1[Amount]),YEAR(Orders_1[Order Date])=2022)".
- I made the fourth matrix "Total Segment Growth by Year" using the X-axis with the column Sub-Category and the Y-axis with the column Total Category Growth per Year.
- I made the fifth matrix "Payment Mode" to gain insight into what payment method our customers usually use. We can use this information to determine payment method preferences for our promotions.
- I made the last matrix scorecard containing total sales and total profit.
- Finally, I used filters to inform the interactive dashboard.
