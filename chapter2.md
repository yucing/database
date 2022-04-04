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