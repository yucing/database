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

![](https://github.com/yucing/database/blob/main/picture/DBMS.png)

# Database Approach
## Data definition language (DDL).
* Permits specification of data types, structures and any data constraints.
* All specifications are stored in the database.
## Data manipulation (操控) language (DML).
* General enquiry facility (query language) of the data.
## Controlled access to database may include:
* a security system
* an integrity system (完整系統)
* a concurrency control system (並行控制系統)
* a recovery control system
* a user-accessible catalog. (使用者易使用的目錄)

# View
* Allows each user to have his or her own view of the database.
* A view is essentially some subset of the database.
## Benefit
* Reduce complexity
* Provide a level of security
* Provide a mechanism to customize (定制) the appearance of the database
* Present a consistent, unchanging picture of the structure of the database, even if the underlying database is changed

# Components of DBMS Environment

![](https://github.com/yucing/database/blob/main/picture/DBMS2.png)

## Hardware
* Can range from a PC to a network of computers.
## Software
* DBMS, operating system, network software (if necessary) and also the application programs.
## Data
* Used by the organization and a description of this data called the schema.
## Procedures
* Instructions and rules that should be applied to the design and use of the database and DBMS.
## People

# Roles in the Database Environment
* Data Administrator (DA)
* Database Administrator (DBA)
* Database Designers (Logical and Physical)
* Application Programmers
* End Users (naive and sophisticated)

# Advantages of DBMSs
* Control of data redundancy (資料冗餘)
* Data consistency
* More information from the same amount of data
* Sharing of data
* Improved data integrity (資料完整性)
* Improved security
* Enforcement of standards
* Economy of scale (規模經濟)
* Balance conflicting (牴觸) requirements
* Improved data accessibility and responsiveness
* Increased productivity
* Improved maintenance through data independence
* Increased concurrency
* Improved backup and recovery services

# Disadvantages of DBMSs
* Complexity
* Size
* Cost of DBMS
* Additional hardware costs
* Cost of conversion
* Performance
* Higher impact of a failure