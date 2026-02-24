                              SALES DATA SET

Introduction
This program is a Sales Analytics Tool designed to automate the calculation and evaluation of product revenue. Using the NumPy library, it transitions from standard Python list processing to vectorized operations, which allows for high-speed mathematical computations. The primary goal is to take raw quantity and price inputs and transform them into actionable financial insights.

Dataset Overview
The dataset for this program is generated dynamically through user input. It consists of two primary independent variables:
•	Quantity ($q$): The number of units sold for each product (Float).
•	Price ($p$): The cost per individual unit (Float).
These inputs are stored in NumPy arrays ($q\_arr$ and $p\_arr$), which serve as a structured, one-dimensional data matrix. The dependent variable, Sales, is derived by calculating the product of these two arrays. 

Methodology
The program follows a linear computational pipeline:
1.	Initialization: The user defines the number of products ($n$), establishing the size of the arrays.
2.	Data Collection: List comprehensions are used to efficiently collect user inputs for both quantities and prices.
3.	Vectorization: Lists are converted into NumPy arrays. Unlike standard Python lists, these arrays support element-wise multiplication, meaning q_arr * p_arr multiplies corresponding index values instantly without a manual for loop.
4.	Slicing: The program utilizes array slicing ([:3]) to isolate a subset of the results for quick viewing.

 Statistical Analysis
To understand the distribution of sales, the program applies four key statistical measures:
•	Total Revenue ($\sum$): The sum of all sales values.
•	Arithmetic Mean ($\mu$): The average sale value per product, calculated as:
$$\mu = \frac{1}{n} \sum_{i=1}^{n} x_i$$
•	Median: The middle value of the dataset, providing a measure of central tendency that is less sensitive to outliers than the mean.
•	Standard Deviation ($\sigma$): A measure of price volatility or sales variance. It shows how much the sales values deviate from the mean.
 
 Conclusion
The script successfully demonstrates how a few lines of Python code can replace manual spreadsheet calculations. By leveraging NumPy, the program ensures scalability—handling 10 products or 10,000 products with the same logic. It provides a foundational framework that can be expanded into larger business intelligence systems, such as automated invoicing or trend forecasting.
