<h1>DATA MODELS</h1>

 - Data Model is the modeling of the data description, data semantics, and consistency constraints of the data. 
 - It provides the conceptual tools for describing the design of a database at each level of data abstraction. 
 - Therefore, there are following four data models used for understanding the structure of the database: 

 <h1>Four Types of DBMS systems are: </h1>

- Hierarchical database 
- Network database 
- Relational database ER model database 

<h2>Hierarchical DBMS</h2> 

  ==>   In a Hierarchical database, model data is organized in a tree-like structure. Data is Stored 
Hierarchically (top down or bottom up) format. Data is represented using a parent-child 
relationship. In Hierarchical DBMS parent may have many children, but children have 
only one parent. 

<h2>Network Model </h2>

  ==>   The network database model allows each child to have multiple parents. It helps you to address 
the need to model more complex relationships like as the orders/parts many-to-many 
relationship. In this model, entities are organized in a graph which can be accessed through 
several paths.

<h2>Relational model</h2>

  ==>   Relational DBMS is the most widely used DBMS model because it is one of the easiest. This 
model is based on normalizing data in the rows and columns of the tables. Relational model 
stored in fixed structures and manipulated using SQL. 

<h2>Entity-Relationship Model</h2>

==>   Entity-Relationship (ER) Model is based on the notion of real-world entities and relationships 
among them. While formulating real-world scenario into the database model, the ER Model 
creates entity set, relationship set, general attributes and constraints. 
<h1></h1>

**Database languages :** `are used to read, update and store data in a database. There are 
several such languages that can be used for this purpose; one of them is SQL (Structured 
Query Language).` 

- ``DDL`` – **Data Definition Language:** (CREATE,DROP,ALTER,TRUNCATE,COMMENT,RENAME) 
- ``DML`` – **Data Manipulation Language:** (INSERT, UPDATE,DELETE) 
- `DCL` – **Data Control Language:** (GRANT,REVOKE) 
- `TCL` - **Transaction Control Language:** (COMMIT,ROLLBACK) 





<h2>1. DDL(Data Definition Language) :</h2>  DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with 
descriptions of the database schema and is used to create and modify the structure of database objects in the database. 

CREATE – it is used to create the database or its objects (like table, index, function, views, store procedure and triggers). 

**There are two CREATE statements available in SQL:** 
- CREATE DATABASE 
- CREATE TABLE

<h2>CREATE DATABASE</h2> 
A Database is defined as a structured set of data. So, in SQL the very first step to store 
the data in a well structured manner is to create a database. The CREATE DATABASE 
statement is used to create a new database in SQL. 

**Syntax:**  
``CREATE DATABASE database_name;``

**Example:** 
``SQL> CREATE DATABASE Employee;`` 

In order to get the list of all the databases, you can use SHOW DATABASES statement. 

**Example –**
``SQL> SHOW DATABASES;``



<h2>CREATE TABLE:</h2>
The CREATE TABLE statement is used to create a table in SQL. We know that a table 
comprises of rows and columns. So while creating tables we have to provide all the 
information to SQL about the names of the columns, type of data to be stored in columns, 
size of the data etc. Let us now dive into details on how to use CREATE TABLE statement 
to create tables in SQL. 

**Syntax:** 

``CREATE TABLE table_name 
(column1 data_type(size),
column2 data_type(size),
column3 data_type(size), .... 
);``

**Example Query:** 
This query will create a table named Students with three columns, ROLL_NO, NAME and SUBJECT.

``CREATE TABLE Students 
(ROLL_NO int(3),
NAME varchar(20),
SUBJECT varchar(20), 
);`` 
