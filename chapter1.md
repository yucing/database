# chapter1
# File-Based System
* Collection of application programs that perform services for the end users.
* Each program defines and manages its own data.

![](https://github.com/yucing/database/blob/main/picture/FBS.png)

# Limitations of File-Based Approach
## Separation and isolation of data
* Each program maintains its own set of data.
* Users of one program may be unaware of potentially (潛在的) useful data held by other programs.
## Duplication (複製) of data
* Same data is held by different programs.
* Wasted space and potentially different values and/or different formats for the same item.
## Data dependence
* File structure is defined in the program code.
## Incompatible file formats
* Programs are written in different languages, and so cannot easily access each other’s files.
## Fixed Queries/Proliferation of application programs
* Programs are written to satisfy particular functions.
* Any new requirement needs a new program.

# Database Approach
## Arose because:
* Definition of data was embedded in (嵌入) application programs, rather than being stored separately and independently.
* No control over access and manipulation (操控) of data beyond that (除了) imposed by (所規定) application programs.
## Result
* the database and Database Management System (DBMS).

# Database
* Shared collection of logically related data (and a description of this data), designed to meet the information needs of an organization.
* System catalog (metadata) provides description of data to enable program–data independence.
* Logically related data comprises entities, attributes, and relationships of an organization’s information.

# Database Management System (DBMS)
* A software system that enables users to define, create, maintain, and control access to the database.
* (Database) application program: a computer program that interacts with database by issuing an appropriate (合適的) request (SQL statement) to the DBMS.