# chapter2

# Objectives of Three-Level Architecture
* All users should be able to access same data.
* A user’s view is immune to (免疫) changes made in other views.
* Users should not need to know physical database storage details.
* DBA should be able to change database storage structures without affecting the users’ views.
* Internal (內部的) structure of database should be unaffected by changes to physical aspects (方面) of storage.
* DBA should be able to change conceptual (概念的) structure of database without affecting all users.

# ANSI-SPARC Three-Level Architecture

![](https://github.com/yucing/database/blob/main/picture/TLA.png)

## External Level
* Users’ view of the database.
* Describes that part of database that is relevant to (相關) a particular user.
## Conceptual Level
* Community view of the database.
* Describes what data is stored in database and relationships among the data.
## Internal Level
* Physical representation of the database on the computer.
* Describes how the data is stored in the database. 

![](https://github.com/yucing/database/blob/main/picture/TLA2.png)

# Data Independence
## Logical Data Independence
* Refers to immunity of external schemas to changes in conceptual schema.
* Conceptual schema changes (e.g. addition/removal of entities).
* Should not require changes to external schema or rewrites of application programs.
## Physical Data Independence
* Refers to immunity of conceptual schema to changes in the internal schema.
* Internal schema changes (e.g. using different file organizations, storage structures/devices).
* Should not require change to conceptual or external schemas.

![](https://github.com/yucing/database/blob/main/picture/TLA3.png)

# Database Languages
## Data Definition Language (DDL)
* Allows the DBA or user to describe and name entities, attributes, and relationships
required for the application
* plus any associated integrity and security constraints (約束).
## Data Manipulation Language (DML)
* Provides basic data manipulation operations on data held in the database.
## Procedural DML
* allows user to tell system exactly how to manipulate data.
## Non-Procedural DML
* allows user to state what data is needed rather than how it is to be retrieved.
## Fourth Generation Languages (4GLs)

# Data Mode
* Integrated collection of concepts for describing data, relationships between data, and constraints on the data in an organization.