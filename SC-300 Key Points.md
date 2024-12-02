# SC-300 Key Points

- When adding domains and subdomains to Entra ID, you will first need to add the root --> [example.com](http://example.com/) and then [my.example.com](http://my.example.com/)
- To delete a Custom Domain from the Entra ID Portal, an error may occur if we have not modified all the UPNs, APP URLs and Mail-enabled security groups that included that domain name.
- The first row of a **CSV** must contain the version number
- SharePoint Online (Plan 2) conflicts with SharePoint Online (Plan 1).
- Exchange Online (Plan 2) conflicts with Exchange Online (Plan 1).
- To start **monitoring** a server **again**, the Health Agent needs to be uninstalled and reinstalled
- The authentication protocols supported by Azure are SAML and WS-Fed
- With **MAM without enrollment (MAM-WE**), a work or school-related app that contains sensitive data can be managed on almost any device, including personal devices in **BYOD scenarios.**
- To view the **app governance dashboard**, you need **cloud app administrator** and access from the **Defender Portal**
- With the **usage and insights report**, you can get an application-centric view of your sign-in data to find information about:
    - The top used applications in your organization
    - The application with the most failed sign-ins
    - The top sign-in errors for each application
- To get a Global Admin:
    - Create a self signed user account
    - Sign into the Microsoft 365 Admin Center with the new account
    - Respond to the become the admin message
    - Create a TXT record in the [contoso.com](http://contoso.com) DNS zone
- To establish [contoso.com](http://contoso.com) as the default domain:
    1. Add a custom domain name of [contoso.com](http://contoso.com/)
    2. Create a new TXT record in DNS
    3. Successfully verify the domain name
    4. Set the domain to primary
- The **maximum** number of **devices registered** by user applies to Entra ID registered and Entra ID joined devices
- To activate **Entra ID Seamless SSO** you need to modify the Intranet Zone Settings
- If a group is member of an **Administrative Unit**, only the group is the member, not all the users assigned to the group
- **Administrative Units** are created from the Azure Portal
- At least two **Microsoft Entra Password Protection proxy servers** per forest are needed for redundancy
- A **mail-enabled security group** is a type of group in Microsoft Exchange Online that combines the functionalities of both a distribution group and a security group. Users can only be directly assigned.
- The **What IF tool in CA**, evaluates which policies will be applied to different sign ins
- With **CA** policies you can ensure that users only connect to an app from email clients that use Modern authentication protocols
- **With Session controls in CA** you can establish the **sign-in frequency**
- In **Key Vault** the Purge protection is not activated by default, it’s period by default is 90 days
- During r**etain deleted key period/purge period even admins allowed CAN’T purge** the deleted secrets or certificates (Key Vault Admin CAN)
- To ensure that users can only provide consent to apps that require low impact permissions, you should configure **permission classifications** in your Entra ID tenant
- **SCIM (System for Cross-domain Identity Management)** is a protocol specifically designed for automating user provisioning and deprovisioning between identity providers like Azure AD and SaaS applications
- To connect **Log Analytics with Entra ID** you need to modify the **Diagnostics settings**
- **Action group** is where you can update where email notifications due to determined alerts are sent
- To **monitor OAuth authentication requests**, you need to add Google Workspace connector.
- You can see apps that **don’t need user authentication** in the cloud app catalog in Defender Portal
- If you want users to sign in with certificates issued by a **Certification Authority**, first add the CA to Entra ID tenant
- **NPS (Network Policy Server)** is like a middle man between the **VPN** client and Azure **MFA**. Provides MFA for VPN connections
- **Managed Identities:**
    - Can be controlled with RBAC
    - From **IAM settings** you can control the access that a M**anaged Identity** has to a **Key Vault or Storage Account**
- **User-assigned managed identity** can be assigned to different apps to access a storage account what reduces the administrative effort
    - To control the access to the storage account use **RBAC**
- **Users:**
    - To **bulk create users** you must include accountEnabled, displayName, userPrincipalName, and passwordProfile
    - To **bulk invite** users you must include the **email** address and the **redirection URL**
    - **Job Title** **property** is only available for member users
    - **Usage location** **property** is available for all users
    - Users have **30 days to be restored** after have been deleted
    - Users receive a **one-time passcode** if:
        - They don't have an Azure AD or Microsoft account
        - The inviting tenant didn't set up federation with social (like Google) or other identity providers.
    - **External users**:
        - **Self-service sign up** via user flows set to **NO** don’t allow guest users to **join** the tenant **on their own without invitation**
        - Are managed in the same directory as employees
        - For external users to log in correctly to the desired tenant, the login link must include the tenant ID or verified domain.
        - **External collaborations settings** to block determined domains or allow only users guests from specific domains
        - From **collaboration restrictions** you can enable invitations to a new guests users from a new domain
        - **Reset redemption status** allows a guest user to authenticate with his new updated email
    - **Admin consent and user consent** are configured from **Entra ID Portal**
- **Identity Protection:**
    - The three **Microsoft Graph APIs** for identity risk are **RiskDetection**, which queries risk detections linked to users and sign-ins; **riskyUsers**, which provides information on users flagged as risky; and **signIns**, which details sign-in information, including risk state, detail, and level.
    - The Risky Users report: log-rotation period no limit
    - The Risky Sign-in report: log-rotation period 30 days
    - The Risk Detections report: log-rotation period of 90 days.
    - Leaked Credentials is a Non premium user risk detection
    - Atypical travel and Suspicious Browser are Premium sign-in risk detections
    - **Entra ID threat intelligence** is a detection type for user risk
    - By default, the change password for high risk users policy template include all users and **exclude the current user**
    - Users marked as **compromised** are automatically enforced to reset password on next sign-in
- **Authentication:**
    - By default, Microsoft Authenticator, Temporary Access Pass, OATH and Email OTP are the authentication methods enabled
    - Microsoft Authenticator, Email OTP, OATH, SMS, Voice Call are the methods supported for both **MFA and SSPR**
    - **Email OTP (one-time passcode):**
        - is valid for 30min
        - Must be enabled from Identity Provider
    - To use **Windows Hello for Business,** you need to create:
        - The **KeyCredential Admins** security group, for managing key credentials and enabling devices to authenticate using WHfB, ensures that only authorized admins can perform operations related to key provisioning and management.
        - The **Windows Hello for Business Users** security group, allows designated users to utilize WHfB for secure sign-ins, enhancing authentication methods while ensuring proper control over who can use this feature within the organization.
    - **MFA registration policy** allow users to register MFA for 14 days
    - If you access **Azure Portal with MFA** and then you need to activate a role which requieres an MFA, is not necessary to do the second MFA
    - To block users automatically when they report and MFA request that they don’t initiate, enable the alert function. Entra ID -> security -> MFA -> **Fraud Alert**
    - If a user access an app through a **legacy MFA trusted location**, he won’t be prompted for MFA
    - When administrators require one MFA method for **SSPR**, **verification code** is the only option available
    - **SSPR** supports an email to an address outside your organization
    - Admins need 2 authentication methods for SSPR and cannot use **security questions** for SSPR, despite of SSPR settings
    - We activate **Enable Password Rightback** to be able to use SSPR and so that the password updated in the cloud is synchronized on the premises.
- **MDCA**:
    - **Access Policy** first need to configura a CA Policy to use CA App Control
    - **Activity Policy** is to be notified by a determined user activity
    - **Session Policy** is to block determined user activities
    - **OAuth app policy** allows you to detect and respond to apps that request high permissions and to set thresholds, such as the number of users who have authorized the app
    - **From DEFENDER PORTAL Unsanction** an app helps monitoring its use, you can know from where users access an app
    - To use **MDCA** with an app:
        1. Publish App1 in Entra ID.
        2. Create a CA policy that has session controls configured.
        3. From MDCA modify the Connected apps settings
        4. From MDCA create a session policy
- **Identity Protection:**
    - Anonymous IP sign in is reported as a medium/high risk
    - To connect **Sentinel with Identity Protection**, first create a playbook
- **BrakeGlass account** must:
    - Be created on Entra ID
    - Be Global Admin
    - Logs must be monitored with notifications by Azure Monitor
    - Use a different MFA than all other accounts
    - Must be excluded from automatic usage reviews since they remain inactive for a long time and will be deleted.
- **Smart Lockout:**
    - Is configured in **Password Protection**
    - A locked user will need to reset their password to regain access. This must be done by the user or a Global Admin
- **Terms**:
    - Can’t be re accepted until the expiration date
    - Can be accessed in any device but the device must be registered with Entra ID, if not the user will be prompted to accept the terms
    - From A**udit logs,** you can see who has accepted or rejected the **terms**
    - With CA you can force users to accept the terms
- **Logs**:
    - Can be downloaded in JSON and CSV formats
    - **Sign-in Logs** are retained for 30 days
    - You can choose to download the filtered data, up to 250,000 records
    - The number of records you can download is constrained by the Microsoft Entra report retention policies.
    - Download CA audit logs in **JSON** format
- **PIM**:
    - **Users can’t approve their own request** for rol activation
    - Justification is **always needed** for **approvers** to approve a role activation
    - If you activate a rol for 5h when there was 1min left to the role stop being elegible, **you can use the rol for 5h**
    - **Access reviews** for **roles** are done from PIM
- **VMs:**
    - Can be integrated with Entra ID to improve the security.
    - CA policies can be applied
    - **System-assigned or user-assigned** m**anaged identities** can be assigned **regardless** of **region**
    - Can be assigned the Owner role for a Resource Group but only with **System-assigned managed identity enabled.**
    - A user needs **RBAC roles to:**
        - Use a VM **- VM User Login**
        - Create a VM - **VM Contributor**
- **Entitlement management:**
    - Modify the **Entitlement Management Settings** to allow a user to create new catalogs and add resources to the catalogs that owns
    - A **Connected Organization** provides a way to add a representation of another organization into your tenant
    - You can configure that after a certain number of days since an **external user** loses their assignment to their last access package, they are **removed** from the directory
    - **Access reviews for access package assignments** are done from entitlement management
    - To control the users that can access the Exchange Admin Center, use **group-based access reviews**
    - To create a **catalog**, first create an Azure Logic App, to distribute the catalog use an **Access Package**
    - **Access packages** allow users to get time limited access to a SharePoint site, and allow automatically approvement of access based on group membership
    - **Access Package policy** to enable only determined users access a package

## Entra Connect

- **Application Proxy** allows Entra ID users to access on-prem apps
- **ProxyAddresses** and **UserPrincipalName** must be unique values
- **AttributeValueMustBeUnique**: when a sync object change value of ProxyAddress and now is duplicated
- **InvalidSoftMatch**: when a object that is going to be sync has the same ProxyAddress as other
- Creating an **inbound synchronization** rule for the Active Directory Domain Services connector allow to prevent the synchronization of users with a determinate attribute.
- Allow **outbound HTTPS connections** from an on-prem server to Entra ID is necessary for a firewall to allow Entra ID users connections to on-prem apps

- If the OU that contains a user is not selected to synchronize, the users in that OU won’t be synchronized even if users are selected

![image.png](image%204.png)

- If you **sync a group**, all the users and groups inside will be sync if their OU are selected
- When a group is selected to be **synchronized**, all the users and groups assigned to the first group will be synchronized
- If you disable a **sync user** on the cloud, it stills can access on-prem. If you want to disable the sync user should be on-prem
- **PHS:**
    - Provides a **higher availability** and a faster **disaster recovery** than PTA and federation
    - Is necessary for **Identity Protection** because is the only way hashed passwords are stored in the cloud
    - Requires the least effort regarding deployment, maintenance, and infrastructure
    - Runs every 2 minutes
    - Is automatically enabled when you install **Entra Connect** by using **Express Settings**
- When you select PTA in Entra Connect, a PTA agent is automatically installed on the server where Entra Connect is installed

- Change from PTA to PHS is not automatic, if you want to change in Entra Connect

![image.png](image%205.png)

- If **on-prem connectivity is lost**, and PTA is enabled, only not sync users (cloud only users) will be able to access Entra ID

## Groups

- **Nested groups** do not inherit application access permissions but are affected by a CA
- **Dynamic group rules** consist of property, operator and value--> user.department(property) - eq(operator) "Marketing"(Value)
- **Dynamic groups** can be either user or device groups, but not both at the same time.
- **M365 groups:**
    - Can’t be added under a security group.
    - Only can be added users
- **Managed Identities** only can be added to **assigned security groups**
- **Cloud Only users** can be added to all type groups excluding on-prem ones
- Security and M365 groups, and assign and dynamic groups can get an **access review**
- **Security, M365 and Mail-Enabled groups** can be assigned to **apps**
- Only **users** with **license** can be assigned to **Mail enabled** security groups
- **Roles** can be assigned to **security and M365 groups**
- If a **role can’t be assigned to a group**, you need to recreate the group enabling roles to be assigned
- Access Reviews:
    - Can be created for a group, an app, a subscription role and an Entra ID role
    - The reviewers can be:
        - Group owners
        - Selected users or groups
        - Members (self) - each member can only review his own access
        - Managers of users

## Applications

- **Enterprise Applications**
    - For SAML, to control access by groups, properties, claims
    - **Visible to users** option is what controls if an app is visible on MyApps for assigned users
- **App Registrations:**
    - For OAuth, roles, certificates, secrets
    - Can be restored for 30 days and the full config is restored (App roles, Users and groups, client secrets, and Self-service)
    - To allow an **app to access Graph you can consent:**
        - **Delegated permissions** if its on behalf a signed-user
        - **App permissions** if the apps Graph without a signed user
- An app deployed as a **registered application**, means it will have a **service principal identity**
- An **app deployed in 2 VMs** will use a **user-assigned managed identity**
- **MyApps** collections allow users to group related apps
- The **approver** of an app will automatically become **owner** of the Group of assigned users to an app after **self service** is configured.
- To be able to grant **Admin Consent**, is compulsory to enable admin consent request in tenant settings

## By default

- All members can create app registrations and manage all aspects of the apps they create,
- **Guest** users do **NOT** have the ability to create **apps**
- All users have the ability to give apps consent to access company data on their behalf
- **Cross-tenant access settings** by default**:**
    - **Inbound settings** allow external users and applications to access resources and apps in your tenant after invitation.
    - **Outbound settings** permit your users and applications to access resources in other tenants
    - **B2B direct connect** are not allowed
- Microsoft Entra **Password Protection default** initial setting is **Audit mode (report only)**

## Roles

- To manage **Entra ID roles** use Privileged Role Administrator
- To manage **Azure resources** **roles** use User Access Administrator
- The **maximum number of roles** that can be created is 5000 for all tenants regardless of the license.
- **Elegible roles** can’t be assigned to managed identities
- You can **compare** user **permissions** through **Microsoft 365 Admin Center**
- You can clone **Azure subscription roles** to make new Azure subscription roles.
- **Permissions**:
    - [Microsoft.App](http://Microsoft.App) - permissions related to container apps
    - [Microsoft.Security](http://Microsoft.Security) - permissions to enforce network rules
    - [Microsoft.Network](http://Microsoft.Network) - permissions related to firewall and app security groups
- **Global Administrator, Security Administrator, Exchange Administrator, SharePoint Administrator** can perform actions that interact with Identity Secure Score
- **Global Administrator and Privileged Role Administrator** are the only ones who can by default approve role activation
- **Global Admin and User Admin** are not affected by naming policy for groups
- **Identity Governance Administrator** can create and manage access reviews for Azure resources
- **Privileged Role Admin** can create access reviews for Entra ID roles
- **User Administrator** can create Access reviews, Reset passwords for non-administrators, Manage licenses, Create and manage users and groups. Restore users
- **Cloud Application Administrator** gives the same permissions as the **Application Administrator** role minus the ability to manage the Application Proxy. They are not added as owners when creating new application registrations. Both can provide Admin consent.
- **Application Developer** can create application registrations independent of the 'Users can register applications' setting. Can’t assign users to apps
- **Global Admin** is the only one who can reset the password for a user admin, global admin and password admin
- **Device Administrator** is local admin for Entra ID joined devices
- **Cloud Device Administrator** can manage device settings
- **Security reader** can review history reports for completed Access reviews
- **Security Operator** provides some permissions for Identity protection such as viewing reports and confirming or denying risks
- **Security Administrator** provides full access to Identity protection minus the ability to reset user passwords. Can create policies. Can manage security defaults
- **Privileged Authentication Administrator**: Set or reset any authentication method (including passwords) for any user, including Global Administrators
- **Authentication Administrator** can reset passwords and manage MFA settings
- **Helpdesk Administrator** can change passwords, Invalidate refresh tokens, Create and manage support requests with Microsoft for Azure and **Microsoft 365 services**, and MONITOR service health.
    - CANNOT CREATE and MANAGE support tickets.
- **Service Support Administrator** can read service health information and manage support tickets.
- **Owner, Contributor, or Support Request Contributor role** can create a support request
- With PIM you can’t manage:
    - Account Administrator
    Service Administrator
    Co-Administrator                                                                    Security Contributor
- **Key Vault:**
    - **Key Vault Administrator** can perform all data plane operations on Key Vault
    - **Key Vault Contributor** roles don't allow to get access to certificate
    - Key Vault **Certificates Officer** can access certificates
    - Key Vault **Crypto Officer** can manage and create keys
    - Key Vault **Secrets Officer** can **read and** **update** secrets
    - Key Vault **Secrets User** can **read** contents of secrets

- Contributor role for a Resource Group, can be assigned to Users, Groups, VM and Apps
- Entra ID Admin Center:
    - User Admin
    - Device Admin
    - Identity Governance Admin
- Microsoft Compliance Admin Center:
    - Records Management
    - Quarantine Administrator role group
- Microsoft Endpoint Manager Admin Center
    - Endpoint Security Manager
    - Intune Role Administrator

## License

- **Usage Location Property** has to be configured before licenses can be assigned, Azure services cannot be used in all locations so you first need to know the user's location
- Assign licenses to groups:
    - Automatically assign multiple licenses to users based on the security groups they belong to, this works with Azure AD Premium P1 and P2, Office 365 E3,A3,G3...
    - Only available through the **Microsoft 365 Admin Centre**
    - Licenses are assigned only to the **direct-assigned users to the group.**
    - You can assign a license to a security group **even if it contains devices** despite of its assigned or dynamic
- To **remove licenses** quickly, use the **Entra ID Admin Center** **Licenses blade**
- To ensure that **External Identities** pricing is based on monthly active users (**MAU**), you should configure a **linked subscription**
- P1 and P2
    - **Administrative Unit** Support
    - Ingest Entra ID **logs** into **Sentinel**
    - Application Proxy
    - Company Branding (available with Office 365 licenses too)
- P2 only
    - PIM
    - Entitlement Management
    - Identity Protection
    - Allow member users that are not Global Admin perform an Access Review, guest users < 50k free

## Permissions Management

- Can manage **AWS** and **GCP**
- To allow a user **access**, add him to the **Permissions Management security group**
- From the P**ermissions subtab**, use a **quick action** to replace permissions with others
- To automatically monitor permissions and create and implement right-size roles, assign the **Contributor role to the service principal of Permission management**
- **The Microsoft Entra Insights** tab shows you who is assigned to privileged roles in your organization
- **PCI:**
    - Can be reviewed on **Dashboard**
    - Helps to monitor the **permissions usage of a user**

![image340.jpg](image340.jpg)

- **Authorization System Name** indicates in which scope a user can request or approve access
- Viewers can only request access
- Approvers can approve access
- The **User Access Administrator** role allows users to manage role assignments on the subscription level without accessing resource content, ensuring least privilege by granting only necessary permission management.
- CIEM in Microsoft Entra Permissions Management enables centralized permission control. Assigning this identity the *User Access Administrator* role allows secure, least-privilege permission management across resources.

## Comands

- **Set-MsolCompanySettings :** change the tenant default options
- **New-AzureADMSInvitation** : cmdlet to invite a guest user
- **Set-MsolUserLicense** : cmdlet to remove user licenses with least amount of effort
- **Update-MgPolicyPermissionGrantPolicyExclude** : prevent users from creating new user accounts
- **$vm = Get-AzVM - ResouceGroupName myResourceGroup -Name vm1** : lo que se hace es asignar los resultados a la variable $vm, se busca de entre todos los objetos del resourceGroup myResourceGroup el que su name es igual a vm1
- **$displayname = Get-AzADServicePrincipal -displayname "vm1"** : asigna los resultados a la variable $displayname, se busca de entre todos los ServicePrincipal el que su displayname es igual a vm1
- GRAPH:

SigninLogs  // Selecciona la tabla de registros de inicio de sesión como fuente de datos
| where ResultType == 0    // Filtra para mostrar solo los inicios de sesión exitosos (ResultType igual a 0)
| summarize login_count = count() by Identity  // Agrupa los registros por usuario (Identity) y cuenta el número de inicios exitosos para cada uno
| render columnchart   // Muestra los resultados en un gráfico de columnas

T1>23,26,72 - 7,9,   15,16,18,20,   23,26,   31,33,34,35,36,   52,56, 69,   72,75

T2>6,   13,18,   24,26,   31,33,36,40,   41,48,   71,72,77

T3>45,47 - 2,5,9,   11,13,15,17,   23,29,   42,43,44,45,47

T4>7,18,58,62,70,73,75 - 2,7,   14,18,20,   26,30,   31,37,   44,50,   51,52,58,   61,68,70

65-74 repasar Permissions Management

Caso A: T1-47   T3-36   T5-1,2,3  

Caso B: T1-48,49,50   T2-55,56,57   T3-27   T4-40,42   T6-1,4   T8-2

| **FALLOS** | Topic 1 | Topic 2 | Topic 3 | Topic 4 | Caso A | Caso B |
| --- | --- | --- | --- | --- | --- | --- |
| 1-10 | 4-2-0 | 4-1-0 | 4-2-0 | 6-2-0 |  | 0 |
| 11-20 | 2-2-0 | 1-1-0 | 6-1-1 | 5-2-0 |  | 0 |
| 21-30 | 6-1-0 | 6-2-0 | 4-1-0 | 2-1-0 |  | 0 |
| 31-40 | 4-2-0 | 4-3-1 | 1-0 | 4-1-0 |  | 0 |
| 41-50 | 4-0 | 4-1-0 | 5-4-2 | 1-1 |  | 1 |
| 51-60 | 5-1-0 | 2-0 |  | 3-2-0 |  |  |
| 61-70 | 4-0 | 2-0 |  | 3-3-0 |  |  |
| 71-80 | 4-1-0 | 3-1-0 |  | 3-0 |  |  |
| 81-90 |  | 0-0 |  |  |  |  |
| TOTAL | 33/79
9/79 | 26/82 9/82 | 20/48 8/48 | 27/75 12/75 | /5 |  |
- Un elemento Action en la definición de roles establece que capacidades de administración están permitidas, un NotActions indica que capacidades se restan al Action para definir la lista final de operaciones permitidas
- A record es para mapear un hostname con una IP
- HelpDesk Administrator no incluye los permisos necesarios para implementar Entra ID Terms of Use, Conditional Access Administrator, Security Administrator y Global Administrator si pueden
- Si los usuarios podían entrar por defecto a las aplicaciones y luego se pone que por defecto no pueden entrar, seguiran con acceso a las aplicaciones que ya habían entrado pero no tendrán a las nuevas
- Es necesario un Admin Role es el unico Entitlement Management Role que tiene los permisos necesarios para crear una Connected Organization
- Azure Cosmos DB no es un destino válido para enviar los Microsoft Entra ID Diagnostics Logs
- No se pueden mover los Packages de Catalog, solo se pueden borrar de uno y crear en el otro
- Windows server es el unico SO que soporta la instalación del Connector Agent que facilita la comunicación entre Azure AD Proxy Service y las aplicaciones
- Los dos directorios que Microsoft mantiene son el directorio de la galería de aplicaciones y el directorio de servicios de Microsoft
- Para desarrollar aplicaciones Multiinquilino se recomienda seguir el permiso de acceso mínimo de los usuarios para asegurarse de que la aplicación solo solicita los permisos requeridos
- Las dos maneras de declarar los roles de aplicación mediante Azure Portal son el uso de los roles de aplicación y el editor de manifiestos de la aplicación
- Windows Hello for Business solo vale para cuando el usuario trabaja desde el mismo ordenador puesto que los datos biométricos se almacenan localmente en la máquina
- 
- Los registros de auditoría de Microsoft Entra proporcionan registros de las actividades del sistema para los informes de cumplimiento
- Azure admite la exportación de datos de registro a varias herramientas de SIEM de terceros como son Splunk, IBM QRadar y ArcSight
- Si tiene aplicaciones heredadas locales publicadas para el acceso a la nube, lo primero es implementar un Application Proxy
- Para usar SmartLockout, el tiempo de bloqueo de Entra debe ser menor que el de la cuenta de AD DS y máyor que el restablecimiento del bloqueo de cuenta de AD DS
- Private Key y Windows Hello no son opciones validas para la vinculación de CBA (Certificate Based Autentication)
- En AAD Provisioning Logs de Log Analytics Query podemos ver los usuarios creados por una tercera parte