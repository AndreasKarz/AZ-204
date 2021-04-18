# Exam Alert: Implement Azure Security



## Pluralsight Modules
- [Preparing for the Exam](https://app.pluralsight.com/course-player?clipId=7e23c185-f6a6-4d61-a324-ec1a3e4446f8)



## Deep Dive
- [Azure AD App Manifest Overview](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-app-manifest), especially oauth2 properties, 
  - [oauth2AllowImplicitFlow](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-app-manifest#oauth2allowimplicitflow-attribute)
  - [oauth2Permissions](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-app-manifest#oauth2permissions-attribute)
  - [signInAudience](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-app-manifest#signinaudience-attribute)
- Azure Key Vault create commands in [PS](https://docs.microsoft.com/en-us/azure/key-vault/general/quick-create-powershell) and [CLI](https://docs.microsoft.com/en-us/azure/key-vault/general/quick-create-cli)
- [Top 10 Best Practices for Azure Security](https://www.youtube.com/watch?v=g0hgtxBDZVE)
- [How attackers exploit containerized Azure workloads](https://www.youtube.com/watch?v=-mmilNn9pak)
- [IT-Exams](https://www.itexams.com/exam/AZ-204?)



## Questions
- SAS with User Delegation works only with Blob Storage?
  **true**



- Use SAS User Delegation when ever possible. Why?
  **Good question**



- Are the Azure App Service available on free or shared tiers?
  **No**



- With TLS-Auth, hiw validate the certificate?
  **The app code is required to validate certificate**



- What happens with a system-assigned Managed Identity when the attached resource will be deleted? 
  **Identity is also deleted**



- If you delete a App Service app, the user-assigned identity will also be deleted? 
  **False**



- When using a user-assigned identity, the app will also have access to the permissions granted by the system-assigned identity? 
  **False. user-assigned turning of system-assigned**



- What is more secure, account SAS or SAS user-delegation? 
  **User-delegation use the Azure AD credentials and not a storage key an it's more secure. Only supports blob storage.**



