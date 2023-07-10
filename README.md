# Instacart Grocery Basket Analysis using Python
Analysing Customers Buying Pattern for an e-commerce website
![InstacartLogo](https://www.zdnet.com/a/img/resize/8ec01a9827508dd3cf0b63effdb15798db5ce95b/2020/08/20/c7ff72fc-cd2a-4f7d-b099-d4becd45c564/instacart.jpg?auto=webp&fit=crop&height=900&width=1200)
## About the Company:
Instacart is an American delivery company that operates a grocery delivery and pick-up service in the United States and Canada. The company offers its services via a website and mobile app. The service allows customers to order groceries from participating retailers with the shopping being done by a personal shopper.
_Note: Instacart is a real company that’s made their data available online. However, the contents of this project have been fabricated for the purpose of learning._
## Project Objective:
The instacart stakeholders would like to be able to answer the following key questions: 
* The sales team needs to know what the busiest days of the week and hours of the day are (i.e., the days and times with the most orders) in order to schedule ads at times when there are fewer orders.
* They also want to know whether there are particular times of the day when people spend the most money, as this might inform the type of products they advertise at these times.
* Instacart has a lot of products with different price tags. Marketing and sales want to use simpler price range groupings to help direct their efforts.
* Are there certain types of products that are more popular than others? The marketing and sales teams want to know which departments have the highest frequency of product orders.
* The marketing and sales teams are particularly interested in the different types of customers in their system and how their ordering behaviors differ. For example:
   1. What’s the distribution among users in regards to their brand loyalty (i.e., how often do they return to Instacart)?
   2. Are there differences in ordering habits based on a customer’s loyalty status?
   3. Are there differences in ordering habits based on a customer’s region?
   4. Is there a connection between age and family status in terms of ordering habits?
   5. What different classifications does the demographic information suggest? Age? Income? Certain types of goods? Family status?
   6. What differences can you find in ordering habits of different customer profiles? Consider the price of orders, the frequency of orders, the products customers are ordering, and anything else you can think of.
## Instacart Data Sets:
* [Customer Dataset](https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis)
* [Data Dictionary](https://gist.github.com/jeremystan/c3b39d947d9b88b3ccff3147dbcf6c6b)
## Exploratory Data Analysis
For the analysis I combined all of the separate data files into one single dataframe and to fit the dataframe in my memory I reduced its size to 50% (7.1 GB to 4.4 GB) by type conversion and without loosing any information.
* Saturday and Sunday are the busiest day of the week whereas, Tuesday and Wednesday are comparatively slower days. It is quite a known fact that consumers genrerally go grocery shopping in weekends mostly.

![image](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/assets/135637670/14989f73-90b5-4e7e-824d-b45b35410e57)

![bar](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/bar_combined.png)
![hist](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/hist_ords_hour_combined_24.png)
* Customers order most frequently from the Produce, Dairy & Eggs, Snacks, Beverages, and Frozen departments. Regular order mostly comes from the Pantry, Bakery, Canned Goods, Deli, and Dry Goods & Pasta departments. All of these departments each have over 2.7% of sales. The Meat & Seafood department composes 2.2% of total sales however the mean price per item ordered from this department is roughly twice the value of other departments.
![bar](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/bar_top_depts.png)
* As part of analysis products have been grouped as price <= 5 : 'Low range product', price > 5 and <= 15 : 'Mid range product', price > 15: 'High range product'.  ![coulmnchart](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/bar_norm_dept_loyalty.png)
 ![pie](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/pie_price_range1.png)
* The age of Instacart customers and the corresponding count of dependents they have were examined, and it was found that the distribution of dependents remains consistent across different age groups. There is no noticeable trend or significant variation observed.
![graph](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/age_dependants_connection_combined.png)
* The scatterplot shows the income in relation to customer's ages in 10 year increments. It can be seen that a majority of the customer's make below 200K whereas the income of 60+ yrs is around 600K. This can be supported by a fact that income of any individual increase with increase in its level of experience that is directly proportional to age.
![image](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/income_scatterplot_combined.png)
* Customers in the lowest income bracket order items 4.2% less then their proportion of the customer base.
* Customers in the middle income bracket order items 2.6% more then their proportion of the customer base.
* Customers in the highest income bracket order items 1.6% more then their proportion of the customer base increase with increase in its level of experience that is directly proportional to age.
![image](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/pie_user_income.png)
![img](https://github.com/malvika-mall/Instacart-Grocery-Basket-Analysis-using-Python/blob/main/03%20Analysis/Visualizations/pie_orders_income.png)
## Analysis Criteria
* Project folder follows industry standards in terms of structure and naming conventions.
* Analysis has been conducted using Jupyter notebooks and the Anaconda libraries manager.
* Analysis has been conducted using Python and relevant libraries (pandas, NumPy, os, matplotlib, scipy, and seaborn).
