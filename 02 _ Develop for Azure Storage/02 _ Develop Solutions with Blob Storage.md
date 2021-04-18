# Develop Solutions with Blob Storage



## Preparations

- [Azure Storage Types and Use Cases](https://www.dremio.com/data-lake/adls/)
- [Configuring and Using Microsoft Azure Blob Storage](https://app.pluralsight.com/library/courses/microsoft-azure-blob-storage-configuring-using/table-of-contents)
- [Authorizing access to data in Azure Storage](https://docs.microsoft.com/en-us/azure/storage/common/storage-auth)
- [Azure Storage redundancy](https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy)
- [Install AzCopy on Windows](https://www.thomasmaurer.ch/2019/05/how-to-install-azcopy-for-azure-storage/)
- [Introduction to the core Azure Storage services](https://docs.microsoft.com/en-us/azure/storage/common/storage-introduction)
- [Azure Storage client libraries for .NET](https://docs.microsoft.com/en-us/dotnet/api/overview/azure/storage)
- [az storage blob Commands](https://docs.microsoft.com/en-us/cli/azure/storage/blob?view=azure-cli-latest)
- [AZCopy Cheat Sheet](https://docs.microsoft.com/en-us/azure/storage/common/storage-ref-azcopy?toc=/azure/storage/blobs/toc.json#see-also)



## Technical Terms
| Term      | Description                                                  | Info                                                         |
| --------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CLI       | Command Line Interface                                       |                                                              |
| ETag      | **E**ntity **Tag**                                           | [Wikipedia](https://en.wikipedia.org/wiki/HTTP_ETag)         |
| RA        | **R**ead **A**ccess                                          |                                                              |
| Legacy    | Altsystem (englisch legacy system)                           | [Wikipedia](https://de.wikipedia.org/wiki/Altsystem#:~:text=Der%20Begriff%20Altsystem%20oder%20Legacy,gewachsene%20Anwendung%20im%20Bereich%20Unternehmenssoftware.) |
| LRS       | **L**ocally **R**edundant **S**torage                        | [Azure Storage redundancy](https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy) |
| ZRS       | **Z**one-**R**edundant **S**torage                           | dito                                                         |
| GRS       | **G**eo-**R**edundant **S**torage                            | dito                                                         |
| RA-GRS    | **R**ead-**A**ccess **G**eo-**R**edundant **S**torage        | dito                                                         |
| GZRS      | **G**eo-**Z**one-**R**edundant **S**torage                   | dito                                                         |
| RA-GZRS   | **R**ead-**A**ccess **G**eo-**Z**one-**R**edundant **S**torage | dito                                                         |
| Inferred  | Zugriffsstufe abgeleitet (englisch inferred)                 | [Account-level tiering](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-storage-tiers#account-level-tiering) |
| Lease     | The Lease Blob operation creates and manages a lock on a blob for write and delete operations. | [Lease Blob](https://docs.microsoft.com/en-us/rest/api/storageservices/lease-blob) |
| Immutable | Unveränderbar                                                |                                                              |
| HSM       | **H**ardware **S**ecurity **M**odule                         | [Azure Dedicated HSM documentation](https://docs.microsoft.com/en-us/azure/dedicated-hsm/) |
| SSE       | **S**torage **S**ervice **E**ncryption                       | [Azure Storage Service Encryption](https://azure.microsoft.com/en-us/updates/azure-storage-service-encryption-sse-support-for-managed-disks/) |
| AADDS     | **A**zure **A**ctive **D**irectory **D**omain **S**ervices   | [Oerview](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/overview) |
| MSI       | **M**anaged **S**ervice **I**dentity (new just 'Managed identities') | [What are managed identities for Azure resources?](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview) |
| SAS       | **S**hared **A**ccess **S**ignatures                         | [Grant limited access to Azure Storage](https://docs.microsoft.com/en-us/azure/storage/common/storage-sas-overview) |
| BCDR      | **B**usiness **C**ontinuity and **D**isaster **R**ecovery    | [Azure Paired Regions](https://docs.microsoft.com/en-us/azure/best-practices-availability-paired-regions) |
| IAM       | **I**dentity and **A**ccess **M**anagement                   | [IAM Overview](https://azure.microsoft.com/en-us/product-categories/identity/) |
| TCO       | **T**otal **C**ost of **O**wnership                          | [TCO Calculator](https://azure.microsoft.com/en-us/pricing/tco/calculator/) |
| SSIS      | **S**QL **S**erver **I**ntegration **S**ervices              | [Lift and shift SQL Server Integration](https://docs.microsoft.com/en-us/sql/integration-services/lift-shift/ssis-azure-lift-shift-ssis-packages-overview?view=sql-server-ver15) |
| RBAC      | **R**ole-**B**ased **A**ccess **C**ontrol                    | [What is Azure RBAC](https://docs.microsoft.com/en-us/azure/role-based-access-control/overview) |
| CIDR      | **C**lassless **I**nternet **D**omain **R**outing            | [Understanding CIDR Notation when designing Azure Virtual Networks](https://devblogs.microsoft.com/premier-developer/understanding-cidr-notation-when-designing-azure-virtual-networks-and-subnets/) |
| NSG       | **N**etwork **S**ecurity **G**roup                           | [Network security groups](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview) |
| UDR       | **U**ser **D**efined **R**outes                              | [Virtual network traffic routing](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-udr-overview) |
| SCOM      | **S**ystem **C**enter **O**perations **M**anager             | [Connect Operations Manager to Azure Monitor](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/om-agents) |



## Pluralsight Modules
- [Understanding Azure Blob Storage](https://app.pluralsight.com/course-player?clipId=42c85e65-9864-4699-96ef-5508c28e2c78)
- [Interacting with Data Using the Azure SDK for .NET](https://app.pluralsight.com/course-player?clipId=39cd8cfc-9a75-4816-b6c1-bb4f8d285665)
- [Setting and Retrieving Properties and Metadata](https://app.pluralsight.com/course-player?clipId=4848740f-7464-425c-b7d4-3fa545dd9726)
- [Implementing Data Archiving and Retention](https://app.pluralsight.com/course-player?clipId=fcf38dd6-562f-41c5-b40e-5037c1fbf1fe)
- [Moving Items between Storage Accounts and Containers](https://app.pluralsight.com/course-player?clipId=68937d6a-5f2e-4261-9514-aaf3794e5ab0)



## Deep Dive
- [Creating and Configuring Microsoft Azure Storage Accounts](https://app.pluralsight.com/library/courses/microsoft-azure-creating-configuring-storage-accounts/table-of-contents)
- [Configuring and Using Microsoft Azure Blob Storage](https://app.pluralsight.com/library/courses/microsoft-azure-blob-storage-configuring-using/table-of-contents)



## Microsoft Learning modules
- [Store data in Azure](https://docs.microsoft.com/en-us/learn/paths/store-data-in-azure/)



## Questions
...



