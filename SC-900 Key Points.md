# SC-900 Key Points

- **Microsoft Cloud Adoption Framework for Azure** provides best practices from Microsoft employees, partners and customers including tools and guidance to assist in an Azure deployment
- **Microsoft Cloud Adoption Framework for Azure**: strategy, plan, ready, adopt, govern, manage (SPRAGM)
- You can **assign** a **security principal** to an **Azure AD role**
- **eDiscovery** is used to identify, hold and export electronic information that might be used in an investigation
- Assigning **custodians** is only available in **Premium eDiscovery**
- Before start to search on **eDiscovery**, you must create a hold
- You can manage **Intune** from the **Microsoft Endpoint Manager Admin Center**
- **Intune** can manage Android devices and manage organization-owned devices and personal device
- **Intune** can’t be used to provision Azure subscriptions
- The **principles of zero trust**: Verify explicitly, Least privileged access, Assume breach
- The **Six privacy principles** are: Control, Transparency, Security, Strong legal protections, No content-based targeting, Benefits to you
- **CASB four pillars** are: Visibility, compliance, data security, and threat protection
- **Hybrid identity** don’t require more than 1 tenant
- **Security baselines for Azure** provides benchmark recommendations and guidance for protecting Azure services
- **Security benchmark** includes **CIS and NIST**
- **Windows Hello for Business** information is stored only in a local device
- You can use **Access Reviews** to evaluate a user membership and automatically remove users that no longer require membership in a group
- You can crate one **Azure Bastion** per **virtual network**
- **Azure Bastion** provides a secure connection to a **VM** using **RDP** for connections through **Azure portal**
- **Network protection** is used to reduce the attack surface
- **Workbooks** are for analysis and visualization of security data
- **Playbooks** are for automated incident response.
- **Azure firewall** can protect **VM** and **virtual networks** in a centralized way
- **Azure firewall** provides network-level filtering, application-level filtering, and outbound SNAT
- **Azure WAF** provides centralized protection of web app from common exploits and vulnerabilities
- **NSG** can be associated to **Subnet and a Network Interface**
- **NSG** have a unique name for identification and default rules can’t be deleted, only overwritten
- **Azure DDoS Protection Standard** can protect up to **100 resources** without additional costs and is **NOT enabled** by **default** in an Azure subscription
- Resource layer attacks, protocol attacks, and volumetric attacks are the most common **DDoS attacks**.
- **DDoS Protection Standard** protect **virtual networks**
- **Pre-trained classifiers** detects a resume document that a job applicant provides an employer
- **Azure Blueprints** can **deploy** Azure **resources** across multiple subscriptions in a consistent manner
- **Multiple sensitivity labels can’t** be applied to a file
- **Multiple Retention labels can’t** be applied to a file
- **Sensitivity labels** add headers and footers to documents
- **Sensitivity labels** can be used to encrypt documents and are **persistent**
- To provide real-time **integration** between Azure **Sentinel** and another security source you use a **connector**
- Microsoft **Sentinel** data **connectors** support **Microsoft and other parties services**
- **Azure Entra ID business-to-business (B2B)** collaboration is a feature within External Identities that lets you invite guest users to collaborate with your organization like suppliers, vendors, partners…
- Entra ID **External identities:**
    - are **not** managed in the same directory as users
    - can sign in by using **social or enterprise** **account** identities
    - **branding** can be applied to Entra ID B2C authentication
- **MFA** is required when **security defaults** are enabled in Entra ID
- **Entra ID Identity Protection** can’t assign users to groups based on risk
- **Conditional Access Session Control** enable limited experiences such as blocking download of sensitive information
- A **Conditional Access policy** can be applied to a **Microsoft 365 group**
- **SSPR** can use an external email address
- Microsoft Entra **Permissions Management** **can’t** be managed by using the Microsoft Purview **compliance portal**
- From Microsoft Entra **Permissions Management** you can manage permissions on **AWS**
- **Secure Score can’t** be reviewed from the **Permissions Management**
- **Managed identities** are used by a resource to access Azure services
- A **SYSTEM-assigned managed identity** can only be used by **one** Azure **resource**
- A **USER-assigned managed identity** **can** be used by **different** Azure Web Apps
- A **USER-assigned managed identity** can **exist** even after the **resource** has been **deleted**
- You should use a **USER-assigned managed identity** to associate the **same identity** to more than one **VM**
- In **Insider Risk Management**
    - Triage: review and filter alerts
    - Investigate: create cases in the case dashboard
    - Action: send a reminder of corporate policies to users
    - **Insider Risk Management** don’t protect against phishing because is a external threat
- **DLP** can display **policy tips** to users who are about to violate your organization’s policies and **protect documents** in OneDrive that contain sensitive information
- **DLP** can only be used with Windows 10 and newer and macOS
- **Microsoft Purview compliance portal** contains the **solution catalog**
- **Compliance Manager** tracks your controls, Microsoft managed controls and shared controls
- An **assessment** in **Compliance Manager** is a grouping of controls from a specific regulation, standard or policy
- **Compliance Manager** assesses compliance data continually for an organization
- **Compliance Manager** can be accessed directly from **Microsoft Purview**
- The **compliance score** in Compliance Manager measures an organization’s **progress** toward **implementing controls.**
- With **Information Protection** in Microsoft 365 compliance center you can protect sensitive data from being exposed to unauthorized users
- With a **Microsoft 365 E3** subscription, when using the unified **audit log and Basic Audit**, the audit records are retained for **180** days
- **Audit (Premium)** can be used to **investigate** possible security or compliance breaches and **identify** their **scope** based on records.
- **Information barriers** are used to **restrict communication** and the sharing of information between members of two departments at your organization, **DO NOT** detect **inappropriate language**
- **Information barriers** is supported by SharePoint, Teams, OneDrive
- **Microsoft Purview communication compliance** detect **inappropriate language**
- **Microsoft Purview communication compliance** works with Teams, Exchange, Copilot, Viva Engage and Third party sources

## Defender

- **Microsoft Secure Score** supports recommendations for Microsoft 365 (including Exchange Online), Microsoft Entra, Microsoft Defender for Endpoint, Defender for Identity, Defender Cloud Apps, and Teams.
- **Microsoft 365 Defender Portal** include alerts from:
    - Microsoft 365 Defender
    - Microsoft Defender for Office 365
    - Microsoft Defender for Endpoint
    - Microsoft Defender for Identity
    - Microsoft Defender for Cloud Apps
    - Azure Active Directory (AAD) Identity Protection
    - App Governance
    - Microsoft Data Loss Prevention
- From I**ncidents** in the **Microsoft 365 Defender portal** you can identify the devices affected by an alert, and aggregation of alerts that relate to the same attack
- From **Reports** in the **Microsoft 365 Defender portal** allow to view security trends and track the protection status of identities
- From **Hunting** in the **Microsoft 365 Defender portal** you can identify security threats before an alert is triggered
- **Cloud Security Posture Management (CSPM)** is available for all Azure subscriptions
- **Azure Defender** can detect vulnerabilities and threats for **Azure Storage**
- **Azure Security Center** can evaluate the security of **workloads** deployed to Azure on on-premises
- Microsoft Defender **XDR** integrates **Defender for cloud and Sentinel**
- You can see **Azure Secure Score** from Microsoft Defender for Cloud
- **Endpoint Detection and Response and vulnerability scanning for SQL** is part of Defender for Cloud enhanced security
- **Microsoft Defender for Identity** is a cloud-based solution that leverages **on-premises** AD signals to identify, detect and investigate advanced threats
- **Microsoft Defender for Cloud Apps:**
    - can use **conditional access** policies to control sessions in real time
    - can discover and control the use of **Shadow IT**
    - **connectors** retrieve data from apps and their activity logs
    - can prevent **data leaks** to nonclompliant apps and limit access to regulated data
    - can **protect sensitive information** hosted anywhere in the cloud
    - allows you to meet the compliance standards for **GDPR and PCI.**
- **Microsoft Defender for Office 365**
    - includes the **Attack simulation training** feature
    - **Threat Explorer** provides real time reports to identify and analyze recent threats
    - **Threat Trackers** provides intelligence on prevailing cybersecurity issues
    - **Anti-phishing protection** detects impersonation attempts
- **Microsoft Defender for Endpoint** can reduce attack surface and automate investigation and remediation.
- **Microsoft Defender for Endpoint** works with **android**

- **Entra ID P1, P2** don’t charge for the first **50000 MAU** per month
- **Entra Free and External ID** include additional costs from the **first user**
- **Entra ID P2** is the minimum edition that allows you to create **access packages** for users

![image.png](image%201.png)

| **FALLOS** | **1-100** | **101-200** | **Learn** |
| --- | --- | --- | --- |
| **1-10** | 1-0 | 5-1 | 1-1 |
| **11-20** | 3-0 | 1-0 | 0-2 |
| **21-30** | 1-0 | 1-0 | 1-1 |
| **31-40** | 2-0 | 2-0 | 1 |
| **41-50** | 1-0 | 0-0 | 4 |
| **51-60** | 3-0 | 3-0 |  |
| **61-70** | 4-2 | 5-0 |  |
| **71-80** | 3-2 | 2-0 |  |
| **81-90** | 3-0 | 2-0 |  |
| **91-100** | 3-0 | 2-0 |  |
| **Total** | 24-4 | 23-1 | 7 |