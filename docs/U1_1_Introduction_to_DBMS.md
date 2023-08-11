---
title:  "Introduction to DBMS"
---
# Introduction to DMBS.

Last year, in the Database Management module we learned how to design, create and manipulate databases using SQL DDL (Data Definition Language) and DML (Data Manipulation Language). In this module we will learn how to use the tool that allows us to implement databases, that is a DataBase Management System or DBMS.

## Functions of the database management system (DBMS).

The functions of the database management system (DBMS) are as follows:

- **Data storage and retrieval**: The DBMS is responsible for storing and retrieving data from the database. It provides a mechanism for creating, reading, updating, and deleting data.

- **Concurrency control**: The DBMS must ensure that multiple users can access the database at the same time without interfering with each other. To do this, the DBMS uses concurrency control techniques to ensure that each user can work with the data safely.

- **Integrity control**: The DBMS is responsible for maintaining the integrity of the data in the database. This means that the data must be accurate and consistent at all times. The DBMS must ensure that the data is not corrupted or becomes inaccurate due to system failures or human errors.

- **Security control**: The DBMS is responsible for ensuring that the data in the database is protected against unauthorized access. This includes user authentication, authorization of database access, and implementation of security policies.

## Components.

We could summarize the components of a DBMS are as follows:

- **Database engine**: It is the core of the DBMS. It controls all database operations, including data storage and retrieval, concurrency control, integrity control, and security control.

- **Query language**: Allows users to perform queries and data manipulations in the database. Examples of query languages are SQL, PL/SQL, T-SQL, etc.

- **User interface**: Allows users to interact with the DBMS. It can be a graphical user interface (GUI), a command line, an API, etc.

- **Administration tools**: Allow database administrators to manage the database and perform tasks such as creating and modifying tables, assigning user permissions, performing backups, etc.

## Types.

There are different types of DBMS, among which are:

- Relational DBMS: Store data in relational tables and use SQL as query language. Examples of relational DBMS are Oracle, MySQL, Microsoft SQL Server, etc.

- NoSQL DBMS: Do not use relational tables to store data. Instead, they use non-relational data structures such as documents, graphs, or columns. Examples of NoSQL DBMS are MongoDB, Cassandra, Couchbase, etc.

- Desktop DBMS: Are DBMS that run on a desktop or laptop computer. Examples of desktop DBMS are Microsoft Access, FileMaker Pro, etc.

- Cloud DBMS: Are DBMS that run in the cloud and are accessible over the Internet. Examples of cloud DBMS are Amazon RDS, Microsoft Azure SQL Database, Google Cloud SQL, etc.

## DBMS Architecture.

We could also make a classification of DBMS according to the number of layers between the user and the database. There are three types of DBMS (Database Management System):

- **Single Layer DBMS**: there is only one layer between the user and the database. This layer provides an interface to the user to access the database. The user interacts with the database directly. The database is managed by a single program that provides an interface for the user to manipulate the data. Examples of single-layer DBMS include dBase, FileMaker, and FoxPro.

![SingleLayer](https://jorgesanchez.net/manuales/abd/bases-sgbd-web-resources/image/3.png)

- **Two Layer DBMS**: there are two layers between the user and the database. The first layer is the user interface layer, which provides an interface to the user to access the database. The second layer is the database management layer, which manages the database and provides functions to the user interface layer.  Examples of two-layer DBMS include MySQL, PostgreSQL, Oracle, and SQL Server.

![2layer](https://jorgesanchez.net/manuales/abd/bases-sgbd-web-resources/image/4.png)

- **Three Layer DBMS**: there are three layers between the user and the database. The first layer is the user interface layer, which provides an interface to the user to access the database. The second layer is the application layer, which manages the application and provides functions to the user interface layer. The third layer is the database management layer, which manages the database and provides functions to the application layer. Examples of three-layer DBMS include IBM DB2, SAP Sybase, and Informix.

![3layer](https://jorgesanchez.net/manuales/abd/bases-sgbd-web-resources/image/5.png)

## ANSI/SPARC architecture of a DBMS.

The **ANSI/SPARC architecture** of a DBMS stands for the *American National Standards Institute/Standards Planning And Requirements Committee* architecture of a Database Management System. It is a conceptual framework for designing and developing database management systems that was proposed by the ANSI in the 1970s.

The ANSI/SPARC architecture defines three levels of abstraction in a DBMS:

- **External level**: This is the level at which individual user views of the data are defined. Each user can have their own view of the data that is tailored to their specific needs. This level is concerned with the user interface and the way in which data is presented to users.

- **Conceptual level**: This is the level at which the overall logical structure of the database is defined. It defines the relationships between data elements and how they are organized into tables or other structures. This level is concerned with the overall design of the database and the relationships between data elements.

- **Internal level**: This is the level at which the physical implementation of the database is defined. It defines how the data is stored on disk or other storage media and how it is accessed and retrieved by the system. This level is concerned with the technical details of the database implementation.

![ANSI/SPARC architecture](https://upload.wikimedia.org/wikipedia/commons/d/df/4-2_ANSI-SPARC_three_level_architecture.jpg)

The ANSI/SPARC architecture also defines several components that make up a DBMS:

- **Data definition language (DDL)**: This is the language used to define the structure of the database and its relationships.

- **Data manipulation language (DML)**: This is the language used to insert, update, and delete data in the database.

- **Data control language (DCL)**: This is the language used to control access to the database, including the creation of user accounts and setting access privileges.

- **Query language**: This is the language used to retrieve data from the database.

The ANSI/SPARC architecture provides a clear separation between the different levels of abstraction in a DBMS, which allows for greater flexibility and scalability in database design and implementation.

## References

[Manual de Administración de Bases de Datos - Jorge Sanchez.net](https://jorgesanchez.net/manuales/abd/bases-sgbd.html){:target="_blank"}

[Database Architecture in DBMS: 1-Tier, 2-Tier and 3-Tier - Guru99](https://www.guru99.com/dbms-architecture.html){:target="_blank"}