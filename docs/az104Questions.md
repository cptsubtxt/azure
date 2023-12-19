# AZ 104 Questions and their answer

- A loadbalancer from basic sku can loadbalance between machines only when the vms are in the same availability set or virtual machine scale set (https://learn.microsoft.com/en-us/azure/load-balancer/skus#skus)

- Azure does not allow to scale Azure Container Instances. One has to delete the ACI and reapply the ARM Template with new settings for CPU and Memory. (https://docs.microsoft.com/en-us/azure/container-instances/container-instances-update#properties-that-require-container-delete)

- Inbound NAT rule are used to forward traffic from a specific port of a front end IP address to specific port of a back-end VM.

- Review process of creating and managing an Azure container registry (Create Container Registry, Select Pricing Tier, Configure Container Registry Settings, Set up authentication and security, Access and manage container images)

- Geo redundant Storage, review https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy#geo-redundant-storage

- Move VMs to a different resource group, subscription and region (https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/move-limitations/virtual-machines-move-limitations?tabs=azure-cli)

- Review Administrative Unit Management (https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/administrative-units#administrative-unit-management)

- You can also send security events of virtual machines to Log Analytics workspace.

-
