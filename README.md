# What does the template do?


The ARM templates creates a resource group within Canada Central region, a virtual network with 2 subnets, a storage account, a log analytics workspace, an App Service Plan with dedicated tier, Private DNS linked to vnet, mutiple premium function apps with private endpoints, vnet integration and links to a private DNS for A records.

# How does the template work?


The template is scoped to subscription to create the resource group and rest of the resources are scoped to the resource group that gets created through nested templates that are scoped to the resource group.

# Prerequisites


To deploy the ARM template, you need following:

- Azure Subscription
- User deploying the template should be a contributor (or similar RBAC role) on the subscription

# Ways to deloy this template to your azure subscription


- Github Actions
- Azure DevOps Pipelines
- Any other CI/CD pipeline that you integrate with your git repository