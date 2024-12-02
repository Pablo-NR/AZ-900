# MS-900

[MS-900 Key Points](MS-900%20Key%20Points%201054bd42f51480599ae2f09bd8375827.md)

**Microsoft 365**: is a cloud-based subscription service that consists of apps and services such as Office apps, Teams, Windows, world-class security and more

**Microsoft Copilot for Microsoft 365:** an AI-powered productivity tool. It uses large language models (LLMs) and integrates your data with the Microsoft Graph and Microsoft 365 apps and services.

**Windows-as-a-Service** is a new model for Windows. Instead of a major release every three or four years, features are released more frequently, such as semi-annually.

**Azure Virtual Desktop (AVD)** is a cloud-based desktop and app virtualization solution that supports multi-session Windows, allowing users to access desktops and apps from anywhere. The customer manages the infrastructure.

**Windows 365** is a cloud-based service that provides personalized, single-user Cloud PCs, streamed from the Microsoft cloud, with simplified deployment and management handled by Microsoft.

**SharePoint team sites:** provide secure shared file storage, facilitate collaboration on content authoring among all team members, as well as support integration with Microsoft Teams and Power Automate

- **SharePoint communication sites:** provide means for communicating information across teams, with a small number of content authors

**Microsoft Yammer**: private social network designed for employees to connect, collaborate, and share ideas within an organization. It is useful for resolving support issues, gathering feedback on projects, and fostering informal communication.

**Microsoft Viva:** is an integrated employee experience platform designed for everyone to connect, learn, and grow. Brings together all the tools employees need to be successful in today’s world of work into one unified solution across four unique experience areas: Connection, Insight, Purpose, Growth

- **Microsoft Viva Connections**: brings together elements of SharePoint,Yammer, Teams and Stream
- **Microsoft Viva Topics:** provides employees access to knowledge and expertise from various Microsoft 365 resources, uses AI to create knowledge pages showing relevant people for each area. It also allows experts to edit and approve the information.
- **Microsoft Viva Learning**: essential hub for learning in the organization. It aggregates content from Microsoft Learn, third parties…
- **Microsoft Viva Insights.** provides data-driven insights to help employees, managers, and leaders improve productivity and wellbeing. It gives personalized recommendations while ensuring privacy, helping everyone in an organization work smarter and find balance.
    - **Personal Insights**: Personalized suggestions to help employees manage their time, focus, and wellbeing.
    - **Team Insights**: Helps managers understand and improve team collaboration and work habits.
    - **Organization Insights:** Offers business leaders insights into the organization’s overall productivity, wellbeing, and work culture.
    - **Advanced Insights:** Provides deeper, data-driven insights for leaders to address complex business challenges.
    - **Viva Insights in Microsoft Teams**: Offers a dashboard in Teams to track and improve productivity and wellbeing.
    - **Viva Insights in Outlook**: Provides insights and suggestions directly in your Outlook inbox to delay delivery of emails or to review outstanding tasks.

## Windows-as-a-Service

**Release Types:**

- **Feature Updates:** Add functionality, released twice a year, these updates add new functionality and are smaller to reduce disruption and cost.
- **Quality Updates:** Fixing things, monthly updates that include security and reliability fixes, either as non-security releases or cumulative updates.

**Servicing Channels:**

- **Windows Insider Program:** Allows early testing of upcoming features; ideal for organizations wanting to preview and test new updates.
- **General Availability Channel:** Receives annual feature updates, suitable for pilot deployments and testing before broader rollout.
- **Long-Term Servicing Channel:** suitable for devices that should only be upgraded after a long period. It provides extended support, with updates only for security and critical issues.

**Deployment Rings:**

- **Preview:** Used for planning and evaluating new features.
- **Limited:** For pilot testing on a small group of devices.
- **Broad:** For widespread deployment after successful testing.

**Deployment Methods:**

- **Modern Deployment:**
    - **Windows Autopilot:** Automate the configuration of new devices through the cloud using predefined profiles and policies. Connects to Entra ID / Intune
    - **In-Place Upgrade:** Upgrades existing Windows versions while preserving data, settings, and applications.
    - **Subscription Activation:** Switches between Windows editions based on user licenses.
    - **Azure AD and MDM Enrollment:** Automatically joins devices to Azure AD and configures them via MDM.
    - **Provisioning Package Configuration:** Uses Windows Imaging and Configuration Designer to apply settings and apps manually using a USB.
- **Traditional Deployment:**
    - **New Computer:** Deploys or reimages a device with a fresh operating system.
    - **Computer Refresh:** Wipes and reloads a device, preserving user state.
    - **Computer Replace:** Transfers user state from an old device to a new one.

## M365 Apps

**Deployment Methods for Microsoft 365 Apps**

- **Deploy from a Local Source with Configuration Manager:** download and deploy Office from network distribution points.
- **Deploy from the Cloud with the Office Deployment Tool (ODT):** Configuration is controlled via a command-line configuration file.
- **Deploy from a Local Source with the Office Deployment Tool (ODT):** downloading and deploying Office from a local network source.
- **Self-Install from the Cloud:** install Office directly from the Office portal.

**Update Channels for Microsoft 365 Apps**

- **Current Channel:** updates 2-3 times a month. Provides the latest features immediately.
- **Monthly Enterprise Channel:** updates monthly on the second Tuesday on a predictable schedule.
- **Semi-Annual Enterprise Channel:** updates every six months, in January and July. Recommended for extensive testing before broader deployment.

## Work management

**Microsoft Project**: is a project management tool designed for complex work efforts with many tasks, resources and dependencies. Project manager can use it to plan and track work that might require dynamic scheduling.

**Microsoft Planner**: integrates with Outlook and Teams, allows employees to organize their tasks on a Kanban board, and it supports the use of @mentions in Word, Excel, and PowerPoint files for task assignments.

**Microsoft Bookings**: simplifies the process of scheduling and managing appointments, includes a web-based booking calendar and integrates with Outlook.

**Microsoft To-Do**: available for iOS, Android, Windows and the web, is an app that empowers you to complete the most important things you need to do everyday.

**Microsoft Forms**: is an easy way to quickly capture the information you need, creating surveys, quizzes…

**Microsoft Lists**: is a smart information tracking app that gives you and your team a flexible way to organize information and work

## Productivity Apps

**Clipchamp**: An in-browser video creation and editing tool with a library of filters, transitions, and stock media, supporting multi-track audio and video editing.

**Delve**:  tool that helps manage your profile and discover content based on personalized insights across the platform.

**Dynamics 365**:  A suite of intelligent business applications that unify CRM and ERP capabilities, offering AI-driven insights and customer feedback management.

**Loop**:  A co-creation platform that enables teams to collaborate on content and tasks across tools and devices with flexible, synchronized components.

**Power Bl**: A cloud-based business analytics tool that connects, visualizes, and analyzes data with interactive reports, leveraging AI and tight Excel integration.

**Power Automate**: allows users to create **automated** workflows between different apps and services, including Microsoft Outlook and Microsoft Teams

**Sway**: A tool for creating interactive, web-based designs that combine text, images, videos, and other media into professional presentations.

**Whiteboard**: A virtual digital canvas for brainstorming and visualizing ideas, enhancing creativity in Teams meetings with drawing tools and organizational features.

## Endpoint management

**Microsoft Intune**: is a cloud-based unified endpoint management solution that simplifies management across multiple operating systems, cloud, on-premises, mobile, desktop, and virtualized endpoints.

**Configuration Manager**: On-premises management tool for deploying apps, updates, and managing desktops, laptops, and servers at scale.

**Co-management**: Allows simultaneous management of Windows devices using both Intune and Configuration Manager, letting transition specific workloads to the cloud.

**Tenant-attach**: Extends Configuration Manager to the cloud, enabling device management and security actions from the Intune admin center.

**Endpoint Analytics**: Provides metrics and insights on Windows device performance and user experience to identify issues and improve efficiency.

**Windows Autopilot**: Cloud service for automating the setup, configuration, and management of new or repurposed Windows devices.

**Intune admin center**: Web-based interface for managing users, devices, policies, and integrating with Configuration Manager for hybrid management.

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

### Global Secure Access

**Microsoft Entra Private Access**: Provides secure, remote access to corporate resources without a VPN, using enterprise applications to manage access and block lateral attacks.

- **Quick Access**: Simplifies access by grouping private resources into a single application with shared access policies based on FQDN, IP, and ports.
- **Global Secure Access App**: Allows for more granular control by creating multiple enterprise apps and for each of these apps, assign users and groups and assign specific conditional access policies.

**Microsoft Entra Internet Access**: protects users and data from web threats by enforcing identity-centric security policies, web content filtering, and continuous access evaluation for SaaS applications and internet traffic.

**Global Secure Access Dashboard:** provides you with visualizations of the network traffic acquired by the Microsoft Entra Private and Microsoft Entra Internet Access services, offering insights through widgets like Global Secure Access snapshots, alerts, usage profiling, and web filtering to help monitor and optimize network configurations.

**Microsoft Entra specific roles:** Manage resources exclusively within Entra ID, such as users, applications, and groups.

**Service-specific roles:** Grant permissions to manage features within specific Microsoft 365 services like Exchange, Intune, SharePoint, or Teams.

**Cross-service roles:** Provide permissions across multiple services, such as security or compliance settings, spanning various Microsoft 365 applications.

## **Microsoft Defender XDR (Extended Detection and Response)**

**Microsoft Defender XDR:** Detects and responds to cyberattacks by analyzing threats across endpoints, email, identities, and apps. It centralizes insights in the Defender portal, integrating with AI and threat intelligence for automated responses.

- **Microsoft Defender for Office 365:** Protects against email and collaboration threats like phishing and malware. It offers real-time threat detection, response automation, and integrates with Office 365 security tools for monitoring and attack simulations.
    - Threat explorer, provides real time report
    - Threat tracker, provides intelligence on cybersecurity issues
    - Anti-phishing protection
    - Attack simulation training feature
- **Microsoft Defender for Endpoint:** Secures endpoints (laptops, phones) against advanced threats through features like antivirus, vulnerability management, and automated incident responses. It integrates with Windows and cloud services.
    - Works with Android
    - Can reduce attack surface
    - Can automate investigation and remediation
- **Microsoft Defender for Cloud Apps:** Secures SaaS apps with features like CASB, threat protection, and app-to-app security. It monitors cloud app activity and improves security posture through the Defender portal.
    - Use CA policies to control sessions in real time
    - Control Shadow IT
    - Protects sensitive information
    - Allow you to meet compliance standards for GDPR and PCI
- **Microsoft Defender for Identity:** Identifies threats like privilege escalation on **on-premises** identity servers by analyzing behavior and providing real-time threat detection and investigation.
- **Microsoft Defender Vulnerability Management:** Continuously identifies vulnerabilities across Windows, macOS, Linux, and mobile devices, prioritizing remediation through risk assessments and Microsoft threat intelligence.
- **Microsoft Defender Threat Intelligence:** Provides enriched threat data for tracking threat actors, prioritizing vulnerabilities, and aiding in threat hunting, integrating with AI tools to support incident response.

**Copilot Integration with Microsoft Defender XDR:** You can switch between ****the embedded experience and the standalone for detailed analysis.

## Compliance

**Microsoft Service Trust Portal (STP):** is a public platform that provides audit reports, compliance information, and resources to help organizations understand how Microsoft cloud services protect data and manage security and compliance.

- **Access Requirements**: Users must log in with a Microsoft cloud services account and accept a non-disclosure agreement to access certain resources.
- **Content Categories**: STP organizes information into categories including Certifications, Regulations, and Standards; Reports, Whitepapers, and Artifacts; Industry and Regional Resources; and Resources for your Organization.
- **My Library Feature**: Allows users to save relevant documents for easy access and set up notifications for updates on saved resources.

**Microsoft Privacy Principals:** Control, Transparency, Security, Legal Protection, No Content, User Benefits

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

- Can only be used with Windows 10 and newer and macOS

**Microsoft Purview Insider Risk Management:** helps organizations detect and manage internal risks by identifying and investigating risky behaviors, such as data leaks and compliance violations.

- **Alerts**: Automatically generated alerts from matching risk indicators that provide a summary view for quick review and investigation.
- **Triage**: review and filter alerts
- **Investigate**: create cases in the case dashboard
- **Action**: send a reminder of corporate policies to users

**Adaptive Protection**: Utilizes ML to assess internal risk levels and dynamically apply adaptive protection controls, allowing high-risk users to face stricter measures while low-risk users maintain productivity.

**Adaptive Protection in Data Loss Prevention**: Automatically assigns DLP policies based on internal risk levels, adjusting to changes in user behavior to effectively protect the organization.

## Purview Compliance

**Audit (Standard)**: Automatically captures and stores user and admin activity logs for 180 days in Microsoft 365 services, providing basic search and export capabilities for security and compliance teams.

**Audit (Premium)**: Expands on the Standard version by offering longer retention (up to 10 years) and provides more bandwidth, customizable retention policies, intelligent insights for investigations, and greater API access for retrieving audit logs.

**Microsoft Purview** **eDiscovery:** helps organizations identify, manage, and deliver electronic information as evidence in legal cases. It allows users to search content across Microsoft 365 services, place content on hold, export results, and create review sets. 

- Place content locations on hold allows preservation of content relevant to an investigation by securing electronically stored information.
- **Copilot in eDiscovery** helps summarize evidence in review sets and convert natural language prompts into KQL queries for efficient investigation.

**Microsoft Purview Compliance Manager:** helps organizations manage and assess compliance by offering prebuilt and custom assessments, workflow tools, step-by-step improvement actions, and a compliance score to track progress and reduce risks across multicloud environments.

- **Controls**: tracks your controls, Microsoft managed controls and shared controls
- **Assessment**: grouping of controls from a specific regulation, standard or policy
- **Regulations**: Compliance Manager offers over 360 regulatory templates to quickly create compliance assessments.
- assesses compliance data continually for an organization

**Information barriers:** used to **restrict communication** and the sharing of information between members of two departments at your organization, **DO NOT** detect **inappropriate language.**

- Works with SharePoint, Teams and OneDrive

**Microsoft Purview Communication Compliance:** detects and manages inappropriate messages. Helps to prevent data security and compliance incidents by monitoring for policy violations and ensuring adherence to organizational standards

- Works with Teams, Exchange, Copilot, Viva Engage and Third party sources

**Microsoft Purview Data Lifecycle Management:** enables organizations to efficiently retain necessary content and delete irrelevant data, ensuring compliance with regulations while minimizing security risks by reducing the amount of stored information.

- **Retention Policies**: These assign the same retention settings to content at the site or mailbox level, ensuring that items inherit the specified retention from their container.
- **Retention Labels**: These apply retention settings at the item level (e.g., folders, documents, emails) and travel with the content within the Microsoft 365 tenant, allowing for more granular control.

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

**Microsoft Purview Data Quality** enables businesses to assess and improve the quality of their data. It uses predefined and AI-generated rules to analyze data, assign a score, and provide visibility into data quality across the organization, helping to easily take corrective action.

## Billing

**Cloud Solution Provider (CSP):** offers flexible, pay-as-you-go Microsoft 365 subscriptions with full support and management by a partner.

**Enterprise Agreement (EA):** provides a cost-effective, three-year licensing solution for larger organizations with 500+ users, including comprehensive support and training.

**Billing Account Options:**

- **Microsoft Online Services Program**: Created for direct Microsoft 365 subscriptions.
- **Microsoft Products & Services Agreement (MPSA) Program**: For an organization that signs an MPSA Volume Licensing agreement to purchase software and online services.
- **Microsoft Customer Agreement**: Created through a Microsoft representative, partner, or independent purchase.

**Consumption and Fixed Cost Models:**

1. **Consumption-Based Price**: Charges based on actual usage (Pay-As-You-Go).
2. **Fixed-Price**: Charges based on provisioned resources, regardless of usage.

**Microsoft 365 Admin Center**: Manages subscriptions, billing statements, payment methods, and billing frequency

**Subscription Plans:**

- **Microsoft 365 for Home**: Personal (for one user), Family (for up to six users). Offering productivity benefits for personal and family use.
- **Microsoft 365 Education**: Tailored for educational institutions with three plans—A1, A3, and A5—providing various productivity and security features for faculty and students.
- **Microsoft 365 Government**: Designed for US public sector employees, with two plans—G3 and G5—and additional Office 365 Government tiers.
- **Microsoft 365 for Business**: For organizations with up to 300 employees, featuring four tiers—Business Basic, Business Standard, Business Premium, and Apps for Business—offering productivity and security tools.
- **Microsoft 365 Enterprise**: For large enterprises with robust features, including threat protection and analytics. Three plans—E3, E5, and F3—plus Office 365 Enterprise tiers are available.

**Base License**: Allows access to features and services in the subscription plan; licenses are assigned to users based on organizational needs.

**User Subscription Licenses (USLs)**: Required for each user to access Microsoft 365 services, managed through the Microsoft 365 admin center.