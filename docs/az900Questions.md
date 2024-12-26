# AZ 900 Questions and their answer

- Management Group can have 6 levles of depth [Important facts about management groups](https://learn.microsoft.com/en-us/azure/governance/management-groups/overview#important-facts-about-management-groups)

- Archive Access tier needs to be set at the blob level, not at the storage account level.

- Azure Advisor [What is Azure Advisor](https://learn.microsoft.com/en-us/azure/advisor/advisor-overview) and integrates with Microsoft Defender for Cloud to give security advise.

- Azure DNS is not providing DNSSEC right now.

- Azure File Sync is used with a windows server to access your data locally. It uses SMB, NFS, and FTPS protocols [Documenation](https://docs.microsoft.com/en-us/learn/modules/describe-azure-storage-services/7-identify-azure-file-movement-options)

- Passwordless Autentication Methods (Windows Hello for Business, FIDO2 security keys, Certificate-based authentication) (https://learn.microsoft.com/en-us/training/modules/describe-azure-identity-access-security/3-authentication-methods) and (https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-passwordless)

- User defined Routes are used in a virtual network to change the way how traffic is routed. (https://learn.microsoft.com/en-us/azure/virtual-network/virtual-networks-udr-overview)

- Quick Response time is reached with Low Latency.

- If a policy defines that a ressource e.g. virtual networks in resource groups it only will be reported as a non-compliant resource

- Microsoft Defender for Identity (formerly Azure Advanced Threat Protection, also known as Azure ATP) implements a security solution for the users who are on on-premises Active directory with following features: Monitor User login/logout, Monitor Active Directory User account changes, Monitor Machine Account

- Virtual Machine must-have: Azure Virtual Network, NIC

- Azure free account can be used to bring load into production. The billihng of resources that are not covered by the free account are billed pay-as-you go

- Azure Data Lake can be used to integrate Apps (e.g. PowerBI), scalable storage, infrequently (https://learn.microsoft.com/en-us/power-bi/transform-model/dataflows/dataflows-azure-data-lake-storage-integration)

- You should use Azure SQL, Azure PostgreSQL, or Cosmos DB for frequently accessed data.

- PowerShell 6.2.4 and later is compatible on all OS platforms. However, Microsoft recommends PowerShell 7.x. [Compatability of version with differnt OS](https://docs.microsoft.com/en-us/powershell/azure/?view=azps-4.5.0)

- Tags from resource groups are not inherited to resources (https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-using-tags)

- Defender for Identity enables SecOp analysts and security professionals struggling to detect advanced attacks in hybrid environments to:

Monitor users, entity behavior, and activities with learning-based analytics
Protect user identities and credentials stored in Microsoft Entra ID
Identify and investigate suspicious user activities and advanced attacks throughout the kill chain
Provide clear incident information on a simple timeline for fast triage

- Azure blob storage that is infrequently accessed is Cool and Archived tiers

- Azure blob storage that is frequently accessed is Hot Storage tier

- Azure management groups are used for organizing resources in Azure e.g. different groups of users

- The Azure subscription gives you authenticated and authorized access to create Azure resources and services

- Only one free account subscription is allowed per User.

- Azure Databox is the prefered solution to transfer huge amounts of data to the cloud. 80TB in maximum and does not need network

- Conditional Access can help to block the sign-in from untrusted locations.

- Azure AD Device management helps register our devices to azure.

- Microsoft Defender for Identity leverages your on-premises Active Directory signals to identify, detect, and investigate advanced threats, compromised identities, and malicious insider actions directed at your organization

- Azure File Sync helps us to configure cloud tiering so the most frequently accessed files are replicated locally, while infrequently accessed files are kept in the cloud until requested.

- Network Security group review

- Review [Support Plans](https://azure.microsoft.com/en-us/support/plans/)

- Azure content delivery network is an efficient way to distribute web content to users across the world

- **Azure HDInsight** is a managed Apache Hadoop service to analyze streaming or historical data. Lets you run Apache Spark, Apache Hive, Apache Kafka, Apache HBase in the cloud.

- Not all regions offer availability zones, check [Azure Regions with availabilty zones](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview)

- Azure Functions is a Platform as a service (PaaS)

- An appropriate support plan has to be bought separately. It does not come as part of the App service plan e.g.

- Local network gateway represents the on-premise VPN Device

- The Azure CLI, Azure Powershell, and Azure Portal are all options on MacOs, Linux and Windows to create resources

- VMs can be deallocated automatically for saving costs: (https://learn.microsoft.com/de-de/rest/api/compute/virtual-machines/power-off?view=rest-compute-2023-10-02&WT.mc_id=modinfra-32183-socuff&tabs=HTTP)

- SLA for Virtual machines deployed across two or more Availability Zones at least Availability 99.99% of the time.

- Azure Policy can be grouped into Initiative Defintions to have them in one place.

- Azure DDoS Protection has the following features: DDoS Infrastructure Protection, DDoS Network Protection and DDoS IP Protection [Table](https://learn.microsoft.com/en-us/training/modules/introduction-azure-ddos-protection/4-when-to-use-azure-ddos-protection)

- Identity Secure Score helps in identifying the identity secure score to provide the recommendations in Azure AD
