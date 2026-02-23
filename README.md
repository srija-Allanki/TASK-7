📊 Basic Sales Summary using SQLite & Python
📌 Project Objective

This project demonstrates how to use SQL inside Python to analyze simple sales data.
It calculates total quantity sold and total revenue, then visualizes the results using a bar chart.

🛠 Tools & Technologies

Python

SQLite (built-in database)

Pandas

Matplotlib

Jupyter Notebook

🗂 Database Details

A small SQLite database file sales_data.db is created with one table:

Table: sales
Column	Description
product	product name
quantity	number of items sold
price	price per item
⚙️ Steps Performed
✅ 1. Created SQLite Database

Connected to SQLite and created a sales table.

✅ 2. Inserted Sample Sales Data

Added sample product sales records.

✅ 3. Executed SQL Query

Used SQL to calculate:

total quantity sold

total revenue per product

SELECT 
    product,
    SUM(quantity) AS total_qty,
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
✅ 4. Loaded Data into Pandas

SQL results were loaded into a pandas DataFrame.

✅ 5. Displayed Results

Printed summarized sales data.

✅ 6. Visualized Data

Created a simple bar chart showing revenue by product.

📊 Sample Output
Product	Total Quantity	Revenue
Laptop	8	400000
Mobile	15	300000
Tablet	7	210000
Headphones	15	22500
📈 Visualization

A bar chart was generated to compare revenue across products.

📁 Saved as: sales_chart.png

🎯 Key Learnings

✔ Writing basic SQL queries
✔ Connecting SQLite database with Python
✔ Importing SQL results into Pandas
✔ Performing simple data summaries
✔ Creating basic data visualizations

🚀 Future Improvements

Add more products & records

Analyze monthly sales trends

Create interactive dashboards

Use real-world datasets

✅ Conclusion

This task demonstrates how Python and SQL can work together to perform basic sales analysis and visualization, providing a strong foundation for data analytics projects.
