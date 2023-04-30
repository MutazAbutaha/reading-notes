Ex 1
SELECT queries : To retrieve data from a SQL database, we need to write SELECT statements,
![](./SQL/Screenshot%20(80).png)

Ex2 : Queries with constraints: we can use condation to retrive spacific data .WHERE
![](./SQL/Screenshot%20(81).png)

Ex3
Queries with constraints : When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison like (<,>,!=,=,%)
![](./SQL/Screenshot%20(82).png)

Ex 4 : Filtering and sorting Query results : provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.
![](./SQL/Screenshot%20(83).png)

Ex 5 : Simple SELECT Queries :
SELECT column,
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
![](./SQL/Screenshot%20(84).png)

Ex 6 : Multi-table queries with JOINs . Using the JOIN clause in a query, we can combine row data across two separate tables using this unique key. The first of the joins that we will introduce is the INNER JOIN
![](./SQL/Screenshot%20(85).png)

Ex 13 : Inserting rows :When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.
![](./SQL/Screenshot%20(88).png)

Ex 14 : Updating rows adding new data, a common task is to update existing data, which can be done using an UPDATE statement
![](./SQL/Screenshot%20(89).png)

Ex 15 Deleting rows : When you need to delete data from a table in the database, you can use a DELETE statement, which describes the table to act on, and the rows of the table to delete through the WHERE clause
![](./SQL/Screenshot%20(90).png)

Ex 16 :Creating tables : hen you have new entities and relationships to store in your database, you can create a new database table using the CREATE TABLE statement
CREATE TABLE IF NOT EXISTS mytable (
);
![](./SQL/Screenshot%20(91).png)


Ex 17 : Altering tables : As your data changes over time, SQL provides a way for you to update your corresponding tables and database schemas by using the ALTER TABLE statement to add, remove, or modify columns and table constraints
![](./SQL/Screenshot%20(92).png)

Ex 18:Dropping tables you may want to remove an entire table including all of its data and metadata, and to do so, you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely
DROP TABLE IF EXISTS
![](./SQL/Screenshot%20(93).png)
![](./SQL/Screenshot%20(94).png)

