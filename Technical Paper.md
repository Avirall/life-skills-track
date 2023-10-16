# Technical Paper
### Situation: You joined a new project. The project is going through some performance and scaling issues. After some analysis, the team lead asks you to investigate possibly using a NoSQL database will improve performance.

## Abstract
NoSQL databases are a type of database that does not use the traditional relational database model. NoSQL databases are often used for applications that require high performance, scalability, and flexibility.
This paper discusses the different types of NoSQL databases and why they are used. It also provides an overview of the benefits and challenges of using NoSQL databases.

## Introduction
When people use the term “NoSQL database”, they typically use it to refer to any non-relational database. Some say the term “NoSQL” stands for “non-SQL” while others say it stands for “not only SQL”. Either way, most agree that NoSQL databases are databases that store data in a format other than relational tables.

## Benefits of NoSQL databases
1. Flexible Data Models:
Unlike SQL tables, these do not mandate a predefined schema. This means that documents within a single collection can possess varying sets of fields, and the data type for a specific field can vary from one document to another within the same collection.
2. Horizontal Scaling:
Unlike many SQL databases that necessitate vertical scaling when resource capacity is exceeded, NoSQL databases are designed for horizontal scaling. This approach permits the seamless addition of economical commodity servers to meet growing demands.
3. Expedited Queries:
In contrast to SQL databases, where data is often normalized, necessitating complex joins for retrieving a single entity's information, NoSQL databases optimize data storage for efficient querying. This optimization eliminates the need for complex joins, resulting in exceptionally fast query execution.
4. Developer-Friendly:
Certain NoSQL databases, such as MongoDB, align their data structures with popular programming languages. This alignment simplifies data storage, mirroring the way developers handle data in their application code. This harmonious mapping reduces the need for extensive coding, expediting development and reducing the likelihood of bugs.

### Types of NoSQL databases
1. Document Databases:
Document databases organize data into documents resembling JSON (JavaScript Object Notation) objects. Each document comprises key-value pairs, where values can assume various types, including strings, numbers, booleans, arrays, and objects.
2. Key-Value Databases:
Key-value databases offer a straightforward data model where each entry consists of keys and associated values.
3. Wide-Column Stores:
Wide-column stores organize data in tables, rows, and dynamic columns. This structure is well-suited for applications that demand the storage and retrieval of vast datasets, particularly when the data's schema evolves or when handling time-series data. Wide-column stores, such as Apache Cassandra, are designed for scalability and distributed data management.
4. Graph Databases:
Graph databases are designed for data organized in nodes and edges. Graph databases are ideal for applications where understanding and traversing complex relationships and dependencies are paramount, such as social networks, recommendation systems, and network analysis.

### Popular NoSQL databases:
#### MongoDB
MongoDB is favoured by developers for its scalability, versatility, and ease of use. Its document data model simplifies data storage in a JSON-like format that aligns with modern programming languages, eliminating the need for complex data normalization. MongoDB's scalability accommodates high data volumes and traffic, offering horizontal and vertical scaling options. The platform provides various deployment choices, from cloud solutions like MongoDB Atlas to on-premises options. With a supportive developer community and enterprise-grade support, MongoDB accelerates software development, facilitates collaboration across teams, and efficiently manages evolving data needs, making it an ideal choice for diverse applications and use cases.
#### Apache Cassandra
Apache Cassandra is an open-source NoSQL distributed database known for its scalability and high availability while maintaining exceptional performance. Its masterless architecture and low latency ensure data durability even during data center outages, making it suitable for hybrid and cloud environments. Cassandra excels in fault tolerance, with robust support for replicating across multiple data centers, minimizing latency and ensuring resilience against regional outages. Its performance is noteworthy, consistently outperforming other NoSQL databases due to its architectural choices. Operators have control over replication methods, offering both synchronous and asynchronous options. Cassandra is well-suited for distributed, data-critical applications, with a decentralized, scalable, and elastic design that ensures continuous operation and growth. Its audit logging and observability features enhance security and monitoring, making it a robust choice for mission-critical data management.
#### Redis
Redis and SQL databases are compared in terms of data modelling, querying, and scalability. SQL databases employ structured, table-based schemas with fixed data models, while Redis uses a flexible model supporting a variety of data structures like strings, hashes, and lists. Redis's data modelling offers agility and more efficient querying due to its complex data structure support, and it enables horizontal scalability by adding nodes. SQL databases, on the other hand, excel in complex queries and data analysis, ensuring data consistency and providing robust transaction support. The choice between Redis and SQL depends on the specific needs of an application, with Redis favoured for its data modelling and scalability, and SQL databases suitable for data consistency and complex queries.
#### Couchbase
Couchbase is a modern and versatile database designed for enterprise applications, catering to a wide range of computing scenarios, from cloud-based microservices to edge computing for Mobile/IoT devices. It efficiently manages JSON documents, eliminating the need for fixed schemas, and provides developers with control over the schema within JSON objects. Couchbase excels in performance, offering various data processing capabilities such as caching, key-value storage, full-text search, analytics, and event-driven programming, all while interleaving transactions. This unique design minimizes data sprawl, enhances security, simplifies administration, and reduces costs. It enables developers to write applications once and deploy them at any scale, all within a distributed and fault-tolerant architecture.
#### Apache HBase
HBase is a column-oriented, non-relational database system that operates on the Hadoop Distributed File System (HDFS). It is optimized for storing sparse data sets, making it ideal for handling large volumes of data with random read/write access. Unlike traditional relational databases, HBase uses Java for application development, and it also supports Apache Avro, REST, and Thrift for application writing. HBase is designed to scale linearly, employing standard tables with rows and columns, and it requires a primary key for table access. It leverages ZooKeeper for high-performance coordination and seamlessly integrates with Hive for robust big-data applications.

### References
https://www.mongodb.com/why-use-mongodb
https://cassandra.apache.org/_/index.html
https://levelup.gitconnected.com/redis-vs-other-databases-an-in-depth-comparison-of-sql-and-nosql-solutions-7c4a9ca9183
https://docs.couchbase.com/server/current/introduction/why-couchbase.html#:~:text=Couchbase%20manages%20JSON%20documents%2C%20eliminating,data%20processing%20capabilities%20on%20it.

