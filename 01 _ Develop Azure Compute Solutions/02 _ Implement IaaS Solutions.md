# Implement IaaS Solutions



## Preparations

- [Common Azure CLI commands for managing Azure resources](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/cli-manage)
- [Common PowerShell commands for creating and managing Azure Virtual Machines](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/ps-common-ref)
- [Azure CLI 2.0 Cheatsheet](https://github.com/ferhaty/azure-cli-cheatsheet)
- [Azure CLI - PowerShell Cheatsheet](http://thedevopspage.com/azurecli-powershell-cheatsheet)



## Technical Terms

| Term      | Description                       | Infos  |
|---|---|---|
| **TSV**	    | **T**ab **S**eparated **V**alue	| [Azure CLI Output Formats](https://docs.microsoft.com/en-us/cli/azure/format-output-azure-cli) |
| **CDN**	    | **C**ontent **D**elivery **N**etwork	| [Azure CDN Documentation](https://docs.microsoft.com/en-us/azure/cdn/) |
| **ASE**	    | **A**pp **S**ervice **E**nvironment	| [Introduction to the App Service Environments](https://docs.microsoft.com/en-us/azure/app-service/environment/intro) |
| **ILB**	    | **I**nternal **L**oad **B**alancer	| [Create and use an Internal Load Balancer](https://docs.microsoft.com/en-us/azure/app-service/environment/create-ilb-ase) |
| **SKU**	    | **S**tock **K**eeping **U**nit (Pricing Tier)	| [Choose a pricing tier](https://docs.microsoft.com/en-us/azure/search/search-sku-tier) |
| **RG**	    | **R**esource **G**roup	        | [Use Azure Resource Groups](https://www.otava.com/reference/how-to-use-azure-resource-groups-a-simple-explanation/) |
| **SNI**	    | **S**ervice **N**ame **I**ndication	| [Enable SNI on a Windows Azure Cloud Service](https://raflrx.wordpress.com/2017/08/08/enable-sni-on-a-windows-azure-cloud-service/) |
| **ACR**	    | **A**zure **C**ontainer **R**egistry	| [Azure Container Registry documentation](https://docs.microsoft.com/en-us/azure/container-registry/) |
| **ACI**	    | **A**zure **C**ontainer **I**nstances	| [Azure Container Instances documentation](https://docs.microsoft.com/en-us/azure/container-instances/) |
| **CRON**	    | A time-based job scheduler	    | [Wikipedia](https://en.wikipedia.org/wiki/Cron) |
| **IaaS**	    | **I**nfrastructure **a**s **a** **S**ervice	|  |
| **PaaS**	    | **P**latform **a**s **a** **S**ervice	|  |
| **SaaS**	    | **S**oftware **a**s **a** **S**ervice	|  |
| **F** (SKU)	| **F**ree plans (for dev)	|  |
| **D** (SKU)	| Shared plans (for **D**evelopment)	|  |
| **B** (SKU)	| **B**asic plans (for testing)	  |  |
| **S** (SKU)	| **S**tandard plans (production)	|  |
| **E** (SKU)	| **E**nterprise plans (production)	|  |
| **I** (SKU)	| **I**solated plans (production)	|  |



## Pluralsight Modules

- [Provisioning and Configuring Azure Virtual Machines](https://app.pluralsight.com/course-player?clipId=1b353c69-1c2b-412e-a803-43250cdcd74b)
- [Creating and Running Containers in Azure](https://app.pluralsight.com/course-player?clipId=6885ddd9-8161-4e85-9193-5ef8700926ea)



## Deep Dive

- [Infrastructure as a Service IaaS on Azure](https://www.youtube.com/watch?v=7PdJ6oT6cBk)
- [Azure IAAS Architecture](https://www.youtube.com/watch?v=GUpIakLNy_s)
- [Azure Interview Questions and Answers](https://www.youtube.com/watch?v=_Pyityj08vU)
- [Azure Container Instances Tutorial | Serverless containers in cloud](https://www.youtube.com/watch?v=jAWLQFi4USk)
- [What is a Container Registry and Azure Container Service](https://www.youtube.com/watch?v=kBw8ODZfCQ8)



## Microsoft Learning paths

- [Manage resources in Azure](https://docs.microsoft.com/en-us/learn/paths/manage-resources-in-azure/)
- [Deploy a website with Azure virtual machines](https://docs.microsoft.com/en-us/learn/paths/deploy-a-website-with-azure-virtual-machines/)



## Questions

#### What is the difference between horizontal and vertical scaling?
Autoscale only scales horizontally, which is an increase ("out") or decrease ("in") in the number of VM instances. **Horizontal** is more flexible in a cloud situation as it allows you to run potentially thousands of VMs to handle load.

In contrast, **vertical scaling** is different. It keeps the same number of VMs, but makes the VMs more ("up") or less ("down") powerful. Power is measured in memory, CPU speed, disk space, etc. Vertical scaling has more limitations. It's dependent on the availability of larger hardware, which quickly hits an upper limit and can vary by region. Vertical scaling also usually requires a VM to stop and restart.

[Overview of autoscale in Microsoft Azure](https://docs.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-overview#horizontal-vs-vertical-scaling)



#### What is the difference between ACR and ACI?
Azure Container Registry is a managed, private Docker registry service.
[Azure Container Registry](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-intro)

Azure Container Instances is a solution for any scenario that can operate in isolated containers, without orchestration. Run event-driven applications, quickly deploy from your container development pipelines, and run data processing and build jobs.
[Azure Container Instances](https://docs.microsoft.com/en-us/azure/container-instances/)

