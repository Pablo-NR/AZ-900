# SC-900

**Zero Trust**: assumes everything is on an open and untrusted network, even resources behind the firewalls of the corporate network “**trust no one, verify everything.**”

- **Verify explicitly**: Always authenticate and authorize users based on multiple factors such as identity, location, and device.
- **Least privileged access**: Limit user access by applying just-in-time and just-enough access, and enforcing adaptive policies to balance security and productivity.
- **Assume breach**: Treat all resources as compromised, using segmentation, encryption, and analytics to detect and respond to threats efficiently.

**Six foundational pillars**: Identities, Devices, Applications, Data, Infrastructure, Networks. All elements work together to provide end-to-end security

**Governance:** is the system of rules, practices, and processes an organization uses to direct and control its activities. Many governance activities arise from external standards, obligations, and expectations.

**Risk management:** process of identifying, assessing, and responding to threats or events that can impact company or customer objectives. **External risks** stem from outside forces like political, economic, or environmental events, while **internal risks** arise from within the organization, such as data leaks or fraud.

**Compliance**: refers to the country, state, or multi-national regulations that an organization must follow. These regulations define what types of data must be protected, what processes are required under the legislation, and what penalties are issued to organizations that fail to comply.

- **Data residency**: Governs where data can be stored, transferred, or accessed based.
- **Data sovereignty**: Ensures data is subject to the laws of the country where it's physically held, even if processed or collected elsewhere.
- **Data privacy**: Focuses on transparency and protection regarding the collection, processing, and sharing of personal data, complying with privacy laws and standards.

**Identity**: It is the unique representation of a user, entity or device that allows its identification, authentication and authorization to access certain resources.

- **Administration**: Involves creating, managing, and governing user, device, and service identities, including their lifecycle (creation, updates, deletions).
- **Authentication**: Verifies an identity by requiring valid credentials to prove the person or entity is who they claim to be.
- **Authorization**: Determines the level of access an authenticated identity has within an application or service.
- **Auditing**: Tracks actions related to identities, including detailed reporting and alerts on who performed what actions, when, and how.

**Identity Provider (IdP):** It is the entity responsible for managing identities and storing them securely while providing authentication, authorization and auditing services.

**Federation**: allows users to access services across different organizations or domains by establishing trust relationships between identity providers, eliminating the need for separate credentials in each domain. 

## MFA and SSPR

![image.png](image.png)

## Infrastructure

![image.png](8adf7804-ae59-4dfd-b8ce-962b1abec14c.png)

## Defense in depth

![image.png](3c404b94-746f-47e2-b2ed-03c19d13bf3e.png)

**Azure DDoS Protection:** protect applications and servers by analyzing network traffic and discarding anything that looks like a DDoS attack. Protects at layer 3 (network layer) and layer 4 (transport layer).

- **DDoS Network Protection**: Provides advanced DDoS mitigation for Azure resources in a virtual network, including extra services like rapid response support and cost protection. It’s easy to enable without changing applications or resources.
- **DDoS IP Protection**: without the additional value-added services included in Network Protection, such as Web Application Firewall or rapid response.

**Network Security Groups (NSGs):** filter network traffic to and from Azure resources within a virtual network using rules based on source, destination, protocol, and ports. Consists of inbound and outbound security rules that allow or deny traffic

- **NSG** provide distributed traffic filtering for access control within a single virtual network, while **Azure Firewall** serves as a centralized, fully stateful firewall-as-a-service.

**Azure Firewall:** provides threat protection for your cloud workloads and resources running in Azure. Deploying on a centralized virtual network allows you to control traffic centrally for all connected VNets, simplifying network security management across subscriptions. (is offered in Basic, Standard and Premium

- Is a Stateful Firewall**,** tracks active connections and makes decisions based on traffic context.
- It ensures uptime by distributing resources across multiple availability zones.
- Filters both network and application-layer traffic based on rules like IPs, ports, and domains.
- Translates private IPs to public ones (SNAT) or public IPs to private ones (DNAT) for traffic management.
- Integrates with Microsoft's feed to block traffic from known malicious IPs and domains.
- Logs can be sent to Azure Monitor and others for tracking and analysis.
- Can integrate with other Azure services like Azure Virtual Networks, Policy, and Security Center for unified security management.

**Web Application Firewall (WAF):** provides centralized protection of your web applications from common exploits and vulnerabilities. A centralized WAF helps make security management simpler, improves the response time to a security threat, and allows patching a known vulnerability in one place, instead of securing each individual web application.

- WAF can protect against DDOS attacks on layer 7

**Azure Virtual Network (VNet):** private network in Azure, enabling segmentation and containment of resources through multiple networks and subnets, with controlled communication that enhances security by preventing unauthorized traffic by default.

**Azure Bastion:** is a PaaS that provides secure RDP and SSH connectivity to virtual machines through the Azure portal, without requiring public IP addresses or client software. It enhances security by preventing exposure of RDP/SSH ports to the internet while allowing seamless access to VMs within the same and peered virtual networks. Is deployed per virtual network

**Azure Key Vault:** securely stores and manages secrets, encryption keys, and certificates, providing centralized access control with strict authentication and authorization measures. It offers Standard and Premium tiers, the latter utilizing hardware security modules (HSMs) for enhanced key protection, automated certificate management, and activity monitoring.

## Compliance

**Microsoft Service Trust Portal (STP):** is a public platform that provides audit reports, compliance information, and resources to help organizations understand how Microsoft cloud services protect data and manage security and compliance.

- **Access Requirements**: Users must log in with a Microsoft cloud services account and accept a non-disclosure agreement to access certain resources.
- **Content Categories**: STP organizes information into categories including Certifications, Regulations, and Standards; Reports, Whitepapers, and Artifacts; Industry and Regional Resources; and Resources for your Organization.
- **My Library Feature**: Allows users to save relevant documents for easy access and set up notifications for updates on saved resources.

**Microsoft Privacy Principals:**

- **Control**: Users can access, modify, or delete their data anytime.
- **Transparency**: Clear about data collection and usage, with user consent required.
- **Security**: Strong security measures and encryption protect data.
- **Legal Protections**: No data disclosure to governments without user consent, unless legally required.
- **No Content Targeting**: Personal content isn't used for advertising.
- **User Benefits**: Data collection enhances user experience and service quality.

**Microsoft Priva** is a comprehensive suite of privacy solutions designed to enhance privacy operations across an organization's digital landscape. It enables organizations to streamline compliance, mitigate privacy risks, and consolidate privacy protections across their data.

- **Subject Rights Requests**: Automates handling of data subject requests (DSRs) within Microsoft 365, facilitating efficient fulfillment of privacy inquiries.
- **Privacy Risk Management**: Establishes policies to identify and remediate privacy risks, including:
    - **Data Overexposure**: Detects and manages insufficiently secure data.
    - **Data Transfers**: Monitors and alerts for data transfers across regions or departments.
    - **Data Minimization**: Identifies and manages stored data based on retention policies.
- **Consent Management (Preview)**: Helps businesses manage how they ask for and record users' permission to collect and use their data. You can create custom consent forms that work in different languages and can be used in various regions.
- **Privacy Assessments (Preview)**: Automatically keeps track of how personal data is used within the organization, ensuring compliance with privacy rules without needing manual updates.
- **Tracker Scanning (Preview)**: Automatically finds and manages tools (like cookies) that track user activities on websites, helping organizations comply with privacy laws easily.

**Microsoft Purview** is a comprehensive set of integrated data security, data governance, and data compliance solutions that can help organizations secure and govern their entire data estate, while helping them meet their compliance requirements.

- **Sensitive Information Types**: built-in types of sensitive information that can be identified using specific patterns. It also allows organizations to create custom types for their unique needs, including exact matches from a database.
- **Trainable Classifiers**: AI to help classify unique data for organizations. It offers ready-to-use classifiers and allows users to train their own for specific content types, improving accuracy through practice before going live.
- **Understanding and Exploring Data**: Microsoft Purview has tools that give insights into classified data and how users interact with it. Content Explorer shows detailed information about sensitive items, while Activity Explorer tracks actions taken on labeled content, helping admins manage compliance effectively.

## Purview Security

**Sensitivity labels:** allow organizations to classify and protect content like emails and documents by applying customizable labels that travel with the content, ensuring appropriate protection settings are enforced.

**Label policies:** publish sensitivity labels to specific users and groups, allowing them to apply labels to their content while enabling settings like default labeling and justification for label changes.

**Data Loss Prevention (DLP):** helps organizations protect sensitive information from being shared inappropriately by defining and applying policies that monitor and manage data across various platforms and applications.

- **DLP policies**: take **protective** actions when risky behavior is detected, such as warning users with pop-up tips, blocking sharing actions, or moving sensitive items to a secure location for data at rest. DLP policies can be created from **predefined templates**, or you can create a **custom policy**
- **Endpoint DLP:** monitors user actions on sensitive items on Windows and macOS devices, tracking activities like creating, renaming, and copying documents.
- **DLP policies in Teams:** protect sensitive information by displaying alerts to users when they attempt to share restricted content, helping them understand and correct the action.
- **DLP integrates with Copilot:** for summarizing alerts and accessing prompts, requiring onboarding and user permissions for effective use.

**Microsoft Purview Insider Risk Management:** helps organizations detect and manage internal risks by identifying and investigating risky behaviors, such as data leaks and compliance violations.

- **Policies**: Define insider risk management policies using templates that specify risk indicators, user inclusion, prioritized services, and monitoring periods.
- **Alerts**: Automatically generated alerts from matching risk indicators that provide a summary view for quick review and investigation.
- **Triage**: Reviewers assess alerts marked as needing attention, evaluating details, severity, and user activity to resolve or dismiss alerts.
- **Investigate**: Cases are created for alerts requiring deeper analysis, using tools like user activity charts, content explorer for related files, and case notes for documentation.
- **Action**: Reviewers take steps to resolve cases, which may include notifications for minor violations or escalating serious cases to eDiscovery for further investigation.
- **Insider Risk Management integrates with Microsoft Copilot for Security**, allowing users to summarize alerts and utilize built-in prompts, provided they have the necessary permissions and access to Microsoft 365 data.

**Adaptive Protection**: Utilizes ML to assess internal risk levels and dynamically apply adaptive protection controls, allowing high-risk users to face stricter measures while low-risk users maintain productivity.

**Adaptive Protection in Data Loss Prevention**: Automatically assigns DLP policies based on internal risk levels, adjusting to changes in user behavior to effectively protect the organization.

## Purview Compliance

**Audit (Standard)**: Automatically captures and stores user and admin activity logs for 180 days in Microsoft 365 services, providing basic search and export capabilities for security and compliance teams.

**Audit (Premium)**: Expands on the Standard version by offering longer retention (up to 10 years) and provides more bandwidth, customizable retention policies, intelligent insights for investigations, and greater API access for retrieving audit logs.

**Microsoft Purview** **eDiscovery:** helps organizations identify, manage, and deliver electronic information as evidence in legal cases. It allows users to search content across Microsoft 365 services, place content on hold, export results, and create review sets. 

- Place content locations on hold allows preservation of content relevant to an investigation by securing electronically stored information.
- **Copilot in eDiscovery** helps summarize evidence in review sets and convert natural language prompts into KQL queries for efficient investigation.

**Microsoft Purview Compliance Manager:** helps organizations manage and assess compliance by offering prebuilt and custom assessments, workflow tools, step-by-step improvement actions, and a compliance score to track progress and reduce risks across multicloud environments.

- **Controls**: Define the requirements for regulations or standards, with Microsoft-managed, customer-managed, and shared responsibilities.
- **Assessments**: Groupings of controls related to specific regulations, helping to ensure compliance with standards like ISO 27001.
- **Regulations**: Compliance Manager offers over 360 regulatory templates to quickly create compliance assessments.
- **Improvement actions**: Provide guidance for aligning with regulations, allowing admins to assign tasks and track progress.
- **Benefits**: Simplifies regulations, provides prebuilt and custom assessments, maps controls to actions, offers step-by-step guidance, and prioritizes high-impact compliance actions.

**Microsoft Purview Communication Compliance:** detects and manages inappropriate messages across platforms like Teams and Outlook, helping to prevent data security and compliance incidents by monitoring for policy violations and ensuring adherence to organizational standards, reducing risk and helping with regulatory compliance.

**Microsoft Purview Data Lifecycle Management:** enables organizations to efficiently retain necessary content and delete irrelevant data, ensuring compliance with regulations while minimizing security risks by reducing the amount of stored information.

- **Retention Policies**: These assign the same retention settings to content at the site or mailbox level, ensuring that items inherit the specified retention from their container.
- **Retention Labels**: These apply retention settings at the item level (e.g., folders, documents, emails) and travel with the content within the Microsoft 365 tenant, allowing for more granular control.
- **Key Concepts**: Retention settings can enforce "retain-only," "delete-only," or "retain and then delete" actions, helping organizations manage compliance, reduce risk, and ensure relevance of content.

**Microsoft Purview Records Management:** helps an organization look after their legal obligations, to demonstrate **compliance with regulations**, and increases efficiency with regular disposition of items that are no longer required to be kept

## Purview Governance

**Data Governance:** is the framework and processes that ensure data is managed, secure, and compliant while enhancing its visibility and accessibility for users, ultimately aligning data management with business objectives.

- **Federated Governance:** Centralizes data safety and quality standards while enabling self-service access and encouraging broad ownership across the organization.
- **Data Access:** Quickly provides appropriate access and enforces usage to balance safety and innovation.
- **Data Curation:** Organizes, annotates, and publishes data for safe accessibility, reusability, and protection.
- **Data Discovery:** Ensures users can easily find the data needed for daily operations and innovation.
- **Data Health:** Maintains data quality standards across the organization and keeps data fresh and secure through an active lifecycle.
- **Data Understanding:** Provides quality descriptors to help users comprehend the data's nature and appropriate usage.

**Data roles and responsibilities:**

- **Data consumers** quickly find and use relevant, trusted datasets through streamlined access request workflow.
- **Data owners** register data assets for use, manage classifications and access, and ensure high quality standards.
- **Data stewards** ensure data quality, seamless data discovery, glossary consistency, and lineage.
- **Central data office** establish and ensure governance policies, active metadata, compliance, and insights into overall governance health.

**Microsoft Purview Data Catalog:** A platform designed for data governance that enhances business value through features that streamline the organization, discovery, and management of data assets.

- **Governance Domains:** Organize data estate by business concepts, enabling common governance and discovery of data products.
- **Data Products:** Define business constructs that encapsulate data assets, providing context and use cases for data consumers.
- **Glossary Terms:** Provide critical business context and apply governance policies to data assets and products.
- **Critical Data Elements (CDEs):** Group important data pieces for easier management and standardization, with attached quality rules.
- **OKRs (Objectives and Key Results):** Trackable business objectives that link data products to governance domains to emphasize business value.
- **Data Access Policies:** Manage access to data products while promoting self-service opportunities within security standards.
- **Search and Browse:** Facilitate easy data discovery through search functionalities and an exploratory browsing experience.
- **Health Management:** Monitor and improve data governance through health controls and actions that enhance data quality and usability.

**Microsoft Purview Data Quality** enables businesses to assess and improve the quality of their data. It uses predefined and AI-generated rules to analyze data, assign a score, and provide visibility into data quality across the organization, helping to easily take corrective action.

## Copilot

**Microsoft Copilot for Security:** An AI-powered security tool that accelerates threat response by summarizing incidents, analyzing impact, reverse engineering malware scripts into clear explanations, and providing guided, actionable steps for efficient incident management.

- The **Standalone Experience:** is ****a dedicated site to interact with Copilot, using a prompt bar to request responses in text, images, or documents.
- The **Embedded Experience** integrates Copilot directly within Microsoft security products, like Microsoft Defender XDR, providing capabilities such as incident summarization and KQL query generation within the product’s interface.

**Session**: A specific conversation within Copilot where context is maintained across multiple prompts.

**Prompt**: A user-entered question or statement within a session, submitted through the prompt bar. 

**Capability**: A function or skill that Copilot uses to address part of a problem or task.

**Plugin**: A collection of capabilities provided by a particular resource, enabling specific functionalities. Microsoft Defender adds different plugins than Microsoft Intune.

**Orchestrator**: Copilot's system that combines and coordinates various capabilities to respond effectively to a user's prompt.

**Effective prompt**: involves being clear and specific about the goal, context, expectations, and sources, leading to more useful responses. Iterating prompts and providing detailed instructions help refine results tailored to your needs.

**Capacity** for Microsoft Copilot for Security should be provisioned within Copilot using a guided wizard, which is the recommended method for easier setup.

To **onboard** an organization to Microsoft Copilot for Security, the admin must **provision** and allocate security compute units (**SCUs**), set up the default environment, and assign role permissions to users.

## Microsoft Defender for Cloud

**Microsoft Defender for Cloud:** enables organizations to manage the security of their resources and workloads in the cloud and on-premises and improve their overall security posture. Integrates DevSecOps, CSPM, and CWPP:

**Cloud Security Posture Management** **(CSPM):** provides visibility into your security posture and offers guidance to improve it by identifying misconfigurations and weaknesses across cloud environments.

- **Secure Score**: Aggregates security findings into a single score, showing overall risk level.
- **Hardening Recommendations**: Groups related security recommendations to help fix vulnerabilities and improve posture.
- **Integration with Microsoft Copilot for Security**: Assists in understanding, remediating, and delegating security issues using AI support.
- **Defender CSPM Plan**: Offers foundational posture management for free, with an advanced plan providing deeper compliance and assessment features.

**Cloud Workload Protection:** secures resources, workloads, and services by detecting and resolving threats using integrated Microsoft Defender plans specific to the types of resources.

- **Microsoft Defender Plans**: Provides advanced protections for workloads like servers, App Service, Storage, SQL, Kubernetes, Key Vault, DNS, and more.
- **Enhanced Security Features**: Includes endpoint detection and response (EDR), vulnerability scanning, multicloud and hybrid security, threat protection alerts, compliance tracking, and access controls.

**Defender for DevOps:** integrates security into the development process, allowing teams to manage code and pipeline security while monitoring the overall security posture across multi-pipeline environments using Defender for DevOps.

- **Unified visibility**: Centralized view of DevOps security posture, including code vulnerabilities, secrets, and open-source dependencies across environments.
- **Strengthen configurations**: Secures Infrastructure as Code (IaC) templates to prevent misconfigurations from reaching production.
- **Prioritize remediation**: Provides code-to-cloud insights, helping developers fix critical issues with annotated pull requests and custom workflows.

**Microsoft Defender XDR:** natively coordinates detection, prevention, investigation, and response across endpoints, identities, email, and applications to provide integrated protection against sophisticated attacks

**Azure Policy**: is a rule about specific security conditions that you want controlled, supports built-in definitions but you can also create your own custom policy definitions.

**Security initiative:** is a collection of Azure Policy definitions, or rules, grouped together as a single item, towards a specific goal or purpose, in order to simplify management.

**Microsoft Cloud Security Benchmark (MCSB):** is a set of security and compliance best practices that map to industry standards (CIS, NIST, PCI DSS) and provide Azure and AWS-specific guidance for securing workloads, data, and services in multicloud environments.

**Regulatory Compliance Dashboard:** shows your compliance status with the Microsoft Cloud Security Benchmark (MCSB) and any other standards applied to your subscriptions. It tracks controls like network security, identity and access management, data protection, data recovery, incident response, and more.

## Sentinel

**SIEM** **(Security Information and Event Management):** is a tool that collects, analyzes, and correlates data across an organization's digital estate, detecting anomalies and generating alerts for potential threats.

**SOAR (Security Orchestration Automated Response):** automates responses to security alerts, using workflows triggered by systems like SIEM to run predefined security tasks and mitigate issues.

**Microsoft Sentinel:** is a cloud-native SIEM/SOAR solution that provides intelligent security analytics, threat detection, and automated response across the enterprise, offering comprehensive end-to-end security management.

- **Data collection**: Gathers data at scale from users, devices, apps, and infrastructure across on-premises and multicloud environments using out-of-the-box and custom connectors.
- **Threat detection**: Detects previously unseen threats and reduces false positives using analytics, MITRE ATT&CK, and threat intelligence integrations.
- **Investigation**: Uses AI and hunting tools to investigate incidents, with Jupyter notebooks for advanced analytics and custom visualizations.
- **Incident response**: Automates response workflows with playbooks, centralizing incident management and enabling rapid reaction to threats.

**Azure Monitor Workbooks:** allows you to monitor data and provides versatility in creating custom workbooks.

**Microsoft Sentinel with Microsoft Copilot for Security:** enables seamless integration through plugins for incident management and threat hunting using natural language queries.

- **Sentinel Plugin**: Allows role-assigned users to manage and investigate incidents within Sentinel workspaces using pre-built or custom prompts.
- **Incident investigation promptbook**: Provides predefined prompts to explore specific incidents, related alerts, reputation scores, and devices for efficient analysis.
- **Natural language to KQL**: Converts natural-language queries into ready-to-run KQL for faster threat hunting and analysis within the Defender portal.

## Entra ID

**Workload identity:** is an identity you assign to a software workload (app). This enables the software workload to authenticate and access other services and resources. 

**Service principal:** is an identity for an application. Once an application is registered with Entra ID, a service principal is created in each tenant where the app is used. Enables authentication and authorization of the app to protected resources.

**Managed identities:** type of service principal that are automatically managed and provide an identity for applications to use when connecting to Azure resources that support Entra ID authentication. Eliminate the need for developers to manage credentials

**Microsoft Entra Registered Devices:** Personal devices registered to Entra ID for BYOD scenarios, allowing access to organizational resources without needing an organizational account.

**Microsoft Entra Joined Devices:** Devices owned by the organization, joined to Entra ID and requiring an organizational account to sign in.

**Microsoft Entra Hybrid Joined Devices:** Devices joined to both on-premises Active Directory and Entra ID, needing an organizational account for sign-in

**Microsoft Entra External ID:** manages scenarios for working with external users. 

- **Workforce B2B collaboration:** allows your workforce tenant to collaborate with external business partners. Share your company's applications and services with guests, while maintaining control over your corporate data
- **External-facing apps**: manage secure sign-in for costumers and business costumers

**Security defaults:** pre-configured, basic security measures from Microsoft designed to enforce identity protection features like multifactor authentication (MFA) for all users and administrators, improving security at no extra cost.

**Password protection:** reduces the risk of users setting weak passwords. Detects and blocks known weak passwords and their variants, and can also block other weak terms that are specific to your organization. Can integrate with On-premises.

**Microsoft Entra ID Governance:** allows you to balance your organization's need for security and employee productivity with the right processes and visibility

- **Microsoft Entra access reviews:** enable organizations to efficiently manage group memberships, access to enterprise applications, and role assignment. Regular access reviews ensure that only the right people have access to resources
- **Entitlement management:** enables organizations to manage the identity and access lifecycle at scale. Automates access request workflows, access assignments, reviews, and expiration.
    - **Access packages**: contain resources that users can request access to. Policies can be defined to establish which users can request access, who must approve their access, and when access expires.

**Microsoft Entra Terms of Use:** allow organizations to present disclaimers or compliance information that users must accept before accessing data or applications, with conditions based on user roles or schedules to ensure legal adherence. With Conditional Access you can require terms of use

**Privileged Identity Management (PIM):** allows organizations to control and monitor access to critical resources by providing time-limited, just-in-time access, requiring approval, and enforcing multifactor authentication for role activation, helping reduce security risks by limiting who has privileged access and for how long.

**Microsoft Entra ID Protection** helps organizations detect, investigate, and respond to identity-based risks, covering both user and workload identities.

- **Sign-in risk** evaluates the likelihood that an authentication attempt is unauthorized, detecting issues like sign-ins from anonymous IPs, unusual travel patterns, or unfamiliar device behavior.
- **User risk** assesses the possibility that an account is compromised, identifying concerns such as leaked credentials, suspicious user behavior, or unusual sending patterns.

**Microsoft Entra Permissions Management:** is a central piece of the Zero Trust Security strategy that provides visibility and control over permissions across multicloud environments. It detects, automatically right-sizes (remediates), and continuously monitors unused and excessive permissions.

**Microsoft Entra Verified ID:** simplifies secure interactions between users and organizations, ensuring control over digital identities without compromising privacy. It allows people to store credentials in a **digital wallet** and share them with organizations that can verify the information using cryptographic signatures.

### Global Secure Access

**Microsoft Entra Private Access**: Provides secure, remote access to corporate resources without a VPN, using enterprise applications to manage access and block lateral attacks.

- **Quick Access**: Simplifies access by grouping private resources into a single application with shared access policies based on FQDN, IP, and ports.
- **Global Secure Access App**: Allows for more granular control by creating multiple enterprise apps and for each of these apps, assign users and groups and assign specific conditional access policies.

**Microsoft Entra Internet Access**: protects users and data from web threats by enforcing identity-centric security policies, web content filtering, and continuous access evaluation for SaaS applications and internet traffic.

**Global Secure Access Dashboard:** provides you with visualizations of the network traffic acquired by the Microsoft Entra Private and Microsoft Entra Internet Access services, offering insights through widgets like Global Secure Access snapshots, alerts, usage profiling, and web filtering to help monitor and optimize network configurations.

**Microsoft Entra specific roles:** Manage resources exclusively within Entra ID, such as users, applications, and groups.

**Service-specific roles:** Grant permissions to manage features within specific Microsoft 365 services like Exchange, Intune, SharePoint, or Teams.

**Cross-service roles:** Provide permissions across multiple services, such as security or compliance settings, spanning various Microsoft 365 applications.
