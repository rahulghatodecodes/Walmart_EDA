# Walmart Data

Order ID	Order Date	Ship Date	Customer Name	Country	City	State	Postal Code	Region	Category	Sub-Category	Product Name	Sales	Quantity	Discount	Profit


## Objective
- Data Transformation
- Data Modelling
- Data Visualization

## Programming Language & Tools:
- Python: Data Manupulation using Pandas library, Data Computation using Numpy library, Data Visualtion using Matplotlib & Seaborn libraries.
- Jupyter Notebook
- Microsoft SQL Server Management Studio (SSMS)
- Microsoft Power BI

## Tasks: 
1. Using dropna function, getting rid of rows where all the column values are null.
   - walmart.dropna(how = 'all', inplace = True)
2. Using replace function, fixed multiple instances of "country" column.
   - walmart.dropna(how = 'all', inplace = True)
3. In data imputation, replaced the null values of "Sales" column with mean.
   - m = walmart['Sales'].mean()
   - walmart['Sales'].fillna(value=m, inplace=True)
4. Using Order by keyword in SQL Server, extracted the products giving us the highest profit.
   - select customer_name, product_name, state, profit 
   - from Walmart 
   - WHERE state = "California" AND customer_name = "Brosina Hoffman"
   - order by profit DESC limit 4


select customer_name, product_name, state, profit, returned
from Walmart join Return_Order
on order_id = orders

