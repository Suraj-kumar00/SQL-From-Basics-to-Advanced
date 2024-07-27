# Introduction to SQL and Database Fundamentals (Day 1)

## What is Database
- It's a collection of data


## Different Types of Databases
- #### Relation Database
    - Data is stored in the form of a table( rows and columns)
    - Structured data will be there
 
- Example:
  - MySQL
  - SQL Server
  - PostgreSQL and more...

- #### NoSQL Database
  - Data is not structured here
  - JSON(JavaScript Object Notation): Data stored in the form of {Key: Value}
  - Document
  - Graph
 
- Example
  - MongoDB
  - Cassandra
  - HBase
 
We'll be using MySQL Workbench --> Practical (Hands-On)

---
## The Installation of MySQL and MySQL workbench in Ubuntu
#### Here are the steps to install throuch terminal and Ubuntu Software

```bash


```


#### Here are the step to install MySQL and MySQL Workbench for window users

[Install MySQL Workbench in windows](https://www.youtube.com/watch?v=KMagIwoe4aY)

---

### Good Practices:
- Use uppercase letter to write commands.
- Use lowercase letter to write names.
- SQL is Case-Sensitive.


### These are the SQL commands:


```sql
-- To create a database

CREATE DATABASE SurajIsLearningSQL


-- To show existing databases
SHOW DATABASES



-- Create a databases if you are not sure that it exits
CREATE DATABASE IF NOT EXISTS SurajIsLearningSQL


-- To use the database
USE SurajIsLearningSQL


-- to know with what databse you are working with
SELECT DATABASE()

```

### CRUD Operations in SQL
- **C**reate: Add new data
- **R**ead: Retrieve data
- **U**pdate: Modify existing data
- **D**elete: Remove data




### DataTypes in SQL:
- **INT**: Deals with numeric data
- **varchar(30)**: textual string, and 30 here represents character length

### Constraints in SQL:
- **NOT NULL**: Whenever any of the columns name as I want ti mandatory field

- **Primary Key**: Used for uniquely identification and not need to mention NOT NULL it'll by default applicable.

- **Composite Primary Key**: A composite key is a primary key composed of two or more columns that together uniquely identify a row in a table. ``` PRIMARY KEY(SID,FirstName)```


```sql
-- To create a table
CREATE TABLE Students(
SID PRIMARY KEY,
SFristName varchar(30) NOT NULL,
SLastName varchar(30) NOT NULL,
SAge INT NOT NULL,
SAddress varchar(30) NOT NULL,
SPhone INT NOT NULL
-- PRIMANRY KEY(SID): This is the another way of writing it.
)
```