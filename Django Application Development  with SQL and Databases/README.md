## What is data?
- Data is a collection of facts (words, numbers) or pictures
- Data is one of the most critical assets of any business
- Data needs to be secure in a database

## What is database
- A database is a collection of data for input, storage, search, retrieval, and modification of data.
- A database management system (DBMS) is a set of programs for creating and maintaining the database, and storing, modifying and extracting information from the database using a function called querying.
- Two main types of databases:
  - Relational databases:
    - Data is organized into a tabular format with rows and columns.
    - Well-defined structure and schema.
    - Optimized for data operations and querying.
    - Involving many tables and much larger data volumes.
    - Use SQL as the stardard querying language.
  - Non-Relational databases:
    - Emerged in response to the volume, diversity, and speed at which data is being generated today
    - Built for speed, flexibility, and scale.
    - Data can be stored in a schema-less form
    - Widely used for processing big data

## Relational Database
- Rows are the records, Cols are the attributes
- Advantages:
  - Create meaningful information by joining tables
  - Flexibility to make changes while the database is in use
  - Minimize data redundancy by allowing relationships to be defined between tables
  - Are ACID compliant (atomicity, consistency, isolation, and durability) ensuring that data transactions are processed reliably.
    - Atomicity means either every operation succeeds or none of them do
    - Consistency is about ensuring that changes made as part of a transaction are consistent with any database constraints. If the data at any stage goes against these constraints, the whole transaction will fail.
    - Isolation is there to make sure that all transactions are run in an isolated environment without interfering (sự can thiệp) with each other.
    - Durability is another important element of ACID because it ensures that no matter what happens, once a transaction is complete, the changes in that transaction are written to the database.
  
- Limitations:
  - Does not work well with semi-structured and unstructured data
  - Entering a value greater than the defined length of a data field results in loss of information
  - May be expensive to maintain

## NoSQL
- There are four common types:
  - Key-value store
    - A key represents an attribute of the data and is an unique identifier
    - Don't use if you want to query data on specific data value, need relationships between data values and need multiple unique keys
  - Document Based
    - Store each record and its asscoiated data within a single document
    - Don't use if you want to run complex searh queries and perform multi-operation transactions
  - Column Based
  - Graph Based
- Advantages:
  - Simpler design, better control and improved scalability
  - Low-cost commodity hardware

## Relational Model
- RM is an abstract model used to organize data within a database.
- Key advantage of RM is data independence

## Entity-Relationship model
- Used as a tool to design relational databases
- Each entity is map into a table

## Primary key vs Foreign key
- Primary keys uniquely identify a specific row in a table
- Foreign keys which are primary keys defined in other tables, creating a link between the tables.

## SELECT Statement
- Used to retrieving rows from a table
- Using WHERE Clause to restrict the result set

## COUNT, DISTINCT, LIMIT
- Count: Retrieves the number of rows in a database
- Distinct: Removes duplicate values from a result set
- Limit: Restricts the number of rows retrieved from the database

## INSERT Statement
- Adding new record into the database
- Two methods: Single, Multiple

## UPDATE Statement
- Read and modify the data

## DELETE Statement
- Remove rows from the database 

## Django
- Follow MVC (model view controller) pattern which helps developers to build applications quickly and efficiently and efficiently Django was created to enable rapid development and code reuseability

## Opject-Relational mapping (ORM)
- Maps data stored in RDBMS into objects
- Allows developers to query and manipulate data using the OOP paradigm
- Performs CRUD on data using methods

## Django models
- Each Django model (class) is a database table
- Each class object represents a database table column
- Each field represents a database table column
- Schema and tables are automatically generated once model classes are defined

- Fields:
  - Each field in a model should be a Field class
  - Django maps each field to a column type, such as INT, ...

- Relationships:
  - One-to-one (inheritance):

<img width="637" alt="Screenshot 2024-02-17 at 5 42 58 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/2949216d-45e3-4d0a-a7b3-fbaae15b9b5a">

  - Many-to-one:

<img width="623" alt="Screenshot 2024-02-17 at 5 44 50 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/d59debc1-600f-428f-a059-42f8db1a2834">

  - Many-to-Many

<img width="624" alt="Screenshot 2024-02-17 at 5 48 28 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/bc5051aa-f9b3-4d3e-b7c0-56c89d1268b7">

<img width="636" alt="Screenshot 2024-02-17 at 5 45 19 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/48287203-81c7-428d-aed1-757fe8ef3448">

## Django Models CRUD

<img width="638" alt="Screenshot 2024-02-17 at 5 54 48 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/eb6ee284-bd92-4b3d-83c6-5ce4ba701a41">
