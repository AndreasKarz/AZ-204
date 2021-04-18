# Implement User Authentication and Authorization

## Preparations
- [What are security principals?](https://docs.microsoft.com/en-us/windows/security/identity-protection/access-control/security-principals)
- [Specifying Account SAS Parameters](https://docs.microsoft.com/en-us/rest/api/storageservices/create-account-sas#constructing-the-account-sas-uri)
- [Microsoft Identity](https://docs.microsoft.com/en-us/azure/active-directory/develop/) 
- [OpenID Connect](https://auth0.com/docs/protocols/openid-connect-protocol)
- [Understanding Tenants, Subscriptions, Regions and Geographies in Azure](https://blog.siliconvalve.com/2018/08/27/understanding-tenants-subscriptions-regions-and-geographies-in-azure/)
- [Understanding Claims](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/technical-reference/the-role-of-claims)



## Technical Terms
| Term  | Description                                         | Info                                                         |
| ----- | --------------------------------------------------- | ------------------------------------------------------------ |
| RBAC  | **R**ole **B**ased **A**ccess **C**ontrol           |                                                              |
| SAS   | **S**hared **A**ccess **S**ignature                 | [Create an account SAS](https://docs.microsoft.com/en-us/rest/api/storageservices/create-account-sas) |
| AAD   | **A**zure **A**ctive **D**irectory                  |                                                              |
| SAAK  | **S**torage **A**ccount **A**ccess **K**eys         |                                                              |
| IAM   | **I**dentity and **a**ccess **m**anagement          |                                                              |
| SAP   | **S**tored **A**ccess **P**olicy                    |                                                              |
| ADFS  | **A**ctive **D**irectory **F**ederation **S**ervice |                                                              |
| MSAL  | **M**icro**s**oft **A**uthentication **L**ibrary    |                                                              |
| OAuth | **O**pen **Auth**orization                          | [Wikipedia](https://en.wikipedia.org/wiki/OAuth)             |
| PKCE  | **P**roof **K**ey for **C**ode **E**xchange         | [Authorization Code Flow](https://auth0.com/docs/flows/authorization-code-flow-with-proof-key-for-code-exchange-pkce) |
| OIDC  | **O**pen**ID** **C**onnect                          | [OpenID Connect](https://auth0.com/docs/protocols/openid-connect-protocol) |



## Pluralsight Modules
- [Secure Azure Storage](https://app.pluralsight.com/course-player?clipId=7e9f5691-8daf-4859-b5f6-1122b84e35d8)

- [Authenticate using Azure AD](https://app.pluralsight.com/course-player?clipId=3b07801d-72fb-454b-9262-6f12954cc221)



## Deep Dive
- [Getting Started with Azure Active Directory for Developers](https://app.pluralsight.com/library/courses/getting-started-azure-active-directory-developers/table-of-contents)
- [Managing Microsoft Azure Active Directory](https://app.pluralsight.com/library/courses/microsoft-azure-managing-active-directory/table-of-contents)
- [Managing Identities in Microsoft Azure Active Directory](https://app.pluralsight.com/library/courses/microsoft-azure-active-directory-managing-identities/table-of-contents)
- RBAC
- [Microsoft Azure Security Engineer: Configure Security for Storage](https://app.pluralsight.com/library/courses/microsoft-azure-security-engineer-configure-security-storage/table-of-contents)
- [Getting Started with Azure Active Directory for Developers](https://app.pluralsight.com/library/courses/getting-started-azure-active-directory-developers/table-of-contents)
- [Building Authorization in Azure Active Directory for Developers](https://app.pluralsight.com/library/courses/building-authorization-azure-active-directory-developers/table-of-contents)
- [Developing Web Applications and Web APIs Protected by Azure Active Directory](https://app.pluralsight.com/library/courses/developing-web-applications-apis-protected-azure-active-directory/table-of-contents)
- [Developing Daemons and Services Protected by Azure Active Directory](https://app.pluralsight.com/library/courses/developing-daemons-services-protected-azure-active-directory/table-of-contents)
- [Microsoft Azure Authentication Scenarios for Developers](https://app.pluralsight.com/library/courses/microsoft-azure-authentication-scenarios-developers/table-of-contents)



## Microsoft Learning modules
- [Secure your Azure Storage account](https://docs.microsoft.com/en-us/learn/modules/secure-azure-storage-account/)

- [Secure your Azure resources with Azure role-based access control (Azure RBAC)](https://docs.microsoft.com/en-us/learn/modules/secure-azure-resources-with-rbac/)

- [Secure your Azure SQL Database](https://docs.microsoft.com/en-us/learn/modules/secure-your-azure-sql-database/)



## Questions
- Deny assignments block access and overwrite Allow assignments?
  **true**



- What is the biggest difference between SAAKs and SAS?
  **SAAKs has root privileges to storage, SAS not**



- Wich are the planes to protect Storage? 
  **Keys, SAS, AAD**



- What you should do frequently with SAAKs and SASs? 
  **Rotate the Keys**



- Should you use SAAKs to access to resources directly? 
  **No for security reasons, they have root privileges.**



- What you should use to rotate SAAKs and SASs automatically? 
  **Azure Key Vault**



- What are the three SAS?
  - **User delegation SAS R**
  - **Service SAS R**
  - **Account SAS R**
  
  
  
- Which SAS Token you can use for Impersonation?
  
  **User delegation SAS**
  
  
  
- What do you need the keys for in practice?? 
  **To generate SAS Token**

- 

- Two Kinds of SAS? 
  - **Ad-Hoc (complete Link)**
  - **Service SAS with SAP (short Link with Policy)**
  
  
  
- Three Kindes of Token? 
  - **Access Token (Authentication)**
  - **ID Token ( (User) Authorization)**
  - **Refresh Token (for new Access Token)**



