# Develop Solutions with Cosmos DB Storage



## Preparations
- [What Is Azure Cosmos DB](https://www.youtube.com/watch?v=FkekFVRTASM)
- [Azure Cosmos DB resource model](https://docs.microsoft.com/en-us/azure/cosmos-db/account-databases-containers-items)
- [Common Azure Cosmos DB use cases](https://docs.microsoft.com/en-us/azure/cosmos-db/use-cases)
- [Azure Cosmos DB: Use Cases and Trade-Offs](https://towardsdatascience.com/azure-cosmos-db-use-cases-and-trade-offs-5a65727daaa9)
- [A Complete Walkthrough of Azure Cosmos DB and Why Should You Use It](https://www.netwoven.com/2018/12/04/a-complete-walkthrough-of-azure-cosmos-db-and-why-should-you-use-it/)
- [Azure Cosmos DB Introduction](https://www.youtube.com/watch?v=R_Fi59j6BMo) 



## Technical Terms
| Term      | Description                                                  | Info                                                         |
| --------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **ACID**  | **A**tomicity, **C**onsistency, **I**solation, **D**urability | [Transactions and optimistic concurrency control](https://docs.microsoft.com/en-us/azure/cosmos-db/database-transactions-optimistic-concurrency) |
| **RUs**   | **R**equest **U**nit**s**                                    | [Request Units in Azure Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/request-units) |
| **SPARK** | Apache Spark is a parallel processing framework that supports in-memory processing | [What is Apache Spark?](https://docs.microsoft.com/en-us/azure/hdinsight/spark/apache-spark-overview) |
| **IOPS**  | **I**nput/**O**utput operations **P**er **S**econd           | [Virtual machine and disk performance](https://docs.microsoft.com/en-us/azure/virtual-machines/disks-performance) |
| **OData** | **O**pen **Data** Protocol                                   | [Introduction to Open Data Protocol](https://azure.microsoft.com/de-de/blog/introduction-to-open-data-protocol-odata-and-sql-azure/) |
| **LINQ**  | **L**anguage **IN**tegrated **Q**uery                        | [Introduction to LINQ Queries](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/introduction-to-linq-queries) |



## Pluralsight Modules
- [Creating Cosmos DB Containers](https://app.pluralsight.com/course-player?clipId=e0a00352-dc1f-4ee4-be7c-68b2c16835ea)
- [Cosmos DB Performance](https://app.pluralsight.com/course-player?clipId=d87f153e-af0c-421b-96ee-6fe5af903104)
- [What is Partitioning in Azure Cosmos DB?](https://www.youtube.com/watch?v=zY09mdcIz0E) 
- [Server-side Programming with Cosmos DB](https://app.pluralsight.com/course-player?clipId=b3d941c4-ca4f-44bb-a2ae-ad6ebb5d9de8) 



## Deep Dive
- [Data Modeling and Partitioning Best Practice in Partitioned Repository Pattern with Cosmos DB](https://medium.com/swlh/partition-key-design-best-practice-in-partitioned-repository-pattern-with-cosmos-db-ef9318007fc1) 
- [Best practices for Azure Cosmos DB: Data modeling Partitioning and RUs](https://www.youtube.com/watch?v=bQBeTeYUrR8) 
- [Modeling data and best practices for the Azure Cosmos DB SQL API](https://azure.microsoft.com/en-gb/resources/videos/ignite-2018-modeling-data-and-best-practices-for-the-azure-cosmos-db-sql-api/)
- [Azure Cosmos DB documentation](https://docs.microsoft.com/en-us/azure/cosmos-db/) 
- [Frequently asked questions about different APIs in Azure Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/faq)



## Microsoft Learning modules
- [Choose the appropriate API for Azure Cosmos DB](https://docs.microsoft.com/en-us/learn/modules/choose-api-for-cosmos-db/) 
- [Build and run a web application with the MEAN stack on an Azure Linux virtual machine](https://docs.microsoft.com/en-us/learn/modules/build-a-web-app-with-mean-on-a-linux-vm/)



## Questions
#### Which API for what? 

- Use Core (SQL) to store a product catalog
- Use the Gremlin (graph) API as a recommendation engine
- Use MongoDB to import historical order data
- Use Cassandra for web analytics
- Use the Azure Table API to store IoT data

Read & learn [Choose the appropriate API for Azure Cosmos DB](https://docs.microsoft.com/en-us/learn/modules/choose-api-for-cosmos-db/)



#### Why CosmoDB instead of MongoDB or SQL directly?

Global distribution, scalable performance and higher availability.



#### What is the minimum RUs per gigabyte of data?

10 RU/s per GB of storage. 



#### What is the minimum throughput for autoscaling? 

10% of the maximum.



#### What has to be considered for the Consistency Level "Strong" and "Bounded Staleness"? 

Two times more RUs . The strong and bounded staleness consistency levels consume approximately two times more RUs while performing read operations when compared to that of other relaxed consistency levels.



#### What is the default consistency level?

Session consistency. One of the consistency levels in Azure Cosmos DB is Session consistency. This is the default level applied to Cosmos accounts by default. When working with Session consistency, the client will use a session token internally with each read/query request to ensure that the set consistency level is maintained.

[Manage consistency levels in Azure Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/how-to-manage-consistency?tabs=portal%2Cdotnetv2%2Capi-async)

