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

# Data Model
* Integrated (整合) collection of concepts for describing data, relationships between data, and constraints (約束) on the data in an organization.
## Data Model comprises:
* a structural part.
* a manipulative (操作性的) part.
* possibly a set of integrity rules.
## Purpose
* To represent data in an understandable way.
## Categories of data models include:
* Object-based.
* Record-based.
* Physical.
## Object-Based Data Models
* Entity-Relationship
* Semantic (語意)
* Functional
* Object-Oriented.
## Record-Based Data Models
* Relational Data Model

![](https://github.com/yucing/database/blob/main/picture/RDM.png)

* Network Data Model

![](https://github.com/yucing/database/blob/main/picture/NDM.png)

* Hierarchical (分層的) Data Model.

![](https://github.com/yucing/database/blob/main/picture/HDM.png)

## Physical Data Models

# Conceptual Modeling 概念模型
* Conceptual schema is the core of a system supporting all user views.
* Should be complete and accurate representation of an organization’s data requirements.
* Conceptual modeling is process of developing a model of information use that is independent of implementation (執行) details.
* Result is a conceptual data model.

# Functions of a DBMS
* Data Storage, Retrieval, and Update.
* A User-Accessible Catalog.
* Transaction Support.
* Concurrency Control Services.
* Recovery Services.
* Authorization Services.
* Support for Data Communication.
* Integrity Services.
* Services to Promote (推動) Data Independence.
* Utility Services.(公用事業服務)

# System Catalog
* Repository (儲存庫) of information (metadata) describing the data in the database.
* One of the fundamental (基礎的) components (零件) of DBMS.
## Typically stores:
* names, types, and sizes of data items;
* constraints on the data;
* names of authorized users;
* data items accessible by a user and the type of access;
* usage statistics (統計).

# Componenets of a DBMS

![](https://github.com/yucing/database/blob/main/picture/compenent.png)

# Componenets of Database Manager

![](https://github.com/yucing/database/blob/main/picture/compenent2.png)

# Multi-User DBMS Architectures
## Teleprocessing
* Traditional architecture.
* Single mainframe (大型電腦) with a number of terminals attached.
* Trend is now towards downsizing (縮小).

![](https://github.com/yucing/database/blob/main/picture/teleprocessing.png)

## File-server
* File-server is connected to several workstations across a network.
* Database resides (居住) on file-server.
* DBMS and applications run on each workstation.
### Disadvantages include:
* Significant network traffic.
* Copy of DBMS on each workstation.
* Concurrency, recovery and integrity control more complex.
## Client-server

![](https://github.com/yucing/database/blob/main/picture/file-server.png)