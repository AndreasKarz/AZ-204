# Implement Secure Cloud Solutions

## Preparations
- [Azure Key Vault](https://www.youtube.com/watch?v=AA3yYg9Zq9w)
- 



## Technical Terms
| Term | Description                                              | Info |
| ---- | -------------------------------------------------------- | ---- |
| AAD  | **A**zure **A**ctive **D**irectory                       |      |
| HSM  | **H**ardware **S**ecurity **M**odule                     |      |
| FIPS | **F**ederal **I**nformation **P**rocessing **S**tandards |      |
| SSE  | **S**torage **S**ervice **E**ncryption                   |      |
|      |                                                          |      |
|      |                                                          |      |
|      |                                                          |      |
|      |                                                          |      |
|      |                                                          |      |
|      |                                                          |      |



## Pluralsight Modules
- [Implement Managed Identities for Azure Resources](https://app.pluralsight.com/course-player?clipId=a194836d-f5bb-4009-a12b-36115418ce9f)

- [Manage Keys, Secrets, and Certificates by Using the KeyVault](https://app.pluralsight.com/course-player?clipId=27cab9a5-a7c3-4911-9090-c02c1a1612f3)



## Deep Dive
- [Microsoft Azure Security - Getting Started](https://app.pluralsight.com/library/courses/microsoft-azure-security-getting-started/table-of-contents)

- [Managing Microsoft Azure Security](https://app.pluralsight.com/library/courses/microsoft-azure-security-managing-update/table-of-contents)

- [Managed Identity Support Overview](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/services-support-managed-identities)

- https://docs.microsoft.com/en-us/azure/search/search-howto-managed-identities-data-sources
  https://docs.microsoft.com/en-us/azure/search/search-howto-managed-identities-sql
  https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview
  https://docs.microsoft.com/en-us/azure/storage/common/storage-auth-aad-msi#net-code-example-create-a-block-blob

  [TODO Split]

- [Configuring and Managing Microsoft Azure Key Vault](https://app.pluralsight.com/library/courses/microsoft-azure-key-vault-configuring-managing/table-of-contents)

- [Securing Application Secrets in ASP.NET Core](https://app.pluralsight.com/library/courses/securing-application-secrets-in-asp-net-core/table-of-contents)

- [Microsoft Azure Security Engineer: Configure and Manage Key Vault](https://app.pluralsight.com/library/courses/microsoft-azure-security-engineer-configure-manage-key-vault/table-of-contents)

- [Microsoft Azure Solutions Architect: Implement an Application Security Strategy](https://app.pluralsight.com/course-player?clipId=3496001b-700c-4ada-bd01-0134084997b6)

- PS und CLI commands for Azure Key Vault

- Grafik mit verschiedenen Apps/Functions die über die Config auf Azure key Vault zugreifen



## Microsoft Learning modules
- [Protect against security threats on Azure](https://docs.microsoft.com/en-us/learn/modules/protect-against-security-threats-azure/)

- [Top 5 security items to consider before pushing to production](https://docs.microsoft.com/en-us/learn/modules/top-5-security-items-to-consider/)

- [Configure and manage secrets in Azure Key Vault](https://docs.microsoft.com/en-us/learn/modules/configure-and-manage-azure-key-vault/)

- [Configure security policies to manage data](https://docs.microsoft.com/en-us/learn/modules/configure-security-policies-to-manage-data/)



## Questions
- Eine Konstellation zu Managed Services
- Two Types of Managed Identities ( system | user ) - assigned
- Managed Identity is not available for the free tier! What is the minimum tier? - - - -
- Reihenfolge Beispiel aus Kurs Demo als Frage
- Was ist der Vorteil (best practice) von User assigned Identity vs. System assigned Identity?
- Difference between Azure Key Vault Tiers Standard and Premium? Hardware encryption (HSM Protected)
- Die 3 Optionen, wie man Azure Key Vault konsumieren kann
  - Azure AD App Registration
  - Managed Identity
  - Key Vault Refereces
- Was kann man in Azure Key Vault hinterlegen?
  - Keys
  - Secrets
  - Certificates
- Welche (2) Nuget Packages werden in einem Dotnet MVC Projekt mindestens benötigt, um auf Azure Key Vault zuzugreifen?
  - Azure.Identity
  - Azure.Security.KeyVault.Secrets
- Was bringt die Versionierung bei Azure Key Vault?
- How long is the maximum retention time for Soft Delete in Azure Key Vault? 90 Days
- Can you disable the purge protection in Azure key vault? Nur, wenn noch nicht enabled.



## Comments
...

