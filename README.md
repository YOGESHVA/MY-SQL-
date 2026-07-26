# MY-SQL-
# Day 1 - Full Stack Development Fundamentals

## 📚 Topics Covered

### 🔹 What is Full Stack Development?

A **Full Stack Developer** is a developer who works on both:

* **Frontend** (Client Side)
* **Backend** (Server Side)

---

## 🌐 Frontend (Client Side)

Frontend is the visual and interactive part of a website or application that users directly see and interact with through a web browser or mobile application.

### Responsibilities

* Display web pages and user interfaces.
* Accept user input (forms, buttons, search boxes).
* Validate user input before sending it to the server.
* Call backend APIs to send and receive data.
* Display responses received from the backend.
* Provide animations and interactive effects.

### Technologies

* HTML
* CSS
* JavaScript
* Bootstrap

---

## ⚙️ Backend (Server Side)

Backend is the server-side part of an application. Users cannot see it directly, but it performs business logic, security, data processing, and database operations.

It acts as the **brain of the application**.

### Responsibilities

* Process client requests.
* Implement business logic.
* Connect with databases.
* Perform CRUD operations.
* Authenticate and authorize users.
* Encrypt passwords.
* Generate reports.
* Return responses to the frontend.

### Backend Languages

* Python
* Java
* .NET
* C++

---

## 🔗 API (Application Programming Interface)

An **API** is a set of rules and protocols that allows different applications or systems to communicate and exchange data without exposing their internal implementation.

It acts as a bridge between the frontend and backend or between different software systems.

### Advantages

* Enables communication between different systems.
* Promotes code reusability.
* Platform independent.
* Faster application development.
* Supports third-party integrations.
* Improves scalability.
* Easy to maintain.

---

## 💾 Storage Areas

Applications need storage to save customer information, billing details, call records, and more.

### 1. Temporary Storage

Stores data temporarily in memory.

**Examples**

* Heap Memory
* Stack Memory
* Method Area
* Program Counter (PC)
* Registers
* Native Method Stack

> Data is automatically cleared when the application or JVM stops.

### 2. Permanent Storage

Stores data permanently.

**Examples**

* File System
* Databases
* Data Warehouses

---

# 📁 File Management System (FMS)

A File Management System stores data in files on the operating system. Each application manages its own storage, retrieval, and updating of data.

### Example

* books.txt
* members.txt

### Advantages

* Easy to use.
* Suitable for storing small amounts of data.
* Simple implementation.

### Limitations

* Data Redundancy
* Data Inconsistency
* Poor Security
* Difficult Data Retrieval
* Integrity Issues
* Scalability Problems

➡️ These limitations led to the development of **Database Management Systems (DBMS).**

---

# 🗄️ DBMS (Database Management System)

A DBMS is software that allows users to create, manage, and manipulate databases.

It acts as an interface between users and the database.

### Advantages

* Stores large amounts of structured data.
* Supports SQL for database operations.
* Provides authentication using usernames and passwords.
* Maintains data integrity through constraints.
* Reduces data redundancy using normalization.
* Supports Primary Key, Foreign Key, Unique Key, and other constraints.

### Limitations

* Not suitable for extremely large-scale data (TBs/PBs).
* Mainly supports structured (relational) data.
* Limited support for semi-structured and unstructured data such as videos, images, and audio.

➡️ To handle massive datasets and unstructured data, technologies such as **Data Warehouses** and **Big Data** platforms are used.

---

## 🎯 Key Takeaways

* Understood the architecture of Full Stack Development.
* Learned the responsibilities of Frontend and Backend.
* Explored APIs and their importance in communication.
* Learned different storage types.
* Understood File Management Systems and their limitations.
* Learned the basics of DBMS, its advantages, and limitations.

---

## 🚀 Day 1 Complete

**Next Topics:** SQL, Database Design, RDBMS, MySQL, and CRUD Operations.

# 📅 Day 2 - Database Management System (DBMS)

## 📚 Topics Covered

### 📁 File Management System (FMS) vs Database Management System (DBMS)

| File Management System                | Database Management System                         |
| ------------------------------------- | -------------------------------------------------- |
| High data redundancy (duplicate data) | Reduces data redundancy                            |
| Difficult to maintain and update      | Easy to maintain and update                        |
| Limited security                      | Provides strong security mechanisms                |
| Data sharing is difficult             | Multiple users can access data simultaneously      |
| No relationship between files         | Supports relationships between tables              |
| Backup and recovery are difficult     | Provides backup and recovery features              |
| Suitable for small applications       | Suitable for small, medium, and large applications |

### 📌 Summary

A **File Management System (FMS)** stores data in separate files, which can lead to data redundancy, inconsistency, and security issues.

A **Database Management System (DBMS)** stores data in a structured format using tables. It minimizes redundancy, provides better security, supports multiple users, and maintains data consistency and integrity.

---

# 📖 Basic Database Terminology

### 🔹 Data

Raw facts or figures without context.

**Example**

```
101, Yogesh, 6000, Hyderabad
```

---

### 🔹 Field (Column/Attribute)

The smallest unit of data in a database.

**Examples**

* EmpID
* EmpName
* EmpSalary
* EmpAddress

---

### 🔹 Record (Row/Tuple)

A collection of related fields representing a single entity.

**Example**

```
(101, Yogesh, 6000, Hyderabad)
```

---

### 🔹 Database

An organized collection of related records stored together.

**Example**
An Employee Database containing employee details.

---

# 🗄️ What is DBMS?

A **Database Management System (DBMS)** is software used to:

* Create databases
* Store data
* Retrieve data
* Update data
* Manage databases efficiently

---

# 🖥️ Client-Server Architecture

A Client-Server Architecture consists of three main components:

## 1️⃣ Client

* Sends requests to the server.
* Receives responses from the server.

## 2️⃣ Server

* Accepts client requests.
* Processes valid requests.
* Returns the required response.
* Generates errors for invalid requests.

## 3️⃣ Protocol

A protocol is a set of rules that enables communication between the client and the server by transferring requests and responses.

---

# 📊 Data Models in DBMS

A **Data Model** defines how data is stored, organized, and manipulated in a database.

## 1. Physical Data Model

**Definition**
Describes how data is physically stored on storage devices.

**Audience**

* Database Administrators (DBAs)

---

## 2. Logical Data Model

**Definition**
Defines the structure of data, including entities, attributes, and relationships, independent of physical storage.

**Audience**

* Developers
* Database Architects

---

## 3. Hierarchical Data Model

**Definition**
Represents data in a tree-like parent-child structure.

**Example**

```
Company
 └── Department
      └── Employee
```

---

## 4. Network Data Model

**Definition**
Represents data as a graph using nodes and relationships.

**Example**

* Students can enroll in multiple courses.
* Courses can be taught by multiple professors.

---

## 5. Relational Data Model (RDBMS)

**Definition**
Stores data in tables consisting of rows (tuples) and columns (attributes).

### Example

**Student Table**

| Student_ID | Name   | Marks | Dept_ID |
| ---------- | ------ | ----- | ------- |
| 101        | Yogesh | 95    | D01     |

**Department Table**

| Dept_ID | Dept_Name        |
| ------- | ---------------- |
| D01     | Computer Science |

---

# 🎯 Key Takeaways

* Learned the differences between File Management Systems and DBMS.
* Understood database concepts such as Data, Field, Record, and Database.
* Explored the purpose and features of a DBMS.
* Learned the Client-Server Architecture.
* Studied different Data Models used in database systems.
* Introduced to the Relational Data Model (RDBMS).

---

# 🚀 Day 2 Complete

### Topics Learned

* ✅ File Management System vs DBMS
* ✅ Basic Database Terminology
* ✅ DBMS Overview
* ✅ Client-Server Architecture
* ✅ Data Models in DBMS

### Next Topics

* SQL
* RDBMS Concepts
* MySQL Installation
* CRUD Operations
* SQL Queries (DDL, DML, DCL, TCL)
  # 📅 Day 3 - SQL Fundamentals

## 📚 Topics Covered

### 🏷️ SQL Identifiers

SQL Identifiers are names used to identify database objects such as:

* Database Names
* Table Names
* Column Names
* View Names
* Index Names
* Constraints
* Triggers
* Stored Procedures

### Rules for SQL Identifiers

1. Only the following characters are allowed:

   * `A-Z`
   * `a-z`
   * `0-9`
   * `_`
   * `$`
2. An identifier must begin with a letter or an underscore (`_`).
3. Reserved keywords cannot be used as identifiers.
4. Spaces are not allowed in identifiers.
5. Identifiers are generally case-sensitive depending on the database system.
6. Maximum identifier length is typically **15 characters** (may vary by DBMS).

---

# 🗄️ What is SQL?

**SQL (Structured Query Language)** is a standardized programming language used to manage and manipulate relational databases.

It allows users to:

* Create databases and tables.
* Insert, update, and delete records.
* Retrieve data.
* Manage permissions.
* Control transactions.

SQL is a **declarative language**, meaning users specify **what** data they want rather than **how** the database should retrieve it.

---

# 📖 SQL Commands

SQL commands are divided into five categories.

---

## 1️⃣ DDL (Data Definition Language)

DDL commands define and modify database objects.

### Commands

### CREATE

Creates new database objects.

**Examples**

* Database
* Table
* View
* Index

---

### ALTER

Modifies the structure of an existing table.

Operations include:

* Add Column
* Drop Column
* Rename Column
* Modify Data Type
* Add or Remove Constraints

---

### DROP

Deletes database objects permanently.

Examples:

* Database
* Table
* View
* Index

---

### TRUNCATE

Deletes all records from a table without deleting the table structure.

---

### RENAME

Renames database objects.

---

# 2️⃣ DML (Data Manipulation Language)

Used to manage data stored inside tables.

### INSERT

Adds new records to a table.

### UPDATE

Modifies existing records based on a condition.

### DELETE

Removes records based on a condition.

### LOCK

Controls concurrent access by locking tables during modifications.

---

# 3️⃣ DCL (Data Control Language)

Used to control permissions and access.

### GRANT

Provides permissions such as:

* SELECT
* INSERT
* UPDATE
* DELETE
* ALL PRIVILEGES

### REVOKE

Removes previously granted permissions from users or roles.

---

# 4️⃣ TCL (Transaction Control Language)

Manages transactions to maintain data integrity.

### COMMIT

Permanently saves all changes made during the current transaction.

### ROLLBACK

Undoes changes and restores the database to the last committed state or a savepoint.

### SAVEPOINT

Creates a checkpoint within a transaction to allow partial rollback.

---

# 5️⃣ DQL (Data Query Language)

Used to retrieve data from database tables.

### SELECT

Retrieves data from one or more tables based on specified columns and conditions.

This is the most frequently used SQL command.

---

# 💻 Basic SQL Syntax

## Create a Database

```sql
CREATE DATABASE database_name;
```

### Example

```sql
CREATE DATABASE pfs4;
```

---

## Drop a Database

```sql
DROP DATABASE database_name;
```

### Example

```sql
DROP DATABASE pfs4;
```

---

## Create a Table

```sql
CREATE TABLE table_name (
    column_name datatype(size) constraint,
    column_name datatype(size),
    column_name datatype(size),
    column_name datatype(size),
    column_name datatype(size)
);
```

### Example

```sql
CREATE TABLE Employee (
    EmpID INT PRIMARY KEY,
    EmpName VARCHAR(50),
    Salary DECIMAL(10,2),
    Department VARCHAR(30),
    City VARCHAR(30)
);
```

---

# 🎯 Key Takeaways

* Learned SQL Identifiers and their naming rules.
* Understood the purpose of SQL.
* Studied the five categories of SQL commands:

  * DDL
  * DML
  * DCL
  * TCL
  * DQL
* Learned how to create and drop databases.
* Learned the syntax for creating tables.

---

# 🚀 Day 3 Complete

### Topics Learned

* ✅ SQL Identifiers
* ✅ Introduction to SQL
* ✅ DDL Commands
* ✅ DML Commands
* ✅ DCL Commands
* ✅ TCL Commands
* ✅ DQL Commands
* ✅ Create Database
* ✅ Drop Database
* ✅ Create Table

### Next Topics

* SQL Data Types
* Constraints
* INSERT Statement
* SELECT Statement
* WHERE Clause
* ORDER BY
* Aggregate Functions
# 📅 Day 4 - SQL Data Types & ALTER TABLE

## 📚 Topics Covered

### 🗄️ Database Operations

* Created new databases.
* Displayed available databases using `SHOW DATABASES`.
* Switched between databases using `USE`.
* Dropped databases using `DROP DATABASE`.

---

# 📋 Table Creation

Created an **EMPLOYEES** table using different SQL data types.

### Data Types Learned

* `CHAR`
* `VARCHAR`
* `INT`
* `DATE`
* `TINYTEXT`

Also learned how to display table structure using:

* `DESC table_name`
* `SHOW COLUMNS FROM table_name`

---

# 📊 SQL Data Types

### Numeric Data Types

* TINYINT
* SMALLINT
* INT
* DECIMAL

### Character Data Types

* CHAR
* VARCHAR
* TINYTEXT

### Date & Time Data Types

* DATE

### Special Data Types

* ENUM
* SET

---

# 🔄 ALTER TABLE

Learned different operations using the `ALTER TABLE` command.

## ➕ Add Column

Added new columns to an existing table.

Examples:

* LOCATION
* EMAIL
* PHONE_NUMBER
* BONUS
* STATUS
* COMPANY_NAME
* QUALIFICATION

---

## 📍 Add Column at Specific Position

Used:

* `FIRST`
* `AFTER column_name`

---

## ✏️ Modify Column

Modified:

* Data type
* Column size

Examples:

* Changed `FNAME` size.
* Updated `SALARY` datatype to `DECIMAL(20,3)`.

---

## 🔄 Rename Column

Used the `CHANGE` command to rename columns.

Examples:

* FNAME → FIRSTNAME
* LNAME → LASTNAME
* EMP_NAME → EMPLOYEE_NAME
* JOINING_DATE → DATE_OF_JOINING

---

## ❌ Drop Column

Removed unnecessary columns.

Examples:

* BONUS
* PHONE_NUMBER
* PEFID
* LOCATION

---

## 📝 Rename Table

Renamed tables using:

```sql
ALTER TABLE old_table_name
RENAME TO new_table_name;
```

Example:

* EMPLOYEES → CODEGNAN_EMP
* CODEGNAN_EMP → EMPLOYEES
* COMPANY_STAFF → STAFF_RECORDS
* STAFF_RECORDS → COMPANY_STAFF

---

# 👨‍💻 Company Staff Table

Created a sample **COMPANY_STAFF** table using multiple SQL data types.

### Columns Included

* Company Name
* Employee ID
* Employee Name
* Qualification
* Age
* Experience
* Gender
* Address
* Salary
* Department
* Status
* Skills
* Last Updated
* Date of Joining
* Email

---

# ⚠️ Errors Practiced

While learning SQL, I also encountered and corrected several common errors:

* Misspelled SQL commands.
* Invalid database names.
* Missing commas.
* Incorrect SQL syntax.
* Wrong data type names.
* Incorrect `ALTER TABLE` syntax.
* Attempting to query non-existing tables.

Learning from these mistakes helped me better understand SQL syntax and debugging.

---

# 🎯 Key Takeaways

* Learned SQL Data Types.
* Created databases and tables.
* Explored `SHOW`, `DESC`, and `SHOW COLUMNS`.
* Practiced `ALTER TABLE` extensively.
* Added, modified, renamed, and dropped columns.
* Renamed tables.
* Worked with `ENUM` and `SET` data types.
* Improved SQL debugging skills by fixing syntax errors.

---

# 🚀 Day 4 Complete

### Topics Learned

* ✅ SQL Data Types
* ✅ CREATE DATABASE
* ✅ CREATE TABLE
* ✅ SHOW DATABASES
* ✅ SHOW TABLES
* ✅ DESC
* ✅ SHOW COLUMNS
* ✅ ALTER TABLE
* ✅ ADD COLUMN
* ✅ MODIFY COLUMN
* ✅ CHANGE COLUMN
* ✅ DROP COLUMN
* ✅ RENAME TABLE
* ✅ ENUM
* ✅ SET
* ✅ SQL Error Debugging

### Next Topics

* INSERT Statement
* UPDATE Statement
* DELETE Statement
* SELECT Statement
* WHERE Clause
* ORDER BY
* Aggregate Functions
* Constraints (Primary Key, Foreign Key, Unique, Check)
# 📅 Day 5 - SQL DML Commands

## 📚 Topics Covered

### 🔹 What is DML?

**DML (Data Manipulation Language)** is used to manage and manipulate the data stored in database tables.

It allows users to:

* Insert new records
* Update existing records
* Delete records
* Retrieve data

---

# 📥 INSERT Command

The `INSERT` statement is used to add new records into a table.

### Syntax

```sql
INSERT INTO table_name (column1, column2, column3)
VALUES (value1, value2, value3);
```

### Example

```sql
INSERT INTO Employees
VALUES
(101,'Yogesh','Developer',50000),
(102,'Vinod','Tester',45000),
(103,'Lokesh','Manager',70000);
```

---

# ✏️ UPDATE Command

The `UPDATE` statement is used to modify existing records.

### Syntax

```sql
UPDATE table_name
SET column_name = value
WHERE condition;
```

### Example

```sql
UPDATE Employees
SET Salary = 60000
WHERE EmpID = 101;
```

---

# ❌ DELETE Command

The `DELETE` statement removes selected records from a table.

### Syntax

```sql
DELETE FROM table_name
WHERE condition;
```

### Example

```sql
DELETE FROM Employees
WHERE EmpID = 102;
```

---

# 🔍 SELECT Command

The `SELECT` statement retrieves data from one or more tables.

### Syntax

```sql
SELECT * FROM table_name;
```

### Example

```sql
SELECT * FROM Employees;
```

---

# 📊 Difference Between DELETE, TRUNCATE, and DROP

| Feature         | DELETE                 | TRUNCATE               | DROP                  |
| --------------- | ---------------------- | ---------------------- | --------------------- |
| Command Type    | DML                    | DDL                    | DDL                   |
| Deletes         | Selected rows          | All rows               | Entire table/database |
| WHERE Clause    | ✅ Yes                  | ❌ No                   | ❌ No                  |
| Table Structure | Remains                | Remains                | Deleted               |
| Rollback        | Possible before COMMIT | Generally not possible | Not possible          |
| Speed           | Slow                   | Fast                   | Fastest               |
| Auto Increment  | Not Reset              | Reset (Most DBMS)      | Removed               |

---

# 📝 SQL Queries Practiced

## Insert Records

```sql
INSERT INTO Employees
VALUES (104,'Rahul','HR',40000);
```

## View Records

```sql
SELECT * FROM Employees;
```

## Update Records

```sql
UPDATE Employees
SET Salary = 55000
WHERE EmpID = 104;
```

## Delete Records

```sql
DELETE FROM Employees
WHERE EmpID = 104;
```

## Delete All Records

```sql
DELETE FROM Employees;
```

## Remove All Records Quickly

```sql
TRUNCATE TABLE Employees;
```

## Delete Table

```sql
DROP TABLE Employees;
```

## Delete Database

```sql
DROP DATABASE CompanyDB;
```

---

# 🎯 Key Takeaways

* Learned DML commands.
* Inserted records into tables.
* Updated existing records.
* Deleted records using conditions.
* Retrieved records using the `SELECT` statement.
* Understood the differences between `DELETE`, `TRUNCATE`, and `DROP`.

---

# 🚀 Day 5 Complete

### Topics Learned

* ✅ INSERT
* ✅ UPDATE
* ✅ DELETE
* ✅ SELECT
* ✅ DELETE vs TRUNCATE vs DROP
* ✅ SQL Query Practice

### Next Topics

* DCL (GRANT & REVOKE)
* User Management
* Transaction Control Language (TCL)
* COMMIT
* ROLLBACK
* SAVEPOINT
# 📅 Day 6 - Data Control Language (DCL)

## 📚 Topics Covered

### 🔐 What is DCL?

**Data Control Language (DCL)** is used to manage permissions and access control in a database. It allows database administrators to grant or revoke privileges for users and roles.

---

# 🏗️ Database Setup

* Created a new database.
* Created tables with `AUTO_INCREMENT` and `PRIMARY KEY`.
* Inserted sample records into tables.
* Created a backup table using `CREATE TABLE ... AS SELECT`.

---

# 📊 Generated Columns

Learned how to create a generated column that automatically calculates values.

### Example

```sql
CREATE TABLE Products(
    ProductID INT AUTO_INCREMENT PRIMARY KEY,
    ProductName VARCHAR(20),
    Price DECIMAL(10,2),
    Quantity INT,
    TotalAmount DECIMAL(10,2)
    GENERATED ALWAYS AS (Price * Quantity) STORED
);
```

---

# 👨‍🎓 Student Table

Created a **Students** table and inserted sample student records.

### Columns

* StudentID
* Student Name
* Mobile Number
* Marks

---

# 👤 Creating Database Users

### Syntax

```sql
CREATE USER username IDENTIFIED BY 'password';
```

### Examples

```sql
CREATE USER YOGESH IDENTIFIED BY 'Yogesh@29';

CREATE USER VINOD IDENTIFIED BY 'varma@29';

CREATE USER CHYTU IDENTIFIED BY 'LoKesh@29';
```

---

# 🔑 GRANT Command

Used to provide permissions to database users.

### Syntax

```sql
GRANT privilege_name
ON table_name
TO username;
```

### Examples

```sql
GRANT SELECT, INSERT, UPDATE
ON STUDENTS
TO YOGESH;

GRANT SELECT, DELETE
ON STUDENTS
TO VINOD;

GRANT ALL PRIVILEGES
ON STUDENTS
TO CHYTU;
```

---

# ❌ REVOKE Command

Used to remove permissions from users.

### Syntax

```sql
REVOKE privilege_name
ON table_name
FROM username;
```

### Examples

```sql
REVOKE INSERT, UPDATE
ON STUDENTS
FROM YOGESH;

REVOKE DELETE
ON STUDENTS
FROM VINOD;
```

---

# 🧪 Permission Testing

Verified user permissions by logging in with different accounts.

### User: YOGESH

* ✅ SELECT
* ✅ INSERT (before REVOKE)
* ✅ UPDATE (before REVOKE)
* ❌ INSERT (after REVOKE)
* ❌ UPDATE (after REVOKE)

---

### User: VINOD

* ✅ SELECT
* ✅ DELETE (before REVOKE)
* ❌ DELETE (after REVOKE)

---

# 🎯 Key Takeaways

* Learned the purpose of Data Control Language (DCL).
* Created database users.
* Granted privileges using the `GRANT` command.
* Removed permissions using the `REVOKE` command.
* Practiced user authentication and access control.
* Tested user permissions by logging in with different database accounts.

---

# 🚀 Day 6 Complete

### Topics Learned

* ✅ DCL (Data Control Language)
* ✅ CREATE USER
* ✅ GRANT
* ✅ REVOKE
* ✅ AUTO_INCREMENT
* ✅ PRIMARY KEY
* ✅ Generated Columns
* ✅ User Privilege Management
* ✅ Permission Testing

### Next Topics

* Transaction Control Language (TCL)
* COMMIT
* ROLLBACK
* SAVEPOINT
* SQL Constraints
* Joins
# 📅 Day 7 - Transaction Control Language (TCL) & Database Locking

## 📚 Topics Covered

### 🔹 What is TCL (Transaction Control Language)?

Transaction Control Language (TCL) is used to manage transactions in a database and maintain data integrity.

A **transaction** is a group of related operations executed as a single unit of work following the principle:

> **"Either all operations succeed or none succeed."**

A common example is a **bank fund transfer**, where the debit and credit operations must both complete successfully to maintain consistency.

---

# 🔄 Types of Transactions

## 1. Local Transaction

* All operations are executed within the same database.
* Example: Money transfer between two accounts in the same bank.

## 2. Global Transaction

* Operations are executed across multiple databases.
* Example: Money transfer between accounts in different banks.

---

# 🛡️ ACID Properties

### 🔹 Atomicity

Ensures that all operations in a transaction are completed successfully or none are applied.

### 🔹 Consistency

Keeps the database in a valid and consistent state before and after every transaction.

### 🔹 Isolation

Ensures that multiple transactions do not interfere with each other.

### 🔹 Durability

Once a transaction is committed, the changes remain permanent even if the system fails.

---

# 📌 TCL Commands

## COMMIT

Permanently saves all changes made during the current transaction.

### Syntax

```sql
COMMIT;
```

---

## ROLLBACK

Reverts all changes made during the current transaction.

### Syntax

```sql
ROLLBACK;
```

---

## SAVEPOINT

Creates a checkpoint within a transaction so you can roll back to a specific point instead of the beginning.

### Syntax

```sql
SAVEPOINT savepoint_name;
```

### Rollback to Savepoint

```sql
ROLLBACK TO savepoint_name;
```

---

# 🧪 SQL Queries Practiced

## Start a Transaction

```sql
START TRANSACTION;
```

## Insert Records

```sql
INSERT INTO EMPLOYEE
VALUES (111,'MALLI',60000);

INSERT INTO EMPLOYEE
VALUES (222,'ARJUN',75000);
```

## Commit Changes

```sql
COMMIT;
```

## Update Records

```sql
UPDATE EMPLOYEE
SET EMPSALARY = 10000
WHERE EMP = 111;
```

## Rollback Changes

```sql
ROLLBACK;
```

## Create Savepoint

```sql
SAVEPOINT SF1;
```

## Delete Record

```sql
DELETE FROM EMPLOYEE
WHERE EMP = 111;
```

## Rollback to Savepoint

```sql
ROLLBACK TO SF1;
```

---

# 🔐 Database Locking

Locking is a mechanism used by databases to control concurrent access and maintain data consistency.

## 1. Shared Lock

* Allows multiple users to read data simultaneously.
* Prevents updates and deletes while the lock is active.

### Example

```sql
LOCK TABLES EMPLOYEE READ;
```

---

## 2. Exclusive Lock

* Allows only one transaction to modify data.
* Blocks other transactions from reading (locking reads) or writing.

### Example

```sql
LOCK TABLES EMPLOYEE WRITE;
```

---

## Unlock Tables

```sql
UNLOCK TABLES;
```

---

## 3. Intent Lock

An Intent Lock is automatically managed by MySQL to indicate that row-level locks will be placed within a table.

It helps improve locking efficiency and conflict detection.

---

# 🛠️ Hands-on Practice

* Created an Employee table.
* Started transactions using `START TRANSACTION`.
* Inserted employee records.
* Used `COMMIT` to save changes permanently.
* Used `ROLLBACK` to undo transactions.
* Created and used `SAVEPOINT`.
* Practiced `LOCK TABLES` with READ and WRITE locks.
* Released locks using `UNLOCK TABLES`.
* Corrected SQL syntax errors while practicing transaction management.

---

# 🎯 Key Takeaways

* Learned Transaction Control Language (TCL).
* Understood Local and Global Transactions.
* Studied ACID properties.
* Practiced COMMIT, ROLLBACK, and SAVEPOINT.
* Learned database locking mechanisms.
* Explored Shared, Exclusive, and Intent Locks.
* Improved SQL debugging through hands-on practice.

---

# 🚀 Day 7 Complete

### Topics Learned

* ✅ TCL (Transaction Control Language)
* ✅ Transactions
* ✅ ACID Properties
* ✅ COMMIT
* ✅ ROLLBACK
* ✅ SAVEPOINT
* ✅ Database Locking
* ✅ Shared Lock
* ✅ Exclusive Lock
* ✅ Intent Lock
* ✅ LOCK TABLES
* ✅ UNLOCK TABLES

### Next Topics

* SQL Constraints
* Joins
* Functions
* Views
* Indexes
# 📅 Day 8 - SQL Constraints & Operators

## 📚 Topics Covered

### 🔹 What are Constraints?

Constraints are rules applied to table columns to ensure that only valid and accurate data is stored in the database.

### Why do we use Constraints?

* Maintain data integrity
* Prevent invalid data entry
* Avoid duplicate records
* Ensure relationships between tables
* Make the database reliable and consistent

---

# 🔒 Types of Constraints

## 1. NOT NULL

Prevents NULL values from being inserted into a column.

### Example

```sql
CREATE TABLE students_1(
    sno INT NOT NULL,
    sname VARCHAR(30),
    marks INT
);
```

---

## 2. UNIQUE

Ensures that duplicate values are not allowed, while NULL values are generally permitted.

### Example

```sql
CREATE TABLE students_2(
    sno INT UNIQUE,
    sname VARCHAR(30),
    marks INT
);
```

---

## 3. PRIMARY KEY

A combination of **NOT NULL** and **UNIQUE**.

* Does not allow NULL values.
* Does not allow duplicate values.

### Example

```sql
CREATE TABLE Employee(
    emp_id CHAR(5) PRIMARY KEY,
    emp_name VARCHAR(30),
    emp_salary DECIMAL(10,2)
);
```

---

## 4. COMPOSITE KEY

A Primary Key created using multiple columns.

### Example

```sql
CREATE TABLE Cricketers(
    player_id CHAR(5),
    player_name VARCHAR(30),
    score INT,
    PRIMARY KEY(player_id, player_name)
);
```

---

## 5. FOREIGN KEY

A Foreign Key creates a relationship between two tables.

### Example

```sql
CREATE TABLE Orders(
    order_id INT PRIMARY KEY,
    customer_id INT,
    FOREIGN KEY(customer_id)
    REFERENCES Customers(customer_id)
);
```

---

## Referential Actions

* ON DELETE CASCADE
* ON UPDATE CASCADE
* ON DELETE SET NULL
* ON UPDATE SET NULL

---

## 6. CHECK

Allows only values that satisfy a specified condition.

### Example

```sql
CREATE TABLE Exams(
    student_id INT,
    marks INT CHECK(marks BETWEEN 0 AND 100)
);
```

---

## 7. DEFAULT

Assigns a default value when no value is provided.

### Example

```sql
CREATE TABLE Customers(
    customer_id INT PRIMARY KEY,
    customer_name VARCHAR(50),
    city VARCHAR(50) DEFAULT 'Hyderabad'
);
```

---

## 8. AUTO_INCREMENT

Automatically generates unique numeric values for a column.

### Example

```sql
CREATE TABLE Employees(
    emp_id INT AUTO_INCREMENT PRIMARY KEY,
    emp_name VARCHAR(50)
);
```

---

# ➕ SQL Operators Practice

Created a **Products** table and practiced arithmetic operations.

### Examples

Calculate price with 12% tax

```sql
SELECT name,
       price,
       price + (price * 0.12) AS price_with_tax
FROM Products;
```

Discounted Price

```sql
SELECT name,
       price,
       (price - 5) AS discounted_price
FROM Products;
```

Total Product Value

```sql
SELECT name,
       price,
       (price * qty) AS total_product
FROM Products;
```

Multiply Price

```sql
SELECT name,
       price,
       (price * 10) AS total_price
FROM Products;
```

Modulo Operator

```sql
SELECT name,
       price,
       qty,
       (qty % 50 != 0) AS total_quantity
FROM Products;
```

---

# 🎯 Key Takeaways

* Learned SQL Constraints.
* Practiced NOT NULL, UNIQUE, PRIMARY KEY, COMPOSITE KEY, FOREIGN KEY, CHECK, DEFAULT, and AUTO_INCREMENT.
* Understood Referential Integrity and Referential Actions.
* Worked with arithmetic and modulo operators.
* Practiced SQL queries and corrected syntax errors during execution.

---

# 🚀 Day 8 Complete

### Topics Learned

* ✅ NOT NULL
* ✅ UNIQUE
* ✅ PRIMARY KEY
* ✅ COMPOSITE KEY
* ✅ FOREIGN KEY
* ✅ CHECK
* ✅ DEFAULT
* ✅ AUTO_INCREMENT
* ✅ Referential Actions
* ✅ SQL Operators

### Next Topics

* SQL Functions
* Aggregate Functions
* String Functions
* Date Functions
* Joins
* Views


