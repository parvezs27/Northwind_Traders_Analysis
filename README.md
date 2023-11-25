# Northwind_Traders_Analysis# games_store_analysis
Overview of Northwind Traders.
# Games Store Analysis
## Context
We are working as Data Analysts for Northwind Traders, a global import and export company that specializes in supplying high-quality gourmet food products to restaurants, cafes, and specialty food retailers globally. The executive team has asked us to build a high level KPI dashboard, allowing the executive team to quickly understand the company's performance in key areas, including:
- Sales trends
- Product performance
- Key customers
- Shipping costs
Our manager has requested insights and recommendations to share with the VP's.
The data has been cleaned by the engineers  and is ready for analysis

Lets start by joining our tables together

Orders table will be joined to order details table via the orderID column (primary and foreign key). 
Customers table iwll be joined to orders table via the the customerID column (primary and foreign key). 
The products table wil be joined to the order details table via the productID column (primary and foreign key). 
The categories table will be joine dto the products table via the categoryID column (primary and foreign key). 
The employees table will be joined to the orders table via the employeeid column (primary and foreign key). 
The shippers table will be joined to the orders table via the shipperid colum n(primary and foreign key). 
The employees table will also be joined to itself (self-join), this is where rows from the employees table will be joined to itself. A good way to visualise this is to create another copy of the table and then go through the join proess row by row. Here we'll be doing a left join, to make sure the rows witch matching values in the employee id and reports to column are captured, as well as all the rows in the first employees table regardless of a matching value or not, in this case it's Andrew Fuller 
![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/b17e02d1-5388-4b3c-a2ac-a7750681f535)
Now lets QA our work and make sure our join has worked, we'll change reports to to manager. we can see that the join has worked and the managers are matching the mployees as per our data set
![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/b323b66b-6e9f-403a-89db-e31d533fa141)


CALCULATED FIELDS we created

Total orders
![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/9e8ac972-1e93-4d23-9bec-e56dea642ae2)





tiled objects ![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/fa50b13d-98c4-4e5d-b638-58cfd48704de)

get rid of it ![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/0ef32656-2582-4504-acab-7011ce300080)

first insert a vertical container, then a blank, make sure to do floating objects, tiled make the item hierarchy messy to work with, a nightmare for yourself and anyone else who would want to work with the dashboard and make changes.
floating containers make it easier to see which objects are in which containers, you'll see thatin a bit, insert 2 blanks that act as placeholders, your dashboard will be looking like this
![image](https://github.com/parvezs27/Northwind_Traders_Analysis/assets/107979122/69e77aad-e203-4f95-a5f2-68f20b8eb28c)







We are employed as Data Analysts for a gaming business with 349 brick & mortar stores nationwide. Business executives have asked us to provide them with dashboards showing how the business is performing to help them with business decisions. Executives have advised us that they don't have any dashboards currently and haven't provided us with any direction on what that they would like to be delivered. This is not an uncommon scenario in the real world, where a business unit doesn't have any dashboards or any reports that have been created. In these situations is upto us, as Data Analysts, to create these dashboards and reports. It's also not uncommon where you get some guidenace from stakeholders, but no further details on what report they would like specifically, which metrics they would like to see or any examples or mock ups of what they're after. Other times, you may get guidance from stakeholders, however as an **analyst**, it's upto you to understand the business, the business situation, what the stakeholders need, the best way to get it to them, anticipating what they might need down the track and preparing for it. 

## Business & Data Information
Here's the information we have on hand currently:
- The business launched on the 01/01/2020, assuming today is the 01/01/2023, we have we have 3 full years of data, with the last full day of data being 31/12/2023.
- The business sells video games and gaming systems, and operates as brick and mortar only with 349 stores nationwide
- We have been given 2 XLSX files aggregated to certain levels, with rather cryptic names. These files have been provided to us by the Data Engineering team, who have mentioned the data is clean and ready to work with in Tableau. 
  - [store_wbr_trans_data_20230424.xlsx](https://shorturl.at/dikmp) - This dataset contains store revenue, transactions and unit sales data, segmented by transaction date and store number. 
  - [sales_by_date_and_prod_cat.xlsx](https://shorturl.at/chGN4) - This dataset contans company-wide revenue, transactions and unit sales data, segemented by transaction date and product category. 

## Business Tasks
Here are our tasks as a Data Analyst based on the information provided.
