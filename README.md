# Food-Stores-Analysis

### Introduction:
###### We have a data about sales for Food Stores in Egypt, data contains 8 Columns and 8035 Rows

###### I started with data analysis process as follow:
####### 1)	Identifying data and measures (business Metrix) to use
####### 2)	Clean data (incorrect data format – incorrect data type – create custom columns – create columns from selection – remove duplicates – recorrect cashier names ####### based on their cashier number – merge columns – fix datetime and date data)
####### 3)	 Analyze data and create useful measures that indicates findings
####### 4)	Create charts based on the measures we used and design a suitable dashboard

### Identifying the data:
###### Store: sales stores in Egypt
###### Source: kind of product sold in these stores
###### ReferenceNumber: Indicates the specific order number and should be unique
###### Value: product price
###### CreatedAtStore: date and time of creating and put the product in our store
###### DueDate: last date and time for selling the product
###### CashedDate: date and time of selling the product
###### Cashier Number: a unique Id for each cashier that used as a primary Key referee to a specific cashier
###### Cashier Name: cashier Name


### Used Measures with details
###### Sales by days
###### Count number of products sold
###### Number of orders sold by cashiers
###### Sales amount
###### Number of orders
###### Sales amount for each store
###### Sales amount for each store
###### Sales for each source (Product)
###### Selling hours for each day
###### hours and number of orders
###### average time in store for each cashier
###### sales outliers detection for each cashier
###### duplicates slicer
###### drill-through option


### Discuss Data Cleaning and Preparing

###### First: checking data for duplicates
###### I found duplicates on the cashiers table (more than 7000 duplicated names and cashiers’ numbers)
###### I found duplicates on the sales table (less than 5 duplicated rows)

###### Second: Checking for incorrect cashiers’ numbers and incorrect names
###### I found that there are incorrect cashiers’ numbers and names for more than one cahier (Ahmed Hasan 791 – m.abdeltawab 2971 – Y.Hany 2992 – and 3 other cahiers) ###### I fixed them based on using the average numbers of names repeated for each cashier number

###### Third: removing rows with errors
###### I removed 2 rows with errors on cells values that detected on Power query editor

###### Fourth: fixing date format:
###### Split datetime columns to date columns and time columns also creating a column with the start hour for cashed date column to be used on our measures in the dashboard

###### Fifth: creating columns based on selection and custom columns
###### Sixth: creating duplicate and unique column
###### Using Dax to create a specific column that detect whether the order is duplicated or not

###### Seventh: creating required measures:
###### I created some measure to be used in our measures

###### Eighth: building the data model
###### After cleaning the data, we are able to connect the fact table (Sales) and the dim table (Cashiers) in a [Many to One] Relationship that will smooth our dashboard work, filters, and connections among the different charts in the dashboard

