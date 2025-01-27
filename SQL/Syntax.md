# Structured Query Language (SQL)

# Major SQL Commands
> * SELECT
> * UPDATE
> * DELETE
> * INSERT
> * WHERE

# Using SQL with a Web Site
What you need
> * A Relational Database Management System
>   * MySQL
>   * SQLite
>   * PostgreSQL
>   * MariaDB
> * A server side scripting language(JS, python, Java, PHP, ASP)
> * SQL
> * HTML/CSS for page styling

# SQL  is broken into tables
Each table is broken up into fields and records.
||||
|:-:|:-:|:-:|
|field|column|vertical|
|record|row|horizontal|

# SQL Statements
> * Keywords

*SQL keywords are not case sensitive: `select` and `SELECT` are the same*

It is convention to type keywords in uppercase

Use a semicolon to separate each SQL statement

syntax:
```
SELECT * FROM Table;
```
Each table is identified by a name and contains fields and records

\* is a wildcard operator that selects all


# Common SQL Commands
|Command|Description|
|:-:|:-:|
|SELECT|extracts data from a database|
|UPDATE|updates data in a database|
|DELETE|deletes data from a database|
|INSERT INTO|inserts new data into a database|
|CREATE DATABASE|creates a new database|
|ALTER DATABASE|modifies a database|
|CREATE TABLE|creates a new table|
|ALTER TABLE|modifies a table|
|DROP TABLE|deletes a table|
|CREATE INDEX|creates an index (search key)|
|DROP INDEX|deletes an index|

# SELECT statment

syntax:
```
SELECT column1,column2, ... FROM table_name;
```

Select distinct is used to return only distinct(different) values

Syntax:
```
SELECT DISTINCT column1,column2, ... FROM table_name;
```

Select Count Distinct, returns the number of a given field

Syntax:
```
SELECT COUNT(DISTINCT column_name) FROM table_name;
```


# WHERE Clause
> * WHERE is used to filter records

syntax:
```
SELECT column1, column2, ... FROM table_name WHERE condition;
```
Where can also be used with UPDATE and DELETE

SQL requires single quotes around text values, most database systems will also allow double quotes

WHERE clause operators
|Command|Description|
|:-:|:-:|
|=	|Equal	|
|>	|Greater than	|
|<	|Less than	|
|>=	|Greater than or equal	|
|<=	|Less than or equal	|
|<>	|Not equal. Note: In some versions of SQL this |operator may be written as !=	
|BETWEEN	|Between a certain range	|
|LIKE	|Search for a pattern	|
|IN	|To specify multiple possible values for a column|


# ORDER BY
> * keyword used to sort the result-set in ascending or descending order

Syntax:
```
SELECT column1, column2, ... FROM table_name ORDER BY column1, column2, ... ASC|DESC;
```
ASC --> Ascending
DESC --> Descending

String values are automatically ordered automatically

When using Several Columns it orders by the first column first, if the first is identical then it orders by the second column.

Using both ASC and DESC
Syntax:
```
SELECT column1, column2, ... FROM table_name ORDER BY column1 ASC, column2 DESC, ... ;
```


# AND Operator
> displays a record if all the records are True
> WHERE can contain one or many AND operators
> AND is used to filter records based on more than one condition


Syntax:
```
SELECT column1, column2, ... FROM table_name WHERE condition1 AND condition2 AND condition3 ...;
```

# OR Operator
> displays a record if any of the conditions are True
> WHERE can contain one or many OR operators
> OR is used to filter records based on more than one condition

Syntax:
```
SELECT column1, column2, ... FROM table_name WHERE condition1 OR condition2 OR condition3 ...;
```





