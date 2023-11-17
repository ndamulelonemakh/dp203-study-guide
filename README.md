# DP 203 Data Engineering on Microsoft Azure - Study Guide
> A curated list of topics to prepare for [Azure DP-203](https://learn.microsoft.com/en-us/certifications/exams/dp-203/) certification exam - Made with :heart: by [Peclyr.ai](). This guide assumes that you have a good conceptual understanding of basic data concepts in Azure Cloud e.g. Structured vs Unstructured data, Azure data platforms etc. We recommend using this guide in conjuction with the [learning path](https://learn.microsoft.com/en-us/certifications/azure-data-engineer/) provided for Free by Microsoft. You can also refer to the [data fundamentals learning path](https://learn.microsoft.com/en-us/credentials/certifications/azure-data-fundamentals/) to get an overview of the data services before diving deep into the details.


# Data Engineering concepts

- [ ] File formats e.g. Parquet, Avro, Binary etc.
- [ ] Surrogate Keys (Alternate keys)
- [ ] Slowly changing dimension Type 0, 1 and 2
- [ ] Big data [reference architectures](https://learn.microsoft.com/en-us/azure/architecture/data-guide/big-data/)


<br/>
<br/>


# Azure Data Lake Storage

- [ ] Posix controls
- [ ] SAS vs Managed Identity Access
- [ ] URL Schems e.g. abfss vs wasbs


<br/>
<br/>

# Azure Synpase Analytics

## 1. Data Injestion

- [ ] Load from SQL database
- [ ] Load with Polybase
- [ ] Load with Lake Database
- [ ] Load from Azure storage
- [ ] CTAS vs CETAS
- [ ] Other sources: Cosmos DB, SAP, S3 etc.

## 2. Pipelines

- [ ]  Copy Activity
- [ ]  Mapping Dataflow functions e.g. Pivot, Select, Filter etc.
- [ ]  Data flow script e.g. Split
- [ ]  Self-hosted vs Azure IR
- [ ]  CI/CD deployment across multiple environments

## 3. Monitoring

- [ ] Execution times
- [ ] Azure Monitor Alerts
- [ ] Sensitivity query results audit
- [ ] System/Metadata tables
- [ ] Common errors e.g. CSV schema mismatch


## 4. Security

- [ ] Admin Accounts
- [ ]  Access control
- [ ] Storage keys
- [ ] Encryption - HTTPS, TDE etc.
- [ ] Row level vs Column level security
- [ ] Masking Functions
- [ ] VNet Intergration
- [ ] Firewall rules

## 5. Perfomance

- [ ] Materialised Views
- [ ] Partitioning vs Distribution
- [ ] Partition switching
- [ ] Clustered columnstore index vs clustered index
- [ ] Capacity planning e.g. Expected rows per distribution/partition

### Labs

i. Create a data warehouse schema from the Contoso sample database

ii. Create a data warehouse schema from database dumps


<br/>
<br/>


# Azure Streaming Analytics

## 1. Window functions

- [ ] Tumbling windows
- [ ] Hopping windows
- [ ] Snapshot windows
- [ ] Session windows

## 2. Perfomance

- [ ] Streaming units
- [ ] Partitioning
- [ ] Embarassingly parallel jobs
- [ ] Late arrival policy
- [ ] Event time vs Arrival time
- [ ] Error policy
- [ ] Cloud vs Edge config

## 3. Development

- [ ] Azure portal vs Vscode vs Visual studio vs Command line development
- [ ] Javascript User-defined functions
- [ ] C# User-defined functions
- [ ] Machine learning scoring functions
- [ ] GeoSpatial functions, for example: ST_DISTANCE, ST_WITHIN etc.
- [ ] Aggregate functions e.g. TopOne()

## 4. Security

- [ ] VNet intergration

### Labs

i. Create a realtime dashboard to track user activity of a website
ii. Build a streaming Power Dashboard using Azure Stream Analytics as a data source

<br/>
<br/>

# Azure Databricks

## 1. Development

- [ ] Databricks utilities - dbutils
- [ ] Spark/Pyspark/Spark SQL - basic tranformations e.g. dropDuplicates(), mode(), partitionBy(), REPLACE()
- [ ] Mount data lake storage
- [ ] Structured streaming output modes
- [ ] Viewing cluster logs

## 2. Perfomance

- [ ] High concurrency cluster vs Standard
- [ ] Standard autoscaling vs Optimised autoscaling
- [ ] Incremental loads with Autoloader

<br/>
<br/>

# Azure SQL Database

## 1. Sharding

- [ ] Vertical Partions
- [ ] Horizontal Partitions
- [ ] Horizonal vs Vertical scaling
- [ ] Single tenacy vs Multi tenacy

## 2. Security

- [ ] Sensitivity Classification & Audit
- [ ] Azure AD Authentication
- [ ] Vnet intergration


<hr/>


# Closing remarks

This guide does not cover the full scope of the [DP 203](https://learn.microsoft.com/en-us/credentials/certifications/exams/dp-203/) exam, but the concepts which I found to be non-obvious when going through the learning material. I passed the exam in my first attempt with a score of over 800, and I would say going through the fundamentals learning path helped a lot when I was faced with tricky questions. Thinking from first principles is key to clearning these exams. If you can, do as many practical examples on Synapse analytics and have a good undestandng of common streaming concepts like windows and partitioning. Having a good grasp of security fundamentals like RBAC, Managed identities and Azure AD will also come in handy. The exam is not that bad if you give yourself time to practice, good luck!
