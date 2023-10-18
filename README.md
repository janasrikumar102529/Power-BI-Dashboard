# SQL-Power-BI-Dashboard-Project

KEY INSIGHTS:

Sales Trend Analysis for Brick & Mortar Business | Power BI | SQL

•	Designed a comprehensive Power BI sales insights dashboard for Atliq hardware, using SQL for data manipulation.

•	Transformed raw sales data into an intuitive dashboard, enabling in-depth analysis of trends.

•	Empowered users to make informed decisions, potentially driving a 7% revenue surge in the upcoming quarter.

----------------------------------------------------------------

Data cleaning using - Mysql

Queries:

use sales;
select sum(transactions.sales_amount) from transactions
join date
on transactions.order_date = date.date
where year = '2020';

select distinct(currency) from transactions;
select count(*)
from transactions
where currency = 'INR\r';

select count(*)
from transactions
where currency = 'INR';

select count(*)
from transactions
where currency = 'USD';

select *
from transactions
where currency = 'USD\r' or currency ='USD';

select sum(transactions.sales_amount) from transactions
join date
on transactions.order_date = date.date
where year = '2020' and month_name = 'January' and (currency = 'INR\r' or currency = 'USD\r');

---------------------------------------------------------------------------------------------

Different DAX Functions - Power BI

SUM()

DIVIDE()

CALCULATE()

GENERATESERIES()

SELECTDVALUE()

These are the differnt DAX functions used to measure data.
