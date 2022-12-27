# SQL

* SQL (Structured Query Language) is a programming language used to communicate with databases. It is used to manage and manipulate data stored in relational databases, which are organized in tables with rows and columns.

* SQL is used to create, modify, and query databases. It allows users to perform a variety of tasks, such as:

  * Creating new databases and tables
  * Inserting data into tables
  * Updating and deleting data from tables
  * Retrieving data from tables
  * Setting permissions on tables and other database objects

* SQL uses a standard set of commands, such as SELECT, INSERT, UPDATE, DELETE, and CREATE, to perform these tasks. These commands are called SQL statements.

* SQL is a powerful and flexible language that is widely used in a variety of applications, including web development, data analysis, and business management. It is a standard language used by many relational database management systems (RDBMS), such as MySQL, Oracle, and Microsoft SQL Server.

## SQL vs NoSQL

|        |SQL Databases|NoSQL Databases|
|--------|-------------|---------------|
|Data Storage Model|Tables with fixed rows and columns|Document: JSON documents, Key-value: key-value pairs, Wide-column: tables with rows and dynamic columns, Graph: nodes and edges|
|Development History|Developed in the 1970s with a focus on reducing data duplication|Developed in the late 2000s with a focus on scaling and allowing for rapid application change driven by agile and DevOps practices.|Document: MongoDB and CouchDB, Key-value: Redis and DynamoDB, Wide-column: Cassandra and HBase, Graph: Neo4j and Amazon Neptune|
|Examples|Oracle, MySQL, Microsoft SQL Server, and PostgreSQL|Document: MongoDB and CouchDB, Key-value: Redis and DynamoDB, Wide-column: Cassandra and HBase, Graph: Neo4j and Amazon Neptune|
|Primary Purpose|General purpose|Flexible|Document: general purpose, Key-value: large amounts of data with simple lookup queries, Wide-column: large amounts of data with predictable query patterns, Graph: analyzing and traversing relationships between connected data|
|Schemas|Rigid|Flexible|
|Scaling|Vertical (scale-up with a larger server)|Horizontal (scale-out across commodity servers)|
|Multi-Record ACID Transactions|Supported|Most do not support multi-record ACID transactions. However, some — like MongoDB — do.|
|Joins|Typically required|Typically not required|
|Data to Object Mapping|Requires ORM (object-relational mapping)|Many do not require ORMs. MongoDB documents map directly to data structures in most popular programming languages.|

### What are the benefits of NoSQL databases?

* NoSQL databases offer many benefits over relational databases. NoSQL databases have flexible data models, scale horizontally, have incredibly fast queries, and are easy for developers to work with.

  * Flexible data models
    * NoSQL databases typically have very flexible schemas. A flexible schema allows you to easily make changes to your database as requirements change. You can iterate quickly and continuously integrate new application features to provide value to your users faster.

  * Horizontal scaling
    * Most SQL databases require you to scale-up vertically (migrate to a larger, more expensive server) when you exceed the capacity requirements of your current server. Conversely, most NoSQL databases allow you to scale-out horizontally, meaning you can add cheaper commodity servers whenever you need to.

  * Fast queries
    * Queries in NoSQL databases can be faster than SQL databases. Why? Data in SQL databases is typically normalized, so queries for a single object or entity require you to join data from multiple tables. As your tables grow in size, the joins can become expensive. However, data in NoSQL databases is typically stored in a way that is optimized for queries. The rule of thumb when you use MongoDB is data that is accessed together should be stored together. Queries typically do not require joins, so the queries are very fast.

  * Easy for developers
    * Some NoSQL databases like MongoDB map their data structures to those of popular programming languages. This mapping allows developers to store their data in the same way that they use it in their application code. While it may seem like a trivial advantage, this mapping can allow developers to write less code, leading to faster development time and fewer bugs.

### What are the drawbacks of NoSQL databases?

* One of the most frequently cited drawbacks of NoSQL databases is that they don’t support ACID (atomicity, consistency, isolation, durability) transactions across multiple documents. With appropriate schema design, single-record atomicity is acceptable for lots of applications. However, there are still many applications that require ACID across multiple records.

* To address these use cases, MongoDB added support for multi-document ACID transactions in the 4.0 release, and extended them in 4.2 to span shared clusters.

* Since data models in NoSQL databases are typically optimized for queries and not for reducing data duplication, NoSQL databases can be larger than SQL databases. Storage is currently so cheap that most consider this a minor drawback, and some NoSQL databases also support compression to reduce the storage footprint.

* Depending on the NoSQL database type you select, you may not be able to achieve all of your use cases in a single database. For example, graph databases are excellent for analyzing relationships in your data but may not provide what you need for everyday retrieval of the data such as range queries. When selecting a NoSQL database, consider what your use cases will be and if a general purpose database like MongoDB would be a better option.

## DDL

* Data Definition Language (DDL) is a subset of SQL that is used to define the structure and organization of data in a database. It includes a set of commands and statements that can be used to create, modify, and delete database objects such as tables, indexes, and views.

* The main statements used in data definition language are:

  * **CREATE**: This statement is used to create new database objects, such as tables, indexes, and views. It allows you to specify the name and structure of the object you want to create, as well as any constraints or other properties you want to set.

   ```sql
    CREATE TABLE orders (
    order_id serial PRIMARY KEY,
    customer_id integer NOT NULL,
    product_id integer NOT NULL,
    quantity integer NOT NULL,
    FOREIGN KEY (customer_id) REFERENCES customers (customer_id),
    FOREIGN KEY (product_id) REFERENCES products (product_id)
    );
    ```

  * **ALTER**: This statement is used to modify the structure or properties of an existing database object. It allows you to add, modify, or delete columns, constraints, and other elements of the object.

    ```sql
    ALTER TABLE customers
    ALTER COLUMN email SET NOT NULL;
    ```

  * **DROP**: This statement is used to delete an existing database object. It allows you to specify the object you want to delete and removes it from the database.

    ```sql
    DROP TABLE customers;
    ```

  * **TRUNCATE**: This statement is used to delete all rows from a table, but unlike the DROP statement, it does not delete the table itself. It can be faster than the DELETE statement, especially for large tables, as it only removes the data and leaves the structure of the table intact.

    ```sql
    TRUNCATE TABLE customers;
    ```

  * **RENAME**: This statement is used to change the name of an existing database object. It allows you to specify the object you want to rename and the new name you want to give it.

    ```sql
    ALTER TABLE customers
    RENAME TO old_customers;
    ```

* Data definition language is an important part of any database management system, as it allows you to define and organize the data stored in your database and to maintain its structure over time.

* DDL statements are typically used to design and modify the structure of a database, rather than to manipulate data within the database. They are an important part of the SQL language and are used to ensure that the database is properly organized and optimized for efficient data storage and retrieval.

## DQL

* Data Query Language (DQL) is a subset of SQL that is used to retrieve and retrieve data from a database. It includes a set of commands and statements that can be used to perform various operations on the data stored in a database, such as selecting, filtering, and sorting data.

* Here are some examples of common DQL statements:

  * **SELECT** is used to retrieve data from a table. It specifies the columns that should be included in the results, as well as any conditions that must be met in order for a row to be included.

  * **FROM** specifies the table(s) from which the data should be retrieved.

  * **WHERE** specifies a condition that rows must meet in order to be included in the results.

  * **GROUP BY** groups rows with similar values together and can be used in conjunction with aggregation functions such as SUM and AVG to perform calculations on the grouped data.

  * **HAVING** is similar to WHERE, but it is used to filter groups of rows rather than individual rows.

  * **ORDER** BY sorts the results by one or more columns in ascending or descending order.

```sql
-- Select the "FirstName", "LastName", and total number of orders for each customer
-- sorted by the number of orders
SELECT FirstName, LastName, COUNT(*) AS TotalOrders
FROM Customers INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID
GROUP BY Customers.CustomerID
HAVING COUNT(*) > 10
ORDER BY TotalOrders DESC;
```

## DML

* Data manipulation language (DML) is a subset of SQL that is used to manage and manipulate data in a database. It includes a set of commands and statements that can be used to perform various operations on the data stored in a database, such as inserting, updating, deleting, and selecting data.

* The main statements used in data manipulation language are:

  * **SELECT**: This statement is used to retrieve data from a database. It allows you to specify which columns and rows you want to retrieve, and can include various clauses such as WHERE, GROUP BY, and HAVING to filter and organize the data.

    ```sql
    SELECT * FROM customers WHERE state = 'NY';
    ```

  * **INSERT**: This statement is used to add new rows of data to a table in a database. It allows you to specify the values you want to insert into the table and the columns in which you want to insert them.

    ```sql
    INSERT INTO customers (first_name, last_name, email, state)
    VALUES ('John', 'Doe', 'john.doe@example.com', 'NY');
    ```

  * **UPDATE**: This statement is used to modify existing data in a database. It allows you to specify which rows you want to update and the new values you want to set for the columns in those rows.

    ```sql
    UPDATE customers
    SET email = 'john.doe@gmail.com'
    WHERE customer_id = 123;
    ```

  * **DELETE**: This statement is used to remove rows of data from a table in a database. It allows you to specify which rows you want to delete, either by specifying a specific condition or by deleting all rows in the table.

    ```sql
    DELETE FROM customers
    WHERE state = 'NY';
    ```

  * **MERGE**: This statement is used to merge data from multiple sources into a single table in a database. It allows you to specify the sources of the data you want to merge and the columns and rows you want to include in the merged table.

    ```sql
    MERGE INTO customers USING new_customers
    ON (customers.customer_id = new_customers.customer_id)
    WHEN MATCHED THEN UPDATE SET customers.email = new_customers.email
    WHEN NOT MATCHED THEN INSERT (first_name, last_name, email, state)
    VALUES (new_customers.first_name, new_customers.last_name, new_customers.email, new_customers.state);
    ```

* Data manipulation language is an important part of any database management system, as it allows you to perform a variety of operations on the data stored in your database and to keep it organized and up-to-date.

## DCL

* Data control language (DCL) is a subset of SQL that is used to control access to and manipulate data in a database. It includes a set of commands and statements that can be used to set permissions, create and modify users and roles, and manage transactions.

* The main statements used in data control language are:

  * **GRANT**: This statement is used to give a user or role permission to perform a specific action on a database object.

    ```sql
    -- grants the user user1 permission to select (retrieve) data from the customers table.
    GRANT SELECT ON TABLE customers TO user1;
    ```

  * **REVOKE**: This statement is used to remove a previously granted permission from a user or role.

    ```sql
    -- revokes the SELECT permission on the customers table from the user user1.
    REVOKE SELECT ON TABLE customers FROM user1;
    ```

  * **SET ROLE**: This statement is used to set the active role for a user, which determines the permissions the user has when accessing the database.

    ```sql
    -- sets the active role for the current user to role1.
    SET ROLE role1;
    ```

* Data control language is an important part of any database management system, as it allows you to control access to the data stored in your database and to manage the changes made to that data over time.

## TCL

* Transaction control language (TCL) is a subset of SQL that is used to manage transactions in a database. Transactions are a way of grouping a series of database operations into a single unit of work, so that either all of the operations are completed, or none of them are completed if an error occurs. This ensures the integrity of the data in the database, as it prevents partially completed transactions from leaving the data in an inconsistent state.

* There are several TCL statements in PostgreSQL that can be used to control transactions:

  * **BEGIN**: This statement starts a new transaction block. All subsequent SQL statements will be part of the same transaction until an explicit COMMIT or ROLLBACK statement is encountered.

  * **COMMIT**: This statement ends the current transaction block and saves all changes made to the database during the transaction.

    ```sql
    BEGIN;
    -- SQL statements go here
    COMMIT;
    ```

  * **ROLLBACK**: This statement ends the current transaction block and undoes all changes made to the database during the transaction.

    ```sql
    BEGIN;
    -- SQL statements go here
    ROLLBACK;
    ```

  * **SAVEPOINT**: This statement creates a named savepoint within a transaction block. A savepoint allows you to roll back part of a transaction block to a specific point, rather than rolling back the entire transaction.

  * **ROLLBACK TO SAVEPOINT**: This statement rolls back the current transaction block to a specific savepoint, undoing all changes made to the database since the savepoint was created.
  *
  * **RELEASE SAVEPOINT**: This statement removes a savepoint that was created within a transaction block.

    ```sql
    BEGIN;
    -- SQL statements go here
    SAVEPOINT my_savepoint;
    -- More SQL statements go here
    ROLLBACK TO SAVEPOINT my_savepoint;
    RELEASE SAVEPOINT my_savepoint;
    COMMIT;
    ```

It is important to use TCL statements carefully, as they can have significant effects on the data in a database. It is a good idea to test transaction blocks in a development environment before using them in a production database.

### SET TRANSACTION

* The SET TRANSACTION statement in PostgreSQL allows you to specify the isolation level and read-only mode for a transaction block. The isolation level determines how the changes made by a transaction will be visible to other transactions. The read-only mode determines whether the transaction is allowed to make changes to the database.

* Here is the syntax for the SET TRANSACTION statement in PostgreSQL:

```sql
SET TRANSACTION [ ISOLATION LEVEL { SERIALIZABLE | REPEATABLE READ | READ COMMITTED | READ UNCOMMITTED } ]
                  [ READ ONLY | READ WRITE ]
```

* The ISOLATION LEVEL clause sets the isolation level for the transaction. The four possible values are:

  * **SERIALIZABLE**: This is the highest isolation level, and it ensures that transactions are executed in a serializable order. This means that transactions will not be able to see any changes made by other transactions until they have been committed.

  * **REPEATABLE** READ: This isolation level ensures that transactions will not be able to see any changes made by other transactions until they have been committed, but it allows non-repeatable reads to occur.

  * **READ COMMITTED**: This isolation level ensures that transactions will not be able to see any changes made by other transactions until they have been committed, but it allows dirty reads to occur.

  * **READ UNCOMMITTED**: This is the lowest isolation level, and it allows transactions to see changes made by other transactions that have not yet been committed.

* The READ ONLY and READ WRITE clauses specify whether the transaction is allowed to make changes to the database. If READ ONLY is specified, the transaction will not be able to make any changes to the database. If READ WRITE is specified, the transaction will be able to make changes to the database.

* The default isolation level in PostgreSQL is READ COMMITTED, and the default read-only mode is READ WRITE.

## PostgreSQL

* PostgreSQL, also known as Postgres, is a powerful, open-source object-relational database management system (ORDBMS). It is designed to handle a wide range of data types, from simple data types such as integers and strings, to more complex data types such as arrays, JSON documents, and spatial data. PostgreSQL is highly customizable, with a large number of configuration options and an extensible architecture that allows users to create custom data types, functions, and index types.

* PostgreSQL is known for its robustness, reliability, and performance. It supports multiple storage engines, including heap-based and B-tree based tables, as well as full-text search and materialized views. It also supports a wide range of programming languages and development frameworks, including C, C++, Java, Python, Ruby, and more.

* PostgreSQL is used by many organizations around the world, including government agencies, educational institutions, and Fortune 500 companies. It is popular for its feature-richness, scalability, and support for ACID (Atomicity, Consistency, Isolation, Durability) transactions, which ensure that data is stored and retrieved consistently and accurately.

* PostgreSQL is available for multiple operating systems, including Linux, Unix, and Windows. It is released under the PostgreSQL License, which is a permissive free software license.

## Schema

* a schema is a logical container for database objects such as tables, views, and functions. A schema is similar to a namespace in other programming languages, as it provides a way to organize and group related objects together. Each database in PostgreSQL can contain multiple schemas, and each schema can contain multiple objects. This allows you to structure your database in a way that makes sense for your application, and to create a logical separation between different types of objects.

* In PostgreSQL, there is also a special schema called public, which is created by default in every database. The public schema is the default schema for all users and roles, unless a different default schema is specified. Objects in the public schema are visible to all users and roles, unless the object's visibility is restricted by permissions.

## Table

* a table is a database object that stores data in rows and columns. Tables are used to store structured data, such as lists of users, products, or orders. Tables in PostgreSQL are defined by a set of columns, each with a specific data type. The data type specifies the kind of data that can be stored in the column, such as integers, strings, or dates. Tables can also have constraints, which are rules that specify the allowed values for a column or group of columns. Constraints can be used to ensure the integrity of the data in the table, such as ensuring that a column contains only unique values or that a column has a non-null value.

## Transaction Properties

* In the context of database systems, the acronym ACID stands for Atomicity, Consistency, Isolation, and Durability. These are the four main properties that are used to describe the behavior of a transaction in a database management system.

  * **Atomicity**: Atomicity refers to the all-or-nothing nature of a transaction. This means that either all of the statements within a transaction are executed successfully, or none of them are executed at all. This ensures that the database remains in a consistent state even if there is an error or failure during the transaction.

  * **Consistency**: Consistency refers to the property that ensures that a transaction only performs valid database operations. This means that a transaction cannot leave the database in an inconsistent state, such as by violating a foreign key constraint or creating a null value in a column that is not nullable.

  * **Isolation**: Isolation refers to the property that ensures that the changes made by one transaction are not visible to other transactions until the first transaction is committed. This ensures that the data accessed by a transaction is consistent with the state of the database at the start of the transaction.

  * **Durability**: Durability refers to the property that ensures that the changes made by a transaction are permanently saved to the database. This ensures that the changes made by a transaction are not lost in the event of a failure or crash.

* In PostgreSQL, transactions have these ACID properties by default. You can use the BEGIN, COMMIT, and ROLLBACK statements to define and control transactions in PostgreSQL.

## JOINS

* a join is a way to combine rows from two or more tables based on a related column between them. There are several types of joins in PostgreSQL: inner join, outer join, left join, right join, and cross join.

  * An **inner join** returns only the rows that satisfy the join condition and exist in both tables. The syntax for an inner join is as follows:

    ```sql
    SELECT *
    FROM table1
    INNER JOIN table2
    ON table1.col1 = table2.col2;
    ```

  * This statement will return all rows from both table1 and table2 where the values in col1 of table1 and col2 of table2 are equal.

  * An **outer join** retrieves all rows from both tables, regardless of whether they match the join condition. There are three types of outer joins: left outer join, right outer join, and full outer join.

  * A left outer join retrieves all rows from the left table (table1 in the example below), even if there is no match in the right table (table2):

    ```sql
    SELECT *
    FROM table1
    LEFT JOIN table2
    ON table1.col1 = table2.col2;
    ```

  * A right outer join retrieves all rows from the right table (table2 in the example below), even if there is no match in the left table (table1):

    ```sql
    SELECT *
    FROM table1
    RIGHT JOIN table2
    ON table1.col1 = table2.col2;
    ```

  * A full outer join retrieves all rows from both tables, regardless of whether there is a match in the other table:

    ```sql
    SELECT *
    FROM table1
    FULL OUTER JOIN table2
    ON table1.col1 = table2.col2;
    ```

  * A cross join retrieves all rows from both tables, creating a Cartesian product of the rows. It does not use a join condition. For example:

    ```sql
    -- will return all possible combinations of rows from table1 and table2
    SELECT *
    FROM table1
    CROSS JOIN table2;
    ```
