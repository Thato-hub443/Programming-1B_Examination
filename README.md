MattressApp

A Java project for a local mattress retailer, built in Apache NetBeans. It has two parts:

Question 1: a console application that generates a quarterly sales report for the three top-performing mattress products.
Question 2: a Swing GUI application that processes mattress sales, calculates VAT and commission, and logs each sale to a file.

Both parts include unit tests written with JUnit 5.

Features
Question 1: Product Sales Report (console)
Captures sales for 3 products over 3 months, using a single-dimensional array (product names) and a two-dimensional array (sales per product per month).
Calculates and displays:
Total number of products sold
Average number of products sold per product-month entry
Most popular product (highest total sales)
Calculation logic lives in Product, which implements the IProduct interface.
Printing is handled separately by the PrintProduct class.
Question 2: Product App (GUI)
Captures the customer name, product (combo box) and price.
Calculates:
VAT: 15% of the price
Commission: 5% of the price
Total: price + VAT + commission
Shows the result in a message dialog and appends it to data.txt.
Menu system:
File > Exit: closes the application
Tools > Process: runs the same logic as the PROCESS button
Tools > Clear: clears the text boxes and resets the combo box to index 0
Calculation logic lives in ProductCalculations, which implements IProductCalculations.
Input validation for an empty name and an invalid or non-positive price.
