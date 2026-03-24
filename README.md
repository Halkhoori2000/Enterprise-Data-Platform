The job description is that of a data engineer in a banking setting. As a data engineer in the data platform we are working with many other roles like analysts and architecture.
in this project you will describe the whole process of the data paltform i will share some content to help u get a better grasp of the architecture.
you need to cover highe level overview and some low level overview too.

here are some context and info you need to answer in ure process:
Confluent Kafka
- Can you explain what Apache Kafka is and what problem it solves?
- What are topics and partitions in Kafka?
- How would you ingest Kafka data into Databricks for real-time streaming?
- What’s the difference between at-least-once and exactly-once delivery in Kafka?
- What is the difference between Kafka and Confluent?
- You are getting duplicated records in your stream pipeline. How would you debug this?
- SQL Debezium inference
- Kafka API data

SQL
- What if the customer has no order?
- SQL query
- What would you change if you have to run this for 100M+ rows?
- What is the diff between UNION and UNION ALL?
- What is [window] function?
- What’s the diff between ROW_NUMBER() and RANK()?
- COALESCE
- Materialized View

Data Modelling
- How to handle many-to-many join?
- Data Mart vs Data Warehouse
- Factless fact
- Over-normalization in OLAP
- Logical vs Physical
- How to unify 2 independent systems with unique PK
- OLAP vs OLTP

Databricks
- DLT table
- Workflow
- Merge vs Upsert vs Insert
- Auto Loader
- Z-Order
- Vacuum [spelled “Vacum” in image]
- Delta Live Tables
- readStream
- Liquid Clustering

Spark
- What is Spark Tungsten engine?
- What is Catalyst optimizer?
- What is the difference between a logical and a physical plan?
- Spark optimization
- spark cache vs persist
- spark RDD and DataFrame
- Predicate pushdown

Database Ingestion
- Incremental load
- Full load
- Hashing for comparison
- Tools
- Migration
- CDC
- File-based ingestion

File System
- CSV
- JSON
- Parquet
- Avro
- ORC
- Are you aware of object store
- Flat address




- what’s the difference between append and complete output mode in structured streaming
- in autoloader how is schema evolution handled
- what’s the difference between checkpoint and write-ahead log
- how does watermarking prevent unbounded state growth
- stateful operation vs stateless
- in DLT what [is] the use of apply_changes
- what’s [RocksDB] in autoloader
- why can dropDuplicates in a streaming query still allow duplicates
- available [availableNow] in autoloader

- photon vs non-photon execution — what changes internally?
- how does Catalyst optimizer rewrite queries under the hood
- what is predicate pushdown?
- what is column pruning
- what’s the difference between narrow and wide transformation
- how does Databricks optimize joins with Delta + Photon
- explain [Z-Order] vs partitioning — when to use which
- your query is running 10 min instead of 2 — what steps will you take to optimize?
- you have to onboard 500 tables into a DLT pipeline — how do you make it metadata-driven
- what is salting?
- design question
- if AQE is enabled but query is still running slow

- what is Databricks Asset Bundle
- if Spark is not choosing a broadcast join when it should, how can you force it?
- which source is best for read-only jobs?
- what is columnar store?
- output file type if any application has to consume your output
- what is deletion vector used for?
- what is CDF in Delta tables?

- why [do] surrogate keys usually perform better than natural keys in joins
- in a lakehouse where would you apply normalization vs denormalization?
- how does partition pruning speed up joins?
- fact table (1B rows) + dimension (500K rows) — what join strategy?
- explain bucketing in Spark. what happens if bucket counts differ?
- you have two fact tables (2TB each); neither can broadcast. how to join efficiently?
- query = sales by region and month — how to optimize
- what are the issues if we over-normalize in OLAP systems
- AQE changes join strategies at runtime — pros/cons


Results-oriented Big Data Engineer with strong expertise in designing, optimizing, and managing large-scale data platforms. Proficient in programming languages and modern big data technologies, I deliver solutions that improve data processing performance and generate valuable business insights. I specialize in building and deploying scalable data architectures, leading end-to-end implementations, and integrating diverse data sources to ensure seamless accessibility and connectivity. Experienced in dashboard creation and data visualization, I support informed, data-driven decision-making. Driven by continuous improvement, I consistently solve complex challenges and deliver high-impact, reliable solutions tailored to modern data-intensive environments.
Partnering with Confluent to architect and implement a real-time streaming data warehouse solution.
- Designed and deployed fully reusable Confluent Kafka infrastructure using Terraform, enabling automated
provisioning, scalable deployment, and seamless teardown; integrated Oracle CDC and SQL Server
Debezium for robust data ingestion.
- Developing real-time data ingestion pipelines using Databricks Auto Loader and Delta Live Tables (DLT)
for scalable and resilient stream processing.
- Collaborating with the Data Modeling team to support the design and implementation of the Enterprise
Data Warehouse (EDW).
- Engineered a control framework on Databricks to integrate and ingest data from on-premise systems
securely and efficiently.
- Integrated Databricks with Informatica Data Quality to enhance data governance and ensure consistent
data standards.
- Connected Power BI to Databricks to enable real-time dashboard reporting and analytics for business
stakeholders.
