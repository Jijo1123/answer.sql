1. Write an SQL query to retrieve the customerName,email and PhoneNumber from the customer table.

SELECT customerName, email, PhoneNumber 
FROM customer;

2. Write an SQL query to retrieve the customerName,email and PhoneNumber from the customer table, where customerAddress is equal to Kisii

SELECT customerName, email, PhoneNumber 
FROM customer 
WHERE customerAddress = 'Kisii';

3. Write an SQL query to retrieve the customerID,TotalAmount from the bills table, where status is equal to unpaid

SELECT customerID, TotalAmount 
FROM bills 
WHERE status = 'unpaid';

4. Write an SQL query to retrieve the customerID,TotalAmount, and CategoryID from the bills table, where status is equal to paid

SELECT customerID, TotalAmount, CategoryID 
FROM bills 
WHERE status = 'paid';

5. Write an SQL query to retrieve the customerID,Status from the bills table, where BillDate is between 2024-11-01 and 2024-11-30

SELECT customerID, Status 
FROM bills 
WHERE BillDate BETWEEN '2024-11-01' AND '2024-11-30';

6. Write an SQL query to retrieve the billID,itemDescription, and LineTotal from the bill_items table ordered LineTotal in descending order

SELECT billID, itemDescription, LineTotal 
FROM bill_items 
ORDER BY LineTotal DESC;

7. Write an SQL query to retrieve the billID,itemDescription, and LineTotal from the bill_items table ordered LineTotal in ascending order

SELECT billID, itemDescription, LineTotal 
FROM bill_items 
ORDER BY LineTotal ASC;

8. Write an SQL query to retrieve the billID,itemDescription, and LineTotal from the bill_items table where LineTotal is greater
than 100 and retreive the result in descending order using billID

SELECT billID, itemDescription, LineTotal 
FROM bill_items 
WHERE LineTotal > 100 
ORDER BY billID DESC;

9. Write an SQL query to retrieve the PaymentAmount,PaymentMethod from the payments table where paymentMethod like '%esa';

SELECT PaymentAmount, PaymentMethod 
FROM payments 
WHERE PaymentMethod LIKE '%esa';

10. Write an SQL query to retrieve the CustomerName,CustomerAddress from the customer table where CustomerAddress like 'Ki%';

SELECT CustomerName, CustomerAddress 
FROM customer 
WHERE CustomerAddress LIKE 'Ki%';
