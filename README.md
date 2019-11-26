# SQL Basics Notes
## Databases
- Column - Database tables are composed of individual columns corresponding to the attributes of the object
- Row - Consists of one set of attributes corresponding to one instance that a table describes (records or tuples)
- Table - Predefined format of rows and columns that define an entity
- DBMS - Database Management System, performs database functions
- Flat-file Database - Stores everything in one table, good for small numbers of records related to a single topic
- Relational Database - Gives you the ability to separate masses of data into numerous tables, linked to each other through the use of keys
- Big Data - MongoDB, Vertica etc., used for data analytics and business intelligence, digital age and internet of things (NoSQL)


## Relational Database
- 1-1 - Each row in Table A is linked to no more than one row in Table B
- 1-Many - Each row in the table can be related to many rows in the relating table
- Many-Many - One or more rows in a table can b e related to 0, or 1 or many rows in another table
- Primary key – Uniquely identifies each record in the table, most tables must have a PK, DBMS will enforce uniqueness meaning not allowing repeated records to exist in the table
  - Must be unique
  - Must always have an entry – cannot be blank or null
  - Value can never change
- Foreign key
  - Natural relationships exist between tables in most databases structures, foreign keys used to create solid relationships
  - Ensure that the row of information in table A corresponds to the correct row of information in table B
  - The constraint is used to prevent actions that would destroy links between tables
  - Prevents invalid data from being inserted into the foreign key columns


## DML DDL DCL and TCL
- DML – data manipulation language, CRUD – create, read, update, delete
  -	Select
  -	Insert
  -	Update
  -	Delete
- DDL – data definition language
  -	Create
  -	Alter
  -	Drop
  -	Truncate
-	DCL – data control language
  -	Grant
  -	Revoke
-	TCL – transaction control language
  -	Commit
  -	Rollback
  -	Savepoint


## Database considerations
-	Data Security
-	Data Recovery
-	Data Integrity
-	Normal Form
  -	1st normal form when following conditions are satisfied:
    - Make everything atomic – data must be presented as small as it can be
    -	There should be no repeating groups – generate new table
  -	2nd normal form is when following conditions are satisfied:
    -	It is in 1st normal form
    -	All non-key attributes are fully functional dependent on the primary key
  -	3rd normal form is when the following conditions are satisfied:
    -	It is in 2nd normal form
    -	There is no transitive functional dependency – when a non-key column is functional dependent on another non-key column, which is functionally dependent on the primary key
