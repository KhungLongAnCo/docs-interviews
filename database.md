# Database

1. **NoSQL vs SQL**
    SQL and NoSQL are two different types of database management systems used to store and manage data. Here are some of the key differences between SQL and NoSQL:
    - **Data Model**: SQL databases use a relational data model, where data is organized into tables with predefined relationships between them. NoSQL databases, on the other hand, use a non-relational data model, where data is stored in a variety of ways, such as key-value pairs, document-oriented, or graph-based.
    - **Scalability**: SQL databases are vertically scalable, meaning that they can handle increased traffic by adding more resources to a single server. NoSQL databases are horizontally scalable, meaning that they can handle increased traffic by adding more servers to a distributed system.
    - **Query Language**: SQL databases use SQL (Structured Query Language) as their primary query language, which is a standardized language used to manage and manipulate data in a relational database. NoSQL databases do not use SQL as their primary query language, and instead use a variety of query languages specific to the type of database.
    - **Data Structure**: SQL databases require a predefined schema, which defines the structure of the data in the database. NoSQL databases do not require a predefined schema, and can handle unstructured or semi-structured data.
    - **ACID Compliance**: SQL databases are typically ACID (Atomicity, Consistency, Isolation, and Durability) compliant, meaning that they ensure that database transactions are processed reliably. NoSQL databases may or may not be ACID compliant, depending on the specific database.
    - **Use Cases**: SQL databases are typically used for applications that require complex queries and transactions, such as financial systems or e-commerce platforms. NoSQL databases are typically used for applications that require high scalability and performance, such as social media platforms or real-time analytics.

    In summary, SQL databases are relational, vertically scalable, use SQL as their primary query language, require a predefined schema, and are typically used for complex queries and transactions. NoSQL databases are non-relational, horizontally scalable, use a variety of query languages, do not require a predefined schema, and are typically used for high scalability and performance.

2. **What is indexing?**
    **Answer:** Indexing is the process of creating an index on a database table to improve the speed of data retrieval.

3. **What is a transaction?**
    **Answer:** A transaction is a sequence of database operations that are treated as a single unit of work. Transactions ensure that all operations are completed successfully or none of them are completed.