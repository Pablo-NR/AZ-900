# MS-900 Key Points

- Content at rest is encrypted using BitLocker
- Microsoft Entra ID provides authorization and RBAC at the tenant layer
- Exchange online contain mailboxes from multiple tenants
- Data Protection can be selectively applied to aplications
- Only **Global Admins** can create **support requests**
- **Information Rights Management (IRM)** classify documents to restrict permission to content
- P2 para PIM, P1 para SSPR
- To ensure data you can use **service-level encryption using customer-provided key**
- Attack Simulator provides 3 attacks:
    - brute force password
    - spray password
    - phishing
- To implement least privileged access use Just In Time access (JIT) and Privileged Access Workstations (PAW)
- If you have a problem with SharePoint you can:
    - Contact Microsoft Technical support by telephone
    - Create a new service request from the Microsoft 365 admin center
- To give **feedback** Windows Feedback Hub

- When you enable **external access**, users can send sharing **invitations** for **specific content**
- **Windows 365 and Azure Virtual Desktop** are both virtual desktop solutions, also known as **Desktop-as-a-Service**.
- **Microsoft 365 and all Office apps like OneDrive are** a **SaaS**

![image.png](image.png)

- **Microsoft SharePoint, Microsoft Exchange and Microsoft Skype for Business** offer **hybrid** abilities
- **Power Bl** can customize a usage report for **Microsoft Yammer**
- **Microsoft Bookings:**
    - Uses Teams for virtual meetings and provides SMS notification for appointments
    - **Staff page** to view technician’s working hours
    - **Booking page** to schedule customer appointments
    - **Booking calendar** to schedule vacation time for technicians and business closures for the company
- Exchange Server and Exchange Online ****support the same minus:
    - Custom EWS throttling settings and apply security updates to Exchange server only for **Exchange server**
    - Use Microsoft Bookings and use M365 groups to send and receive emails only for **Exchange Online**
- **Microsoft Dynamics 365** is not part of Microsoft 365, provides a remote assistance solution, a customer relationship management solution, an enterprise resource planning and IA tools
- In **Microsoft Stream**:
    - Video files are stored in SharePoint Online
    - Video files can be accessed from Microsoft Teams and Yammer
- **Finding files** in **OneDrive** is easier with the **Graph**. It suggests files for you based on your connections with others, how you got the files, and when you last looked at them.
- If **users** use **Microsoft Entra ID credentials** to sign in to their devices, they would be able to access **OneDrive** from **remote locations** because they are using a trusted identity
- **Microsoft Planner** allows track project task within a Microsoft maintained unified interface that can be shared and updated across multiple users

- All **legacy apps** will remain in a **hybrid** environment after migrating to Azure
- **Microsoft 365 Roadmap** allow to determine the **lifecycle** of products and features in Microsoft 365
- **Microsoft 365 Roadmap** portal displays the month and year a feature of Teams will be GA and allows companies to provide feedback about features.
- **Microsoft Access** is a database application design and implementation tool that you can use to track important information
- **Microsoft Access** needs to be **installed on a** **local computer** to be used by a licensed user
- When someone includes **@xxx** in a word document, xxx will receive an email with a preview of the document text and the associated comment, he can click the link and open the document exactly on the comment or can respond to the comment directly from the email.
- You can **deploy** Microsoft 365 apps from the **on-premises** using **Configuration Manager**, **on-premises** using **ODT**, **cloud** using **ODT** and **cloud** with **self install**
- **Configuration Manager** allows to manage power settings for on-premises servers
- **Windows 365 (cloud PC)** provisions automatically a VM after assigning a license to a user
- **Enterprise Mobility + Security** allows to register a **personal** home **device** with the company
- After an unplanned outage a **Post-Incident Review (PIR)** will be delivered within **48 hours** of incident resolution
- **Microsoft 365 Usage Analytics**:
    - **EnabledUsers**: Number of users enabled to use the product in the month.
    **ActiveUsers**: Number of users active in the month.
    **MoMReturningUsers**: Number of users active in the month that were also active in the preceding month.
    **CumulativeActiveUsers**: Number of users active in the month plus any preceding month.                                                                                                                          **Data Loss Prevention**: Number of rules applied to information that is classified as sensitive
    - **Usage**: number of active users and the primary activities of each product for the last 12 months
    - **Communication**: identifies patterns in the use of Microsoft Teams and Yammer among users
    - **Collaboration**: identifies the number of documents that are shared internally or externally
    
- **Microsoft Viva** connect the correct customer service associate to a customer
- **Microsoft Viva Insights:**
    - MyAnalytics Offers **employee work** and **collaboration metrics**, it’s **included in office 365 E5 license**
    - MyAnalytics supports Outlook add-ins and weekly email digests
    - **Workspace Analytics** can be purchased **only as an add-on license**, permits upload of **custom organizational data** and provides **team work** and collaboration metrics
    - Workspace Analytics supports PowerBl templates
    - Microsoft **Viva Insights** can be added as an app in **Teams**
    - **Outlook** includes an add-in for **Viva Insights**
    - **Viva Insights** includes a web-based **dashboard**
    - Your personal insights can’t be seen by your manager or an administrator
- **Viva Learning** aggregates third-party training content and internal company content, and allows managers to assign, track and report on training

- **Targeted release** channel allows to install new features **as soon as** it becomes available
- **Current Channel (Preview)** receives feature updates as soon as they are available.
- **Monthly Enterprise Channel** receives updates once a month on a predictable schedule.
- **Semi-Annual Enterprise Channel (Preview)** receives updates every six months, a few months before these are made available to **Semi-Annual Enterprise Channel**
- **Windows Update** offers limited control over feature updates and the ability to manually defer updates
- **Windows Update for Business** update periodically without on-premises
- **Windows Server Update Services (WSUS)** updated from on-premises, used for scheduling upgrades and updates to be executed consistently for all devices
- **Microsoft Endpoint Configuration Manager** updates and monitors using a single system

## Admin center

- The Microsoft 365 **admin center** provides **support** for products in the **General Availability (GA) phase and Public preview**
- To deploy an **add-in** to Outlook go to **M365 admin portal** and go to **Services & adds-ins** menu
- **Email activity**: report that shows the number of meeting interactions by users
- **Mailbox usage**: report that shows the amount of storage used by users
- **Email apps usage**: report that shows the number of unique users that use Outlook on the web

## Microsoft Intune

- **Microsoft Intune** is a mobile device management (**MDM**) and mobile application management (**MAM**) solution that enables you to apply **security policies** and restrictions to mobile devices, such as smartphones and tablets.
- **Microsoft Intune** can deploy apps into devices.
- **Microsoft Intune** lets you manage apps from third-party stores, supports volume licensing for iOS and Android store apps, and handles both internal (line-of-business) and public-facing apps efficiently.
- **Microsoft Intune** prevent users from copying company data from managed applications installed on unmanaged devices
- If a user looses the PC, from Intune you can protect the data on it by clicking on **Retire, Wipe, Delete and Fresh Start**
- To requiere a **PIN** to access an app, use **app protection** in Intune
- You **cannot assign apps** to devices that are **not enrolled** with Microsoft Intune
- You can assign **wrapped apps**, or apps that incorporate the **Intune SDK**, to devices **not enrolled with Intune**
- You can install available **apps** from the **web-based Company Portal** to devices **enrolled** and **not enrolled** with Intune
- In Intune **Device Enrollment** is where you can add new devices, **Devices** are where you can manage and view registered devices
- Intune can define **where** corporate data is **stored**
- In Intune if you **wipe** a device you **delete personal data too**
- Intune connector for AD:
    - add entries to AD domains for computers that enroll using Autopilot
    - don’t allow access to Exchange servers if devices are compliant with preset Intune policies
    - The connector don’t processes certificate request from devices that use certificates for authentication
- Intune Policies:
    - Protect access to Exchange Server on-prem mailboxes
    - Don’t require a MDM solution
    - Don’t support apps that connect on-prem SharePoint

## Compliance

- To **retrieve data** for employees who request personal data **under** General Data Protection Regulation (**GDPR**) guidelines, you have to create a **data subject request case**
- **Service Trust Portal:**
    - Provides **audit** and **assessment reports** for Microsoft 365 cloud services, including Exchange Online and SharePoint Online.
    - The **penetration** test **report** of an specific office is located on **Regional Compliance page of the Service Trust Portal**
- Microsoft Purview Information Protection:
    - For **document classification** and **protection** you need an **Azure subscription** in the tenant and to **enable** the **default** Azure Information Protection **policy**
    - Works with on-prem and cloud
    - Works with data on devices and in Office apps
    - Can **classify** and **label** emails and documents in the organization
    - You can supplement the default templates to apply restrictive controls
    - Installing the Information Protection Client installs a Information Protection bar to Excel
    - Implementing Azure Rights Management (RMS) for individual users account you can access a document encrypted by Information Protection
    - Detects sensitive data across SaaS apps
- **Sensitivity labels:**
    - Control read and write access to docs
    - Can be customized
    - Can be automatically applied
    - Allow users in another organization to review the content of an email for a number of days
    - Can be applied to content in Teams, SharePoint, M365 groups
    - Can’t be applied to mails
- **Microsoft Purview Information Protection Scanner** detects sensitive contents uploaded to cloud
- In order to configure a data governance strategy that allows for **data classification:**
    - Publish **labels** to **classify** docs
    - Apply **supervision policies** to ensure **classifications** are **enforced**
    - **Delete** documents that are **no longer** **used** applying **retention policies**
- **Content search eDiscovery** in the **Microsoft 365 compliance center** can search for in-place content such as email, documents, and instant messaging conversations in your organization. Searches across Exchange Online mailboxes, SharePoint Online sites and OneDrive for Business accounts, Teams, Microsoft 365 Groups and Yammer Groups
- **Customer Lockbox** ensures that Microsoft can’t access your data during service operations without your approval, so you authorize any request for access to your content
- Recommendations impact in descendant:
    - Preventive
    - Detective
    - Corrective
- Communication compliance policies identify email risk and provides workflows to remediate

## SharePoint

- **SharePoint Online** allows **co-author** files with other users, supports third-party apps and can track the activity of files that are accessed in SharePoint team site
- A **SharePoint site** is created when you create a **Microsoft 365 group** and **vice versa**
- You can **disable** the **enterprise social collaboration feature** in SharePoint
- You can use **Teams**, **Yammer** and SharePoint **Newsfeed** to provide enterprise social features in SharePoint
- You **cannot use different** enterprise social **collaboration services** in SharePoint **simultaneously**

## Teams

- Microsoft **Teams Phone** supports **direct routing**
- In a **Teams meeting**, the **screen sharing** capability is supported for up to **1,000** participants of a meeting. While **meetings can have up to 20,000 participants**, the remaining participants have view-only capabilities.
- Microsoft Teams allow users outside the company **collaborate** on a project in **real time** by using a **whiteboard**
- Types of apps that can be used on teams:
    - Core apps that are part of Teams.
    Other apps created by Microsoft.
    Third-party apps by partners (validated by Microsoft).
    Custom apps created by your own organization.
    - Microsoft Store apps can’t be used with teams
- **Private teams** are only for **specific people** from the organisation, **Public teams** are available for **anyone** in the **organisation**
    - **Standard channel** are for **everyone in** the **team**, **Private channel** are for a **subset** of people.
    - **Shared channels** allow adding members and not members of the team, but by default don’t allow adding guests.

## Defense

- **Microsoft Office 365 Advanced Threat Protection** allows you to protect against unidentified **malware, viruses, and malicious URLs**
- **Microsoft 365's Advanced Threat Protection (ATP) anti-phishing features** are designed to help protect against malicious content, including harmful attachments in emails
- **Microsoft Defender for Cloud Apps:**
    - Provides insight into which apps are being used in the organization and the risk levels for the apps
    - Detects unusual behavior across apps and users as well as potential ransomware
    - Prevents data leaks from uncompliant apps and limit access to regulated data
    - Integrates with **Graph** to generate Microsoft Defender for Identity alerts
    - Integrates with **Power Bl** to automate the response when alerts are triggered
    - Doesn’t include a VPN
    - Can be used to asses the **regulatory compliance** of Cloud Apps
- **Microsoft Defender for Office 365:**
    - Can configure policies to set the appropriate level of protection
    - Automated Investigation and Responde (AIR) capabilities can start a playbook to automate investigation
    - Attack simulator can prevent a real attack

## Entra ID

- With Entra ID **Privileged Identity Management** you **protect admin roles**
- **Password Hash Synchronization (PHS):** The user's credentials are synchronized from on-premises to the cloud, and the user can authenticate against the cloud using their on-premises credentials.
- **Pass-Through Authentication (PTA):** The user authenticates against the cloud, but the credentials are redirected to on-premises for verification; the credentials are not stored in the cloud.
- **ADFS:** The user authenticates against on-premises, and the credentials are never sent to the cloud; after authentication, the user receives a token that allows access to cloud services. It’s the only way a user can authenticate using methods not supported by Entra ID
- **Entra ID** **can’t** manage Entra ID **joined** devices using a group **policy**
- Entra ID don’t support LDAP or ADAL
- Entra ID doesn’t need domain controllers

## Billing and licensing

- You can pay Microsoft 365 monthly or annually
- **Billing profile** provides customization of invoices and payment options
- **Billing invoice** provides a summary of charges
- You can pay with debit card, credit card and with check
- In order to **buy** new **licenses** you need the **Billing Admin role**, if you need to **assign** a **license** to a user you need the **User Admin role**. With Global Admin role you can do both
- To get an **Enterprise Agreement** you have to contact a **Cloud Solution Provider (CSP)**
- **Microsoft 365 apps for Enterprise** allow installation by using:
    - Microsoft Intune                                                                                                                                   Office Deployment tool                                                                                                                               Click-to-Run                                                                                                                                                                                                                                               System Center Configuration                                                                                                                                                                                                                              Enabling auto-deployment of Office 365 apps for all devices                                                           Install from the Office 365 portal with dashboard                                                                                  Don’t support Windows installer package
- **Microsoft 365 apps for Enterprise** can change the update channels from:
    - Intune                                                                                                                                                                       Office Deployment Tool                                                                                                                                       Group Policies
    Microsoft Configuration Manager
    Servicing profiles
    Microsoft 365 admin center
- Microsoft 365 for Enterprise can have a local copy of Outlook that connects to an Exchange Server Instance
- Enterprise E1 allows Delve
- Enterprise E3 allows eDiscovery
- Enterprise E5 allows advanced eDiscovery
