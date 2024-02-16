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
  - Are ACID compliant (atomicity, consistency, isolation, and durability)
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
