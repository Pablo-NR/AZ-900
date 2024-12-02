# AZ-900

[Puntos ](Puntos%204b718dbb96ab468e98b39abd50aecb49.md)

**Azure Government:** is only for EE.UU and their partners

**Azure Hybrid Benefit**: License program for using existing licenses for Windows Server and SQL Server with discounts on Azure.

**Azure Marketplace**: Platform for discovering, trying, and acquiring third-party solutions and services for Azure.

**Azure Service Bus**: Managed messaging service for communication between applications and services.

**Azure Resource Manager (ARM)**: It is the Azure deployment and management service that allows you to create, update, and delete resources in your account, managing all interactions with those resources.

**Bicep**: It is similar to ARM but uses a simpler language.

**Azure Migrate**: Provides a portal with tools and services for migrating infrastructure to Azure from on-premises environments.

- **Azure Migrate: Discovery and assessment**. Discover and assess on-premises servers running on VMware, Hyper-V, and physical servers in preparation for migration to Azure.
- **Azure Migrate: Server Migration**. Migrate VMware VMs, Hyper-V VMs, physical servers, other virtualized servers, and public cloud VMs to Azure.

**Azure API Management Service**: is a way to create and manage customer APIs for existing backend services

**Azure Batch**: Runs applications and jobs at scale in the cloud efficiently.

**Azure Policy**: A service for creating, assigning, and managing policies that control or audit resources.

**Initiative Definition**: Groups related policies to achieve a common goal.

**Azure Blueprints**: Define and deploy sets of Azure resources that meet organizational standards.

**Azure Architectures**: Set of reference architectures and best practices in Azure.

**Azure Machine Learning Studio**: is a drag-and-drop tool you can use to build, test, and deploy predictive analytics solutions.

**Azure Cognitive Services**: is a simplified tool to build intelligent IA apps

**Azure Bot Services**: provides a digital online assistant that provides speech support

## Defensa

**Microsoft Defender**: Collects security data, assesses environments, and prevents attacks.

**Azure Arc**: Expands Microsoft Defender's capabilities to machines in other clouds and hybrid environments.

**Azure Security Benchmark**: Uses security data from Microsoft Defender to apply security best practices in Azure.

**Azure DDoS Protection**: is an example of protection implemented at the perimeter layer. Protects websites and generate reports.

**DDoS Infrastructure Protection**: Monitors traffic and mitigates DDoS attacks at the infrastructure level.

**DDoS Network Protection**: Most comprehensive plan for DDoS protection, with the fastest response.

**DDoS IP Protection**: Similar to Network Protection but with a slower response.

**Microsoft Purview**: Data governance, risk, and compliance solutions. It allows you to manage and monitor data services both in the cloud and on-premises, ensuring security, privacy, and regulatory compliance

**Service Trust Portal**: Web portal that provides details on security, privacy, and compliance standards. It contains Microsoft Purview

**Azure Dedicated Hosts**: Assigns a physical server exclusively to a single organization, providing enhanced security and control.

**Azure Information Protection (AIP)**: Enables organizations to discover, classify, and protect documents and emails by applying labels to content.

**Azure Sphere**: Highly secure IoT solution that includes a microcontroller unit and a customized Linux OS

**Azure IoT Hub**: Connects and manages IoT devices.

**Azure IoT Central**: Easy-to-use platform for monitoring IoT devices.

**Azure Advanced Threat Protection**: Monitor threats by using sensors

## Monitorización y análisis

**Pricing calculator**: Give you an estimated cost for provisioning resources in Azure

**Calculadora TCO**: compare the costs for running an on-premises infrastructure compared to an Azure Cloud infrastructure.

**Cost Management**: provides the ability to quickly check Azure resource costs, create alerts based on resource spend, and create budgets that can be used to automate management of resources.

**Azure Event Hubs**: collect **events** from multiple resources into a centralized repository, Azure Blob Storage as an example

**Azure Monitor**: is a platform for collecting data on your resources, analyzing that data, visualizing the information, and even acting on the results. Can monitor Azure resources, your on-premises resources, and even multi-cloud resources

**Azure Monitor Alerts:** automatically notify you when specified thresholds are crossed and can also take corrective actions. Alerts can be based on logs or metrics and use action groups to configure notifications and actions.

**Azure Application Insights**: Azure Monitor functionality, monitors web applications, tracking metrics such as response times, failures, and server usage. It is configured with an SDK or agent and supports multiple languages.

**Azure HDInsight**: Managed Apache Hadoop clusters in the cloud that enable you to process massive amounts of data.

**Azure Advisor**: Provides recommendations to optimize deployed resources in terms of cost, reliability, performance, security, and operational excellence.

**Azure Service Health**: helps monitor the status of both the global Azure infrastructure and your specific resources. It includes:

- **Azure Status**: A global overview of Azure service outages.
- **Service Health**: Focuses on the services and regions you use, with alerts for outages and maintenance.
- **Resource Health**: Provides the health status of your individual Azure resources.

**Azure Log Analytics**: is a tool for writing and running log queries to analyze data gathered by Azure Monitor, supporting both simple and complex data analysis.

**Azure Activity Logs**: History of actions such as creating or shutting down a VM.

**Azure Databricks**: Data analytics platform based on Apache Spark, capable of consuming data from Azure SQL Database, Event Hubs, and Cosmos DB.

## IaaS

**Azure Virtual Machines**: Service that allows you to create and manage virtual machines in Azure.

**Azure Reservations**: Helps minimize virtual machine costs without reducing functionality by reserving capacity for the long term.

**Azure Virtual Machine Scale Sets**: Manages and creates a set of identical virtual machines with integrated load balancing.

**Azure Virtual Desktop**: Provides access to a Windows operating system from any device.

**Spot VM's**: Allows you to run virtual machines at a lower cost by utilizing unused capacity.

**Azure DevTest Labs:** is a service for easily creating, using, and managing infrastructure-as-a-service (IaaS) virtual machines (VMs) and platform-as-a-service (PaaS) environments in labs

## PaaS

**Azure Functions**: Allows you to run code as a service without managing the infrastructure; it is a serverless PaaS. It scales automatically and only consumes CPU while executing the code, as it deallocates resources once execution is complete.

**Azure Logic Apps**: Similar to Functions, but for predefined workflows without the need to develop code; it runs only in the cloud and is stateful.

**Azure Container Instances (ACI)**: execute containers in Azure without managing VMs. Provide operating system virtualization and a portable environment for virtualized apps.

**Azure Container Apps (ACA)**: Similar to Azure Container Instances but more elastic, as it includes load balancing and scalability.

**Azure Service Fabric**: Platform for packaging, deploying, and managing scalable and reliable microservices and containers.

**Azure Kubernetes Service (AKS)**: Provides management and scalability for container groups, and controls the lifecycle.

**Azure App Service**: Service for hosting web applications, REST APIs, and mobile backends.

**Azure DevOps**: is an integrated solution for the deployment of code

## Redes y tráfico

**ExpressRoute**: Private connection between the organization's on-premises network and the Azure virtual network, faster and more reliable as it does not traverse the public internet.

**Azure Virtual Network**: Service for creating and managing networks in Azure.

**Azure VPN Gateway**: Secure and encrypted connection between the organization's on-premises network and the Azure virtual network. Only one VPN Gateway is allowed per Virtual Network, but it can connect to multiple sites.

**User Defined Routes**: Allows you to modify traffic routing by creating custom routes and adding subnets.

**Azure DNS**: Allows you to host and manage DNS domains (but not purchase them; once purchased, they can be stored), providing fast and secure resolutions along with simplified management and high availability.

**Azure Traffic Manager**: DNS-based traffic load balancer.

**Azure Load Balancer**: Distributes load across multiple servers or virtual machines.

**Azure Application Gateway**: Load balancer that helps manage traffic in web applications.

**Network Security Groups**: (firewall) Are resources that can contain multiple rules to allow or block traffic.

**Network Virtual Appliances**: are specialized VMs that run a specific network function such as running a firewall or performing a WAN optimization.

## Almacenamiento

**Azure CDN**: Content delivery network (CDN) for efficiently delivering content globally.

**Azure Storage**: Provides storage of up to 5 PiB with no limit on the number of files, globally accessible via HTTP and HTTPS, ideal for storing entire computer data.

**Azure Blobs**: A massively scalable object store for text and binary data. Also includes support for big data analytics through Data Lake Storage Gen2.

**Azure Disks**: Block-level storage volumes for Azure VMs.

**Azure Files**: Managed file shares for cloud or on-premises deployments that are accessible by using Server Message Block (SMB) protocol.

**Azure Queues**: A messaging store for reliable messaging between application components.

**Azure Tables:** NoSQL table option for structured, non-relational data.

**Azure Cosmos DB**: NoSQL, provides low-latency access to globally distributed data, works with JSON documents, and offers options to use table APIs.

**MongoDB**: NoSQL database that stores data in JSON format, compatible with Cosmos DB.

**Azure SQL Database**:Stores relational data in SQL tables, ideal for traditional databases.

**Azure Synapse Analytics**: Builds data warehouses (formerly known as Azure SQL Data Warehouse), combining storage and analysis of large volumes of data.

**Azure Locks**: Prevents accidental modifications or deletions of resources in Azure.

**Azure Data Lake Storage**: Stores large volumes of data, including rarely used data, with support for analysis and processing.

**AzCopy**: It is a command-line utility (uses KQL) for copying, uploading, downloading, and synchronizing files in Azure storage accounts, and even between different cloud providers.

**Azure Storage Explorer**: Provides a graphical interface for managing files and blobs similar to AzCopy, and works on Windows, macOS, and Linux.

**Azure File Sync**: Replicates frequently accessed files locally and keeps less used files in cloud, synchronizing data as needed. Changes made locally are replicated in Azure and vice versa.

**Backup and Site Recovery**: Services for backup and disaster recovery.

**Data Migration Assistant**. is a stand-alone tool to assess SQL Servers. It helps pinpoint potential problems blocking migration. It identifies unsupported features, new features that can benefit you after migration, and the right path for database migration.

**Azure Database Migration Service**: Facilitates the migration of SQL databases from on-premises environments to Azure SQL Database.

**Azure App Service migration assistant**. is a standalone tool to assess on-premises websites for migration to Azure App Service. Use Migration Assistant to migrate .NET and PHP web apps to Azure.

**Azure Data Box**: It is a physical migration service that quickly and securely transfers up to 80 TB of data using a robust storage device, which is sent to your data center and returned via a regional carrier.

## Entra ID

**Microsoft Entra Connect**: Synchronizes user identities from an on-premises Active Directory (AD DS) domain to Microsoft Entra.

**Microsoft Entra Domain Services:** Provides managed domain services in the cloud without the need to manage domain controllers. It facilitates moving legacy applications to the cloud using existing credentials and groups.

**Azure AD Password Protection**: Protects passwords against brute force attacks and banned password lists.

**Azure AD Identity Protection**: Protects identities by detecting risks and responding to threats.

**Conditional Access**: Controls, allows, or denies access to resources based on signals such as location, device, or session state.

**Azure RBAC (Role-Based Access Control)**: Assigns roles to users to manage access to resources in Azure, defining which resources can be accessed and how.

**Privileged Identity Management (PIM)**: Limits and monitors access to privileged roles in Azure, and is not used for Azure Storage.

**Azure Key Vault**: Manages and protects keys, certificates, and secrets for applications and services.

**Microsoft Entra Private Access**: Connects users securely to private applications from any location.

**Microsoft Entra Verified ID**: Verifies and authenticates the identity of internal users for secure access.

**Microsoft Entra External ID**: Authenticates external users, such as customers or vendors, for secure access.

**Identity Secure Score**: Provides a security score that assesses current measures and suggests improvements across multiple subscriptions.

**User Risk Policy**: Activates when a user's credentials are compromised, to mitigate associated risks.

**Sign In Risk Policy**: Detects and investigates suspicious sign-ins to protect user accounts.

**Azure Resource Graph**: Allows performing complex queries and exploring resources in Azure using a powerful query language.