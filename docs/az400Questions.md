# AZ 400 Questions

- Blue Green Deployment with Loadbalancing methods --> with weighted round-robin as the routing method and add the endpoints corresponding to these environments. [Blue Green Deployment Azure Traffic Manager](https://azure.microsoft.com/de-de/blog/blue-green-deployments-using-azure-traffic-manager/)

- When packages have to be installed the Feed permission is important: Reader can list, read and install packages (https://learn.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops#feed-permissions-overview)

- Add secret to keyvault, command: az keyvault secret set --vault-name "<your-unique-keyvault-name>" --name "ExamplePassword" --value "hVFkk965BuUv"

- DACPACs can be used to package and deploy schema changes and data. Used in Pipelines for changing databases.

- With RBAC you can set permission for Key vaults to delete them etc.

- Pre deployment Gates are used to make sure that no active work items or problems exist before a build step is done (https://learn.microsoft.com/en-us/azure/devops/pipelines/release/approvals/?view=azure-devops&tabs=yaml)

- Query Permissions in Azure Devops (https://learn.microsoft.com/en-us/azure/devops/boards/queries/set-query-permissions?view=azure-devops#default-query-permissions)

- Platform Log Facilities: https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/platform-logs-overview

- Connect Azure DevOps to Github, ADO --> Project Settings --> Permissions.
  (https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops), (https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository#collaborator-access-on-a-repository-owned-by-a-user-account)

- Process model templates (https://learn.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=agile-process)

- Desired State Configuration (https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview)
