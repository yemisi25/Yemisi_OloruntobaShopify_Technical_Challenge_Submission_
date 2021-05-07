# Yemisi_OloruntobaShopify_Technical_Challenge_Submission_
Question 1
On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

Think about what could be going wrong with our calculation. Think about a better way to evaluate this data.
What metric would you report for this dataset?
What is its value?
Answers:
The incorrect AOV calculation of $3145.13 was most likely arrived at by mistakenly calculating the total_items with the count() function instead of sum(). Whereas count() will only provide the total count of the number of rows, sum() will more accurately provide the AOV value by adding together all of the values in the total_items column.

To determine the correct Average Order Value (AOV), the reporting metrics are the respective sums of both 'order_amount' and 'total_items':

oa_sum = data_df['order_amount'].sum()
ti_sum = data_df['total_items'].sum()

Next divide the total order amount (oa_sum) by the total items amount (ti_sum):
AOV = oa_sum/ti_sum

The Average Order Value (AOV) is: $357.92


Question 2.
For this question you’ll need to use SQL. Follow this link (https://www.w3schools.com/SQL/TRYSQL.ASP?FILENAME=TRYSQL_SELECT_ALL) to access the data set required for the challenge. Please use queries to answer the following questions. Paste your queries along with your final numerical answers below.

How many orders were shipped by Speedy Express in total?\
What is the last name of the employee with the most orders?\
What product was ordered the most by customers in Germany?\
Answers:
How many orders were shipped by Speedy Express in total? 54

What is the last name of the employee with the most orders?

Employee: Peacock
Most orders: 40

What product was ordered the most by customers in Germany?
 VIEW CODE THROUGH LINK- https://docs.google.com/document/d/11okNiLLdPwpXuS_wTwFkgrzLd0M_1ln4bqQMDIm7J9w/edit?usp=sharing
 
Product: Camembert Pierrot
Quantity: 40
Orders: 300
TotalOrdered: 12000
