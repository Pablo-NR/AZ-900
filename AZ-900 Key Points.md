# AZ-900 Key Points

- To sign in to an **Azure account**, a **Microsoft account** is **required**.
- **Azure China** is **not** operated by **Microsoft**, is operated by **21Vianet**
- If you are migrating to Azure, the **first** step is to have a **Microsoft account** to create a **subscription**.
- A **tenant** is created in the default domain `onmicrosoft.com`.
- Different **subscriptions** can be purchased for an organization using the same tenant that contains the organization's accounts.
- **Subscriptions** can be transferred under a single account to manage them centrally.
- You can only have **one** account **administrator** per **subscription**
- For a support request and to manage Azure Web Apps, visit [https://portal.azure.com](https://portal.azure.com/).
- Microsoft provides a separate portal for working with **preview** services.
- **Private preview** = **lower cost**, when services are released the price increase
- **Private preview** is early access to new concepts and tools for a select group of consumers.
- **Public preview** is similar but provides early access to everyone.
- To integrate an ITSM tool, you can use the ITSM connector.
- The Account Administrator, Service Administrator, and Co-Administrator can all make a support request.
- Changes in roles can take up to 30 minutes to take effect.
- **Microsoft Cloud Defender** is designed for Azure, on-premises, and hybrid environments.
- One of the alerts provided by **Azure Advisor** is a notification that Virtual Machines (VMs) do not have backup enabled.
- In **Microsoft Purview governance:**
    - Data Catalog –– This enables data discovery.
    - Data Sharing –– This shares data within and between organizations.
    - Data Estate Insights –– This accesses data estate health.
    - Data Policy –– This governs access to data.
- To access **Service Health**: Dashboard>Help+Support> Service Health
- **Azure Service Health** cannot prevent a service failure from affecting a specific VM.
- **Health advisories** are issues that require that you take proactive action to avoid service interruptions, such as service retirements and breaking changes
- **ARM templates** can be added to **Azure Blueprint**
- **Azure Blueprint** can’t be assigned to a Resource Group but **can** be used to **grant permissions** to a resource

- In a **JSON**, attributes are between quotes
- When you are implementing a Software as a Service (**SaaS**) solution, you are responsible for configuring the SaaS solution. Everything else is managed by the cloud provider.
- **Cloud Bursting** is a hybrid cloud configuration where, when the capacity of the private cloud reaches 100%, the traffic is automatically redirected to the public cloud.
- **Threat Intelligence** includes a Parent Policy, which is a set of default rules for protection. These can be overridden with stricter and therefore more secure rules.
- **Log Analytics** is a tool within **Azure Monitor** that can be used to collect and analyze logs.
- The only security model that adapts to the complexity of new environments is the **Zero Trust model**.
- The objective of **defense in depth** is to use several layers of protection to prevent information from being accessed or stolen by unauthorized users.
- You can access **Compliance Manager** from the Microsoft 365 **admin center**
- From **Azure Portal**, to **assign a role** to a resource group yo should enter to **Access control (IAM)**
- **Azure Sentinel** doesn’t store the logs in a storage account
- **Azure Sentinel** can remediate incidents automatically using playbooks
- **Azure Sentinel** can collect Windows Defender Firewall logs from Azure VMs
- **Azure Key Vault** can control and **manage disk encryption** keys and secrets.
- Microsoft Privacy Statement details the personal data collected by Microsoft and how uses the data
- Only the **billing administrator** of an account can **transfer** ownership of a **subscription**

## Payment

- **Pay-as-you-go** means you only pay for the Azure services you use.
- With a **pay-as-you-go subscription** you can use **Azure Cost Management**
- There are 2 types of **expenditure model**: Capital Expenditure (CAPEX) and Operational Expenditure (OPEX)
- A user can only have one free account.
- A free account has 5GB blob storage and a limit of 10 web apps
- During the **first 30 days** of the **free account**, you have access to everything with up to **$200**. After that, only free resources for everyone remain available, and any unused portion of the $200 will be forfeited.
- With the **Azure Free Account**, you have access to over **55 products** that are **always free**. You only pay if you use paid services, and **Azure Hybrid Benefit does not apply** since you are not paying for anything (there's no discount to use).
- **Azure Cost Manager** provides details on the costs of deployed resources. To calculate future costs, you use the **Pricing Calculator**.
- **Azure Cost Manager** can view costs associated to **management groups and resource groups**
- When planning to **migrate a public website to Azure**, you must plan to **pay monthly usage costs**. This is because Azure uses the pay-as-you-go model.
- **Creating** multiple **resource groups** does **not** incur **additional costs.**
- If you want to **raise** the **limit** or quota above the default limit, open an online **customer support** request at no charge.
- You can view your company’s regulatory compliance report from Microsoft Defender for Cloud
- The **only** Entra ID **tier** that limits the number of objects is the **FREE** tier, with a limit of **50,000 objects**. The other tiers have unlimited objects.
- **Azure web tier plan**:
    - **Free**: Does not support custom domains, has limited storage, does not provide dedicated compute instances, and lacks load balancing.
    - **Shared**: Supports custom domains but does not provide dedicated compute instances and lacks load balancing.
    - **Basic**: Supports custom domains and provides dedicated compute instances, but does not include load balancing.
    - **Standard**: Supports custom domains, provides dedicated compute instances, includes load balancing, includes SSL support and offers 50GB storage.
- **ISO**: organization that defines **international** standards across all industries
- **NIST**: organization that defines standards used by the **United States** government
- **GDPR**: **European** policy that regulates data privacy and data protection
- **Modern Lifecycle Policy:** Microsoft provides a minimum of 12 months' notice before ending support for a service.
- Azure **TCO calculator** can be used by **anyone**.
- **Purchasing** Azure **services** through an **Enterprise Agreement** requires you to spend a **predetermined amount**
- **Azure reservations** can be purchased for a max of **3 years**

## PowerShell, CLI

- You can **create a VM** using Azure Cloud Shell, Azure PowerShell, and Azure CLI.
- Yes, you can **deploy a Virtual Machine Scale Set** using the Azure **CLI**.
- To **create a policy** in Azure Policy, you can use Azure Portal, ARM Template, Azure CLI, Azure PowerShell, Python, and REST.
- Azure CLI, Azure PowerShell, and Azure Portal are **compatible** with virtually all OS.
- Con **Azure Cloud Shell** puedes ejecutar scripts tanto de Bash como de PowerShell
- Yes, you can **launch the Azure CLI** from both PowerShell and the Windows CMD.
- To run Azure **commands** on Powershell installed in a computer, is needed the **Azure Powershell module.**
- New-AzVm    —> Powershell
- az vm create —> CLI (siempre que empiecen por AZ)
- Los **comandos** de **CLI funcionan** para **Powershell** también
- Los **comandos** de **Powershell no** funcionan para **CLI**
- Desde la **CLI** se puede **acceder** a **Powershell y al revés**

## VM

- A VM **only** needs a **public IP** if it must be accessible from the **internet**, and it **only** needs a **data disk** if you want to **expand** its **storage**.
- A VM **requires** a **virtual network** to communicate with other resources and a **NIC** to connect to that network.
- **Just In Time VM Access** is a feature of Microsoft Defender for Cloud that **limits access** to a specific **VM** to a **time window.**
- The **user** of a **VM** is **responsible** for the **data** stored on it.
- A **VM** in the **Deallocated** state does not incur costs for compute resources. However, if it is in the **Stopped (Allocated)** state, it will generate compute costs. Regardless of the state, as long as the VM is not deleted, there will always be a cost for the OS disk, which occupies storage space in Azure until the VM is deleted.
- **Availability Sets,** (escalonan) VM updates based on their **update and fault domains.**
- **Azure Advisor** identifies underutilized or **unused** Azure **VMs**
- SLA guarantees an uptime for VMs

## Storage

- **Hot access tier**: For data that is accessed frequently, such as images for a website.
- **Cool access tier**: For data that is accessed infrequently and must be stored for at least 30 days, such as customer invoices.
- **Archive access tier**: For data that is rarely accessed and must be stored for at least 180 days, such as backups.
- An **access tier** is configured individually for each object, not for the entire storage account, so each object inherits its own tier.
- Before access data stored in the **Archive access tier**, data must be **rehydrated**
- Only the **hot and cool** access tiers can be **set at the account level**. The **archive access** tier can only be set at the **blob level**
- **Blob storage** can be reached from anywhere by using an internet connection
- To **store** the unmanaged data **disks** of an Azure **VM**, one should use Azure **Blob Storage** within the **Containers** service
- To store **several computer** data on Azure Storage you must use **File Service** in a storage account
- A **Storage Account limit** is **2PB** for US and Europe, and **500 TB** for all other regions.
- Data stored in Azure Storage has **at least 3 copies**
- **Azure File Sync** can be used in a variety of scenarios, such as:
    - Enabling users to access files from any location, using any device
    - Offloading storage from on-premises servers to the cloud
    - Replicating files between servers for disaster recovery
    - Centralizing file share management in the cloud
- **Uploading** data to Azure from anywhere, such as from on-premises, does **not** incur additional costs. However, **downloading** data **from Azure** or transferring data between regions does **incur costs**.
- You can use **Power BI** to analyze and visualize data stored in **Azure Data Lake** and **Azure Synapse Analytics**
- The **cost** of cloud **storage** depends on both the **amount of data** stored and the number of **read and write** operations.
- **Data transfers** within the **same** Azure **region** is always **free**
- Inbound is free.
Outbound is paid per GB.
Storage rent is paid per GB/month.
Storage read/write operations are paid.
- There are two storage services **IoT Hub** can route messages to -- **Azure Blob Storage and Azure Data Lake Storage**
- **Premium storage** accounts **can** be configured as Azure **File Shares**, Block **Blobs** Storage but **NO StorageV2**
- **Premium Block Blobs** only support **ZRS**

## Availability

- **Geo-redundant storage** replicates data to a secondary region for protection against regional outages, but it is only readable if a failover occurs. Enabling **read access** to the secondary region allows the data to be read at any time
- To achieve **higher availability:** replicate within different data centers in the same availability zone > replicate across different availability zones within the same region > replicate across different regions.
- You **cannot choose the region** where data is **replicated**, Microsoft determines this.
- Not all regions support **Availability Zones**
- An Azure **region** contains **one or more data centers** that are connected by using a **low-latencty** network
- In a **region pair**, a region is paired with another region in the same geography
- **Geo-distribution** enables Azure **resources** to be deployed **close** to **users**
- 2 or more VMs on **2** or more **Availability Zones** = **99.99%** 
2 or more VMs on **1 Availability Zone** = **99.95%                                 Min** offered by azure **= 99.9%**
- If uptime is below the SLA, you can claim a credit
- To calculate composite SLA, multiply all the SLA
- Each service in Public Preview defines its own SLA, algunos tienen y otros no

## Resources

- **10,000 management groups** can be supported in a single directory.
- A management group **tree** can support up to **six levels of depth**. This limit doesn't include the root level or the subscription level.
- Each management group and subscription can support only one parent.
- Yes, you can have **resources** in the same resource group but in different regions.
- **Tags** assigned to a resource group are not inherited by the resources within that group. Each resource must be tagged individually if you want it to have specific tags.
- **Tags** can be assigned by policy (example: non-compliant tag)
- **Permissions** assigned to a resource group are inherited by the resources within that group. If you have permission to manage a resource group, you can manage all the resources inside
- Azure **resources** can be **moved between** different **subscriptions**.
- A user can **access** to Azure cloud **resources without** an **Entra ID** account, if **granted** by an **administrator**.
- CPU time, disk size, and write operations, are used to calculate your **bill** for a resource.
- While a **policy cannot** be created for a **specific scope** (resource group, subscription, etc.), a **lock can** be.
- **Locks** are **inherited,** and a **resource** can have **multiple locks**
- To **remove** a **resource with** a **lock**, the **lock** must be **removed before**.
- **Azure Policies** can only control access for a **single solution**, while **Management Groups** can **manage access** across **multiple subscriptions at once**.
- If you create a **policy** in a resource group that **prohibits a** certain **existing resource** within that group, the resource will **continue to exist** after the policy is applied but will be marked as **non-compliant.**
- If you delete a resource group you delete all the resources inside

## Network

- You can modify the **Azure Firewal**l to allow access to a web application installed on a VM.
- To **enable communication** between a VM and other Azure resources outside of the virtual network, you can modify the **Network Security Groups (NSGs)**. NSGs function similarly to a firewall, controlling inbound and outbound traffic
- Service **endpoints** are used to expose Azure services to a virtual network, providing communication between the two.
- The **local network gateway** is a specific object that represents your on-premises location (the site) for routing purposes.
- **Virtual Network Gateway** is generally used to connect networks over the internet.
- **Azure DNS** does not support DNSSEC. It does not allow you to purchase domains directly. It uses Anycast to direct DNS queries to the nearest DNS server. It supports private DNS domains.
- **Express Route** works on OSI **layer 3**
- You can use cloud computing without internet using **ExpressRoute,** but you **can’t manage cloud resources without internet**
- **Azure Firewall** uses **NAT** which is applied before any rules
- **Azure Firewall and Network Security Groups** **can’t** be used to **encrypt traffic** from Azure to the internet, for that **VPNs are used.**
- The **difference** between **Azure Firewall and NSGs** is that Azure Firewall can filter traffic for **multiple subscriptions**, **NSGs** filter it for a **specific one.**
- **NSGs** can use resources such as I**P addresses, Service tags, Applications** **security groups, subnets and network interfaces** for a inbound security **rule**.
- NSGs block all inbound traffic by default.
- Azure **charges** for renting **public IP addresses.**
- **Creating virtual networks is free**, and **each subscription allows** for the creation of up to **50** virtual networks.
- **BGP** enables dynamic routing between **on-premises** and the **cloud**.
- To create a **route** in a virtual network, it is **not necessary** to create a **subnet** first. Routes can be defined independently of subnets, even though routes are applied to specific subnets or the entire virtual network.
- You can link virtual networks together by using virtual network **peering**. **Peering** enables resources in each virtual network to communicate with each other.
- **Route-based VPN gateway** are **more resilient** to **topology changes,** such as the creation of new subnets, than **Policy-based VPN gateway.**
- **Azure Advisor** does **not** provide **recommendations** on how to configure the network settings on Azure VM**.**

## Entra ID

- You need an **Entra ID account** to manage a **subscription**.
- You can create **group policies** in Entra ID
- **Entra ID** can be used to authenticate users for both Azure and Microsoft 365.
- It is **not necessary** to implement domain controllers to use Entra ID.
- **Azure Advisor** does **not** provide **recommendations** on how to **improve security** in **Entra** ID**.**
- To control which users can stop a VM, you do so from the **Conditional Access**.
- With **B2B in Entra ID**, you can manage external collaborators.
- To use **Entra ID** credentials to **sign in** to a **computer** that runs Windows 10, the computer must be **joined to Azure AD**
- **Alert messages** **cannot** be sent from **Azure Monitor** to **Entra ID security** groups, messages can **only** be sent to **specific users**

## PaaS

- A **PaaS** can automatically scale the number of instances and provides additional memory to apps by changing pricing tiers.
- **Azure Logic Apps** runs only in the **cloud** and is **stateful**
- **Microsoft SQL server database** and **Azure Backup** are **PaaS**

## IaaS

- If an **app** needs several **prerequisite** and services installed, that app can only be deployed as a **IaaS**
- If a **PaaS** is **installed** on a **VM**, then the entire setup **is** an example of **IaaS**.1
- Anything **legacy** is an **IaaS**

**What is SaaS, PaaS, IaaS**

![image.png](https://github.com/Pablo-NR/Microsoft-Certifications/blob/main/Images/image.png)

**Supports plans**

![image.png](https://github.com/Pablo-NR/Microsoft-Certifications/blob/main/Images/image%201.png)

![image.png](https://github.com/Pablo-NR/Microsoft-Certifications/blob/main/Images/image%202.png)

**Microsoft Cloud Adoption Framework**

![image.png](https://github.com/Pablo-NR/Microsoft-Certifications/blob/main/Images/image%203.png)

![image.png](https://github.com/Pablo-NR/Microsoft-Certifications/blob/main/Images/image%204.png)
