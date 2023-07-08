# meta_database_engineer_capstone


## Exercise: Create an ER diagram data model and implement it in MySQL

### Task 1
 Implementing task 1 as mentioned at https://www.coursera.org/learn/database-engineer-capstone/supplement/o3pao/exercise-create-an-er-diagram-data-model-and-implement-it-in-mysql.

 In this task, a normalized ER diagram is created (that adheres to 1NF, 2NF and 3NF) with relevant relationships to meet the data requirements of Little Lemon which is depicted at [ER_diagram.png](ER_diagram.png).
 
### Task 2 and 3
For implementation of the Little Lemon data model inside MySQL server, tables creation and databases show
[LittleLemonDB.sql](LittleLemonDB.sql) can be utilized. 

## Exercise: Create a virtual table to summarize data

### Task 1
In the first task, Little Lemon need you to create a virtual table called OrdersView that focuses on OrderID, Quantity and Cost columns within the Orders table for all orders with a quantity greater than 2.
Implemented with [OrderView.sql](OrderView.sql).

### Task 2
For your second task, Little Lemon need information from four tables on all customers with orders that cost more than $150. Extract the required information from each of the following tables by using the relevant JOIN clause. 
Implemented with [OrderMenu.sql](OrderMenu.sql).

### Task 3
For the third and final task, Little Lemon need you to find all menu items for which more than 2 orders have been placed. You can carry out this task by creating a subquery that lists the menu names from the menus table for any order quantity with more than 2.
Implemented with [MenuName.sql](MenuName.sql).

## Exercise: Create optimized queries to manage and analyze data

### Task 1
In this first task, Little Lemon need you to create a procedure that displays the maximum ordered quantity in the Orders table. 

Creating this procedure will allow Little Lemon to reuse the logic implemented in the procedure easily without retyping the same code over again and again to check the maximum quantity. 
Implemented with [MaxQuantity.sql](MaxQuantity.sql).

### Task 2
In the second task, Little Lemon need you to help them to create a prepared statement called GetOrderDetail. This prepared statement will help to reduce the parsing time of queries. It will also help to secure the database from SQL injections.

The prepared statement should accept one input argument, the CustomerID value, from a variable. 

The statement should return the order id, the quantity and the order cost from the Orders table. 

Once you create the prepared statement, you can create a variable called id and assign it value of 1. 
Implemented with [OrderDetail.sql](OrderDetail.sql).

## Exercise: Create SQL queries to add and update bookings

### Task 1 
In this first task you need to create a new procedure called AddBooking to add a new table booking record.
The procedure should have two input parameters in the form of booking id and booking date. You must also include an UPDATE statement inside the procedure.
Implemented with [AddBooking.sql](AddBooking.sql).

### Task 2
For your second task, Little Lemon need you to create a new procedure called UpdateBooking that they can use to update existing bookings in the booking table.
Implemented with [UpdateBooking.sql](UpdateBooking.sql).

### Task 3
For the third and final task, Little Lemon need you to create a new procedure called CancelBooking that they can use to cancel or remove a booking.

The procedure should have one input parameter in the form of booking id. You must also write a DELETE statement inside the procedure. 
Implemented with [CancelBooking.sql](CancelBooking.sql).

## Exercise: Create interactive dashboard for sales and profits

Dashboards can be found at [dashboard.png](dashboard.png).

## Exercise: Database Client

Rest of the tasks regarding database client are implemented at [database_client.ipynb](database_client.ipynb) jupyter notebook.