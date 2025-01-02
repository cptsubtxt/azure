# AZ 104 Questions and their answer

- A loadbalancer from basic sku can loadbalance between machines only when the vms are in the same availability set or virtual machine scale set (https://learn.microsoft.com/en-us/azure/load-balancer/skus#skus)

- Azure does not allow to scale Azure Container Instances. One has to delete the ACI and reapply the ARM Template with new settings for CPU and Memory. (https://docs.microsoft.com/en-us/azure/container-instances/container-instances-update#properties-that-require-container-delete)

- Inbound NAT rule are used to forward traffic from a specific port of a front end IP address to specific port of a back-end VM.

- Review process of creating and managing an Azure container registry (Create Container Registry, Select Pricing Tier, Configure Container Registry Settings, Set up authentication and security, Access and manage container images)

- Geo redundant Storage, review https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy#geo-redundant-storage

- Move VMs to a different resource group, subscription and region (https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/move-limitations/virtual-machines-move-limitations?tabs=azure-cli)

- Review Administrative Unit Management (https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/administrative-units#administrative-unit-management)

- You can also send security events of virtual machines to Log Analytics workspace.

- If there is a read lock on a resource group no ressources cannot be moved to this RG

- If a user only has reader role ressources cannot be moved to RG by that user.

- When a resource group already contains resources from a App Services resource no other App Services Resources cannot be moved into that Resource Group --> [Move across subscriptions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/move-limitations/app-service-move-limitations#move-across-subscriptions)

- Move across subscriptions: The destination resource group must not have existing App Service Resources like Web Apps, App Service Plans, Uploaded or imported TLS/SSL certificates, App Service Environments

https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/move-limitations/app-service-move-limitations#move-across-subscriptions

- A network interface can only be attached to a virtual machine when it resides in the same region.
  https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-network-interface

- Only resources in the same geographic reason can be backed up using recovery services vault service
  https://docs.microsoft.com/en-us/azure/backup/backup-azure-recovery-services-vault-overview
  http://docs.microsoft.com/en-us/azure/backup/backup-azure-arm-vms-prepare

- At the time of Microsoft Entra join we add the following security principles to the local administrator group
  The Microsoft Entra Global Adminstrator role
  The Azure AD Joined Device Local Administrator role
  The user performing the Microsoft join

- An Azure Container Instance has to be deleted first and you have to redeploy ARM ACI deployment template.

- ACI group is similiar to AKS Pods

- Version-level immutability can only be enabled once and cannot be disabled any more.

- Administrator reset policy differences
  Administrator accounts does not answer security questions

- Virtual Networks can be moved across Regions. VMs, VM Scalesets etc. cannot be moved across regions.

- Steps to add a custom domain name are: Create a Custom Domain in Entra ID, add domain information on your domain registrar site and last step verifiy that you are the owner of the domain.
  see: https://learn.microsoft.com/en-us/entra/fundamentals/add-custom-domain

- In order to add a network interface to a virtual machine, the machine needs to be stopped first.

- IP Flow Verify checks if a packets are allowed or denied to or from a virtual machine

- Packet capture should be used to check on any network intrusions, packet capture is a feature in Azure Network Watcher that enables detailed analysis of network traffic. By capturing packets traversing the VPN tunnels, you can identify patterns or anomalies, including latency issues, by examining timestamps and response delays in the captured data.

- Steps to set a container registry https://learn.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-prepare-registry

- Learn Storage Types https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy#geo-redundant-storage

- Availability Set encourages Scalability & Availability https://docs.microsoft.com/en-us/azure/virtual-machines/windows/manage-availability

- Privilegded Access Management - https://learn.microsoft.com/en-us/entra/fundamentals/licensing#microsoft-entra-privileged-identity-management

- P2 adds certrain security Policy Services e.g. conditional access policies

- How to create an anomaly alert: https://learn.microsoft.com/en-us/azure/cost-management-billing/understand/analyze-unexpected-charges#create-an-anomaly-alert and how to edit it: https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-manage-alert-rules

- Identify scope in Azure: https://learn.microsoft.com/en-us/azure/role-based-access-control/role-assignments-steps#step-3-identify-the-needed-scope

- RBAC - deny assignments take precedence over role-based access (RBAC assignments)

- "Restore VM" option in the Recovery Services vault is the appropriate method for restoring a full virtual machine

- Drill VM Failover https://learn.microsoft.com/en-us/azure/site-recovery/azure-to-azure-tutorial-dr-drill#failover

- Azure Policy the deployIfNotExists effect ensures that any existing resources outside the allowed locations can be remediated

- Azure Logic Apps provide a flexible platform to automate workflows by interacting with various Azure services, including Azure Advisor through its REST API.
  How to create a logic app

- Public-facing load balancers: Most A Standard SKU Static Public IP is the most suitable choice (Static IP crucial)

- Cross region Load balancer: A Standard SKU Dynamic Public IP is well-suited for this scenario ()

- Load balancer with sticky sessions: Basic SKU Public IP - Load balancer with sticky sessions: For load balancers requiring sticky sessions, the Basic SKU Public IP is a cost-effective option. Sticky sessions (session persistence) ensure consistent routing of client requests to the same backend instance. https://learn.microsoft.com/en-us/azure/load-balancer/distribution-mode-concepts#session-persistence

- Loadbalancer Links: https://learn.microsoft.com/en-us/azure/load-balancer/load-balancer-overview#internal-load-balancer, https://learn.microsoft.com/en-us/azure/load-balancer/cross-region-overview#standard-sku

- Public IP Addresses: https://learn.microsoft.com/en-us/azure/virtual-network/ip-services/public-ip-addresses#sku

## Powershell Commands

Get-AzRoleDefinition - for creating a custom role based on an existing role
New-AzRoleDefinition - Commit a new role definition after adding some parts.

Save-AzResourceGroupDeploymentTemplate - e.g. Save-AzResourceGroupDeploymentTemplate -ResourceGroupName demoGroup -DeploymentName demoDeployment
Save-AzManagementGroupDeploymentTemplate - for deployments to management groups
Save-AzTenantDeploymentTemplate - for deployments to tenants
