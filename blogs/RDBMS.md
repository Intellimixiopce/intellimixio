<h1> What is Relational Model? </h1>

**Relational Model (RM)** represents the database as a collection of relations. A relation is nothing but a table of values. Every row in the table represents a collection of related data 
values. These rows in the table denote a real-world entity or relationship. The table name and column names are helpful to interpret the meaning of values in each row. 
The data are represented as a set of relations. In the relational model, data are stored as tables. However, the physical storage of the data is independent of the way the data are logically 
organized. 

<h1>Relational Model Concepts</h1>

1. Attribute: Each column in a Table. Attributes are the properties which define a relation. e.g., Student_Rollno, NAME,etc. 
2. Tables – In the Relational model the, relations are saved in the table format. It is stored along with its entities. A table has two properties rows and columns. Rows represent records and columns represent attributes. 
3. Tuple – It is nothing but a single row of a table, which contains a single record. 
4. Relation Schema: A relation schema represents the name of the relation with its attributes. 
5. Degree: The total number of attributes which in the relation is called the degree of the relation. 
6. Cardinality: Total number of rows present in the Table. 
7. Column: The column represents the set of values for a specific attribute. 
8. Relation instance – Relation instance is a finite set of tuples in the RDBMS system. Relation instances never have duplicate tuples. 
9. Relation key - Every row has one, two or multiple attributes, which is called relation key. 
10. Attribute domain – Every attribute has some pre-defined value and scope which is known as attribute domain Keys in DBMS 

<h1>KEYS</h1>

**KEYS in DBMS** is an attribute or set of attributes which helps you to identify a row(tuple) in a relation(table). They allow you to find the relation between two tables. Keys help you 
uniquely identify a row in a table by a combination of one or more columns in that table. Key 
is also helpful for finding unique record or row from the table. Database key is also helpful for finding unique record or row from the table. 

<h1>Why we need a Key?</h1>
Here are some reasons for using sql key in the DBMS system.

- Keys help you to identify any row of data in a table. In a real-world application, a 
table could contain thousands of records. Moreover, the records could be 
duplicated. 
Keys ensure that you can uniquely identify a table record despite these challenges. 
- Allows you to establish a relationship between and identify the relation between 
tables 
- Help you to enforce identity and integrity in the relationship. 
Types of Keys in Database Management System 
There are mainly seven different types of Keys in DBMS and each key has its different 
functionality: 
- Super Key - A super key is a group of single or multiple keys which identifies 
rows in a table. 
- Primary Key - is a column or group of columns in a table that uniquely identify 
every row in that table. 
DATABASE MANAGEMENT SYSTEMS Page 30
- Candidate Key - is a set of attributes that uniquely identify tuples in a table. 
Candidate Key is a super key with no repeated attributes. 
- Alternate Key - is a column or group of columns in a table that uniquely identify 
every row in that table. 
- Foreign Key - is a column that creates a relationship between two tables. The 
purpose of Foreign keys is to maintain data integrity and allow navigation 
between two different instances of an entity. 
- Compound Key - has two or more attributes that allow you to uniquely 
recognize a specific record. It is possible that each column may not be unique by 
itself within the database. 
- Composite Key - An artificial key which aims to uniquely identify each record is 
called a surrogate key. These kind of key are unique because they are created 
when you don't have any natural primary key. 
- Surrogate Key - An artificial key which aims to uniquely identify each record is 
called a surrogate key. These kind of key are unique because they are created 
when you don't have any natural primary key. 


**Primary key example:** 

``CREATE TABLE Persons ( 
 ID int NOT NULL, 
 LastName varchar(255) NOT NULL, 
 FirstName varchar(255), 
 Age int, 
 PRIMARY KEY (ID) 
);``

<h1>ER model</h1> 

- ER model stands for an Entity-Relationship model. It is a high-level data model. This model is used to define the data elements and relationship for a specified system. 
- It develops a conceptual design for the database. It also develops a very simple and easy to design view of data.
- In ER modeling, the database structure is portrayed as a diagram called an entityrelationship diagram. 

``For example``, Suppose we design a school database. In this database, the student will be an 
entity with attributes like address, name, id, age, etc. The address can be another entity with 
attributes like city, street name, pin code, etc and there will be a relationship between them. 


<h1>Relational Algebra</h1>

- Relational Algebra is procedural query language, which takes Relation as input and generates relation as output. Relational algebra mainly provides theoretical 
foundation for relational databases and SQL. 
- Relational algebra is a procedural query language, it means that it tells what data to be retrieved and how to be retrieved. 
- Relational Algebra works on the whole table at once, so we do not have to use loops etc to iterate over all the rows (tuples) of data one by one. 
- All we have to do is specify the table name from which we need the data, and in a single line of command, relational algebra will traverse the entire given table to 
fetch data for you. 


<h2>Basic/Fundamental Operations: </h2>

1.Select (σ) 
2. Project (∏) 
3. Union ( ) 
4. Set Difference (-) 
5. Cartesian product (X) 
6. Rename (ρ) 

 <h2>Select Operation (σ) :</h2>
 
This is used to fetch rows (tuples) from table(relation) which satisfies a given condition. Syntax: σp(r)

➢ σ is the predicate

➢ r stands for relation which is the name of the table 

➢ p is prepositional logic ex: σage > 17 (Student)

<h2>Project Operation (∏): </h2>

- Project operation is used to project only a certain set of attributes of a relation. In simple words, If you want to see only the names all of the students in the Student table, then 
you can use Project Operation. 
- It will only project or show the columns or attributes asked for, and will also remove duplicate data from the columns. 


<h2>Union Operation (U): </h2>

- This operation is used to fetch data from two relations(tables) or temporary relation(result of another operation). 
- For this operation to work, the relations(tables) specified should have same number of attributes(columns) and same attribute domain. Also the duplicate tuples are 
autamatically eliminated from the result. 

<h2>Set Difference (-):</h2>

This operation is used to find data present in one relation and not present in the 
second relation. This operation is also applicable on two relations, just like Union 
operation. 

<h2>Rename Operation (ρ):</h2>

This operation is used to rename the output relation for any query operation which returns 
result like Select, Project etc. Or to simply rename a relation(table)

<h1>Join in DBMS:</h1>

- A JOIN clause is used to combine rows from two or more tables, based on a related column between them.
- Join in DBMS is a binary operation which allows you to combine join product and selection in one single statement. 
- The goal of creating a join condition is that it helps you to combine the data from two or more DBMS tables. 
- The tables in DBMS are associated using the primary key and foreign keys.


Types of SQL JOIN

``1. INNER JOIN`` 
In SQL, INNER JOIN selects records that have matching values in both tables as long as the 
condition is satisfied. 
It returns the combination of all rows from both the tables where the condition satisfies. 

``2. LEFT JOIN ``
The SQL left join returns all the values from left table and the matching values from the right 
table. If there is no matching join value, it will return NULL. 

``3. RIGHT JOIN`` 
In SQL, RIGHT JOIN returns all the values from the values from the rows of right table and 
the matched values from the left table. If there is no matching in both tables, it will return NULL. 

``4. FULL JOIN`` 
In SQL, FULL JOIN is the result of a combination of both left and right outer join. Join 
tables have all the records from both tables. It puts NULL on the place of matches not found. 
