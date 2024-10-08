# SQL
---
SQL is Structured Query Language. It's a special programming language that is used to query out a specific information from a data base.  It's also a standard language that's use for storing, manipulating and retrieving of data from a data base. It's a standard language for Relational Database System, it enables a user relate databse and tables.

## TABLE OF CONTENTS
---
[MEANING OF SQL](#meaning-of-sql)
 
 [EXAMPLES OF RDBMS TOOLS](#examples-of-rdbms-tools)
 
[USES OF SQL](#uses-of-sql)
 
 [DATABASE IN SQL](#database-in-sql)
 
 [LANGUAGES IN SQL](#languages-in-sql)

 [SQL OPERATORS](#sql-operators)
 
 [COMMANDS IN SQL AND MEANINGS](#commands-in-sql-and-meanings)
 
 [JOIN IN SQL](#join-in-sql)
 
 [SQL KEYS](#sql-keys)
 
 [SQL CLAUSES](#sql-causes)
 
 [VIEW IN SQL](#view-in-sql)
  
 [SQL CASE WHEN STATEMENT](#sql-case-when-statement)
  
### EXAMPLES OF RDBMS TOOLS
---
- SQL
- ORACLE
- POSTGRESQL
- MYSQL
- INFORMIX
- AZURE SQL
- IBM DB2
- MICROSOFT
- SQLIFE
- MARIADB

### USES OF SQL
---
- SQL can be used to create tables.
- It can be used to retrieve data from the database.
- We can insert record, delete and create new tables and stock procedure.
  
### FOUR DATABASE IN SQL:
---
-	Master
-	Tempdb
- Model
- Msdb
  
### LANGUAGES IN SQL
---
- DDL- Data Definition Language - It is used to create database.DDL changes the structure of the table like creating a table, deleting a table, altering a table, etc. 
All the command of DDL are auto-committed that means it permanently save all the changes in the databas. Different commends under DDL are
  
  1. Create
  2. Truncate
  3. Drop
  4. Alter
  5. Rename
  5. Comment
     
- DQL- Data Query Language - It is used to fetch data from the databse.
  
     - Select
    
- DML- Data Manipulation Language - It is used to update or modify the value of a column in the table.
  DML commands are used to modify the database. It is responsible for all form of 
CHANGES in the database.The command of DML is not auto-committed that means it can't permanently save all 
the changes in the database. They can be rollback.

  1. Insert
  2. Update
  3. Delete
  4. Lock
  5. Call
  6. Explain
  7. Plan
 
- DCL- Data Control Language. DCL commands are used to GRANT and TAKE BACK authority from any database user
  
  1. Grant
  2. Revoke
 
- TCL- Transaction Control Language- TCL commands are used to manage transactions in the database. These are used to manage the changes made by DML 
Statement (INSERT, DELETE and UPDATE only). It also allows statements to be grouped into logical transactions
  
  1. Commit
  2. Roll back
  3. Safe point
  4. Set
  5. Transaction

### SQL OPERATORS
---
- Arithmetic Operators in sql	
1. Addition ‘+’
2. Subtraction  ‘-‘
3. Multiplication ‘x’
4. Division ‘/’
5. Equals to ‘=’
6. Greater than ‘>’
7. Less than ‘<’
8. Percentage ‘%’
  
- Aggregate Operators in sql

1. Minimum ‘Min’
2. Maximum ‘Max’
3. Average ‘Avg’
4. Count ‘Count’
5. Sum ‘Sum’

- Logical Operators in sql

1. And ‘AND’
2. Or ‘OR’
3. On ‘ON’
4. IN ‘IN’
5. Like ‘LIKE’
6. Is-null ‘IS_NULL’

- Special Keywords in sql

1. Select ‘SELECT’
2. Where ‘WHERE’
3. Group by ‘GROUP BY’
4. Order by ‘ORDER BY’
5. Ascending ‘ASC’
6. Descending “DESC’
7. From ‘FROM’
8. As ‘AS’

# DATABASE
---
Database is a collection of related information eg. phone book, shopping list, Todo list, facebook’s userbase.
Databases can be stored in different ways – on paper, on a computer. It's an organized collection of data that's stored and managed in a structured way to allow for easy access. retrievel and manipulation. 

### Advantage of Databases:
- Data Integrity: Ensures accuracy and consistency of data.
- Security: Protects data from unauthorized access and breaches.
- Backup and Recovery: Allows data to be recovered in case of loss or corruption.
- Concurrency: Supports multiple users accessing the database simultaneously.
- Scalability: Ability to handle increasing amounts of data and users without performance degradation.
- Efficient Data Management: Databases are optimized for quick access to large volumes of data, enabling fast retrieval 
of information through queries

### COMMANDS IN SQL AND MEANINGS
---
- SELECT: Is used to query out a result or information from the database.
- GROUP BY: Is used to group an item together in a given query. It is used in aggregate operators.
- IN: Means sub-query returning more than one result.
- WHERE CLAUSE:  Is used to filter for a single result in a given query.
- HAVING CLAUSE: Is used to filter for multiple results in a given query.
- UNION: Is used to append tables together in SQL. 
- EQUALS TO: Means sub-query returning only one result.
- AS: is used to label a column or to give a column name or alias.
- IDENTITY in sql is auto increasing the value. It's use to create auto increment.
  
### JOIN IN SQL
---
Join in sql is used when you want to join two or more columns together on the common
column between the two of them. SQL JOIN means "to combine two or more tables". In SQL, 
JOIN clause is used to combine the records from two or more 
tables in a database.

---
### TYPES OF JOIN
1. Self join
2. Inner join- Is used to combine two tables together on the common column between them. Types of inner join- Inner join, left join, right join, full join
3. Cross join
4. Outer join which is sub-divided into three- The full outer join, the left outer join, the right outer join.

 - INNER JOIN 
In SQL, INNER JOIN selects records that have matching values in both tables as long as the condition is satisfied. It returns the combination of all rows from 
both the tables where the condition satisfies.

- LEFT JOIN 
The SQL left join returns all the values from left table and the matching values from the right table. If there is no matching join value, it 
will return NULL.
SELECT EMPLOYEE.EMP_NAME, PROJECT.DEPARTMENT FROM EMPLOYEE 

- RIGHT JOIN
In SQL, RIGHT JOIN returns all the values from the values from the rows of right table and the matched values from the left table. If 
there is no matching in both tables, it will return NULL.
SELECT EMPLOYEE.EMP_NAME, PROJECT.DEPARTMENT FROM EMPLOYEE

- FULL JOIN 
In SQL, FULL JOIN is the result of a combination of both left and right outerjoin. Join tables have all the records from both tables. It puts 
NULL on the place of matches not found.
SELECT EMPLOYEE.EMP_NAME, PROJECT.DEPARTMENT FROM EMPLOYEE 

## SQL Set Operation
---
SQL set operations allow you to combine the results of two or more SELECT queries. These operations treat the result sets 
of each query as mathematical sets, enabling you to perform set operations like union, intersection, and difference on them. 
SQL provides the following set operations.

1. Union Operation 
• The SQL Union operation is used to combine the result of two or more SQL SELECT queries. 
• In the union operation, all the number of datatype and columns must be same in both the tables on which UNION operation is being 
applied.
• The union operation eliminates the duplicate rows from its result set.

2. Union All
Combines the results of two or more SELECT queries but does not remove duplicates.
 
3. Intersect Operation
• It is used to combine two SELECT statements. The Intersect operation returns the common rows from the SELECT statements.
• In the Intersect operation, the number of datatype and columns must be the same.
• It has no duplicates, and it arranges the data in ascending order by default.

### SET OPERATORS
  ---
- Union – Is used to combine two columns from two tables but remove duplicate.
- Union all – It used to combine two columns without removing duplicate.
- Intersect – Picks what is common between the two tables.
- Minus – Picks what we have in Table B and not what we have in Table A
- Except – Picks what we have in Table A and not in table B.
- DISTINCT: Is used to make a unique listing or use to make a distinguish value.

   
### SQL DATATYPES
---
- SQL data types is defined as the type of value that can be stored in a table column. For example, if you want a column to store only integer values, you can define its data type as INT. SQL data types can be broadly divided into the following categories.
  
1. Numeric data types such as: INT, TINYINT, BIGINT, FLOAT, REAL, etc.
2. Date and Time data types such as: DATE, TIME, DATETIME, etc.
3. Character and String data types such as: CHAR, VARCHAR, TEXT, etc.
4. Unicode character string data types such as: NCHAR, NVARCHAR, NTEXT, etc.
5. Binary data types such as: BINARY, VARBINARY, etc.
6. Miscellaneous data types - CLOB, BLOB, XML, CURSOR, TABLE, etc.

### SQL KEYS 
---
- In SQL, Keys are special fields in a table that help:
✓ Create relationships between tables,
✓ Maintain uniqueness 
✓ Ensure data is consistent and valid

1. Primary Key: 
A special type of key that uniquely identifies each record in a table. Each table can have only one primary key.
Example: Employee_id in the Employee table.

2. Foreign Key:
A field in one table that uniquely identifies a row of another table, creating a relationship between the two tables.
Example: Employee_id in the Salary table is a foreign key (FK) that references the Employee_id in the Employee table 
(PK)

2. Surrogate Key:
A surrogate key is a unique identifier for each record in a table, typically created by the database itself (e.g an autoincrementing integer)

3. Composite Key:
Composite key (also known as compound key concatenated key) is a group of two or more columns that identifies each 
row of a table uniquely.
Example: In salary tables, Employee_id and Salary_month_year are combined to identify each row uniquely in salary 
table

4. Candidate Key:
Candidate key is a key of a table which can be selected as primary key. A table can have multiple candidate keys, out of 
which one can be selected as a primary key. 
Example: Employee_id, License_Number, and Passport_Number
Alternate key:
Alternate key is a candidate key, currently not selected as a primary key of the table
Example: License_Number and Passport_Numbers

### SQL CLAUSES
---
SQL clauses are essential components of SQL (Structured Query Language) that define how queries interact with the 
database. They are used to specify conditions, modify data, and control how results are returned. Here’s an overview of 
some of the most common SQL clauses.

- Group BY Clause
SQL GROUP BY statement is used to arrange identical data into groups. 
• The GROUP BY statement is used with the SQL SELECT statement. 
• The GROUP BY statement follows the WHERE clause in a SELECT statement and precedes the ORDER BY clause. 
• The GROUP BY statement is used with aggregation function
- Having Clause
• HAVING clause is used to specify a search condition for a group or an aggregate. 
• Having is used in a GROUP BY clause. If you are not using GROUP BY clause then you can use HAVING function like a 
- WHERE clause 
Order BY 
• The ORDER BY clause sorts the result-set in ascending or descending order. 
• It sorts the records in ascending order by default. DESC keyword is used to sort the records in descending order

### VIEW IN SQL 
---
An SQL View is a virtual table that is created based on the result set of a SQL query. Unlike a regular table, a view does not 
store data itself; instead, it dynamically retrieves data from one or more underlying tables whenever the view is queried.
✓ A view behaves like a table in SQL, allowing you to select, update, insert, and delete data (with some limitations).
✓ The data in a view is not stored physically; it is generated dynamically when the view is accessed.
✓ A view is defined using a SELECT statement that can join multiple tables, filter rows, and select specific columns.
Security
✓ Views can be used to restrict access to certain data in a table by exposing only specific columns or rows to the user.
✓ For example, you can create a view that only shows certain fields of a sensitive table, hiding the rest from the user.
Simplicity
✓ Views simplify complex queries. Instead of writing a complex query repeatedly, you can create a view and use it as a 
simple table.
✓ This is particularly useful in applications where complex logic needs to be reused

### SQL CASE WHEN STATEMENT
---
The CASE WHEN statement in SQL is a conditional expression that allows you to create different outputs based on certain 
conditions. It is similar to the IF-THEN-ELSE logic in programming languages.
This statement is often used to implement logic directly within SQL queries, making them more dynamic and adaptable to 
different scenarios.

```SQL
SELECT 
 product_name,
 CASE category_id
 WHEN 1 THEN 'Electronics'
 WHEN 2 THEN 'Furniture'
 WHEN 3 THEN 'Clothing'
 ELSE 'Other'
 END AS category_name
FROM products;
In this example, the CASE statement checks the category_id of each product and returns the corresponding category 
name. 
If category_id is 1, it returns 'Electronics’;
if 2, it returns 'Furniture’; 
```
and so on.

 - Flexibility: 
CASE can be used in SELECT, UPDATE, INSERT, and ORDER BY clauses, making it very versatile..
 - Readability: 
CASE statements can make your SQL queries more readable by replacing nested IF statements.
- Efficiency: 
Even though CASE adds some complexity to your queries, it often improves efficiency by reducing the need for multiple 
queries or conditional logic in your application code

