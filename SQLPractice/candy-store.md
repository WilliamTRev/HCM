# Candy Shop

This is a small exercise to build an inventory table for a candy shop. 

## Instructions

Read each of the following steps and write a script to simulate that instruction in your database. 

1. Create a table named `inventory` with the following fields
   1. ID (number)
   2. name (varchar)
   3. price (number; choose a type that supports at least two decimal places)
   4. description (varchar)
   5. quantity (number)
   

2. Insert the following records to your table so that it looks like the following:

 | ID | NAME | PRICE | DESCRIPTION | QUANTITY|
 | - | - | - | - | - |
 | 1001 | Hershey Bar | 3.45 | A small chocolate bar | 50 |
 | 1002 | Skittles | 3.05 | A bag of rainbow colored candies | 100 |
 | 2003 | Gummy Bears | 5.55 | A large bag of chewy fruit-flavored bears | 48 |
 | 2005 | Sour Gummy Worms | 9.55 | A very large bag of gelatin worms | 20 |
 | 3008 | Lollipop | 2.25 | A hard candy atop a stick | 268 |
 | 9007 | M&Ms | 1.95 | A bag of small chocolate candies | 58 |

3. Run a query to read and display all records in our table


4. A customer has just purchased 2 Hershey Candy Bars. Update the inventory to be 48 now. 

5. Run a query to return only the descriptions of all records in the table. 

6. A customer wants to see all items in your store and their prices. 
Run a query to return the name and price only of all records in the table. 

7. Change the description of the Sour Gummy Worms to be 'A very large, delicious bag of worms'.

8. You've received a shipment of M&Ms just now! Update the quantity to 100. 

9. You are getting a lot of demand for lollipops. Update the price to $2.50. 

10. What is the total cost to purchase all remaining M&Ms in your store?

11. Run a query to return the name and price of the candy item that costs the least amount of money. 

12. Run a query to return the candy item with the largest quantity in inventory. Return just the name and the quantity left. 

13. Run a query to return the 3 most expensive candy items. Return all columns. 

