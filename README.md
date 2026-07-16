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


