# sql_cert_practice
Some queries written using SSMS as practice for LCC SQL Certification Exam. 

This query uses multiple joins to connect a series of separate tables by their Primary and Foreign Keys to get a comprehensive view of the database’s information. You can see we have some inconsistencies within the column titles, such as CustId being used on the Customer tables and CustomerId being used on the OrderId table - not a big problem by any means, but something to be tided up. 

I ordered the resulting table by Country and Order Date in descending order to make it easier to read. 


![1](https://github.com/Tkurylo/sql_cert_practice-/assets/125916229/6ca970e9-9dfa-48f5-ad85-600d6a07fc91)



In this query I switched the Left join, as it was unnecessary. Afterwards, I decided I wanted to filter the results to get a specific set of data. To do so I included a WHERE clause with OR logical operators to restrict the results to those suppliers in three different countries. I then used an AND operator to include the additional filter with a binary value of 1 in the ‘isDiscontinued’ column to display only discontinued products. Finally, I used ORDER BY to order the results by OrderDate.

![2](https://github.com/Tkurylo/sql_cert_practice-/assets/125916229/075cab81-d35f-455f-9233-a7e64cad5b4b)


In this query I used some aggregate functions to get some basic stats on the UnitPrice and assigned them aliases, while joining the Supplier table to get the CompanyName. 


![3](https://github.com/Tkurylo/sql_cert_practice-/assets/125916229/eebb5f68-1ddc-4ffc-92dc-a36da7a93562)
