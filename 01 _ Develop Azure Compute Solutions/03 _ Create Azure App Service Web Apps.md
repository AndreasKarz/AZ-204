# Create Azure App Service Web Apps

## Preparations
- [Downwload Visual Studio Code](https://code.visualstudio.com/download)
- [Download Azure Storage Explorer](https://azure.microsoft.com/en-us/features/storage-explorer/)



## Technical Terms

| Term     | Description                           | Info                                                         |
| -------- | ------------------------------------- | ------------------------------------------------------------ |
| **RG**   | **R**esource **G**roup                | [Use Azure Resource Groups](https://www.otava.com/reference/how-to-use-azure-resource-groups-a-simple-explanation/) |
| **SNI**  | **S**ervice **N**ame **I**ndication   | [Enable SNI on a Windows Azure Cloud Service](https://raflrx.wordpress.com/2017/08/08/enable-sni-on-a-windows-azure-cloud-service/) |
| **ACR**  | **A**zure **C**ontainer **R**egistry  | [Azure   Container Registry documentation](https://docs.microsoft.com/en-us/azure/container-registry/) |
| **ACI**  | **A**zure **C**ontainer **I**nstances | [Azure   Container Instances documentation](https://docs.microsoft.com/en-us/azure/container-instances/) |
| **CRON** | A time-based job scheduler            | [Wikipedia](https://en.wikipedia.org/wiki/Cron)              |



## Pluralsight Modules

- [Creating Azure App Service Web Apps](https://app.pluralsight.com/course-player?clipId=2bad70bc-c13a-4978-9df7-76176464c252)
- [Configuring Azure App Service](https://app.pluralsight.com/course-player?clipId=609f6ffe-9c01-40fb-b522-df4aaec44985)
- [Scaling Azure App Service](https://app.pluralsight.com/course-player?clipId=da28941a-34bd-420a-bd0d-f8b35590bc79)



## Deep Dive

- [Secretless apps with .NET and Azure Key Vault](https://channel9.msdn.com/Shows/On-NET/Secretless-apps-with-NET-and-Azure-Key-Vault)
- [Building and deploying web apps with Static Web Apps](https://channel9.msdn.com/Shows/DevOps-Lab/Building-and-deploying-web-apps-with-Static-Web-Apps)



## Microsoft Learning modules

- [Deploy a website to Azure with Azure App Service](https://docs.microsoft.com/en-us/learn/paths/deploy-a-website-with-azure-app-service/)



## Questions

#### How to consume the WebApp connection string from the Azure App Service in DotNet Core?

Using Microsoft.Extensions.Configuration. Works with Environment Variables, appseetings.json and App Settings.

If you configure an app setting with the same name in App Service and in appsettings.json, for example, the App Service value takes precedence over the appsettings.json value. The local appsettings.json value lets you debug the app locally, but the App Service value lets your run the app in production with production settings. 

[Configure an ASP.NET Core app for Azure App Service](https://docs.microsoft.com/en-us/azure/app-service/configure-language-dotnetcore?pivots=platform-windows)



#### Where to find the logs of a WebApp with Cloud Shell?

[az webapp log tail --name appname --resource-group myResourceGroup](https://docs.microsoft.com/en-us/azure/app-service/troubleshoot-diagnostic-logs#stream-logs)



#### What is in the config.sh

The configuration for Linux based App Services.

[Configure a Node.js app for Azure App Service](https://docs.microsoft.com/en-us/azure/app-service/configure-language-nodejs?pivots=platform-windows)



