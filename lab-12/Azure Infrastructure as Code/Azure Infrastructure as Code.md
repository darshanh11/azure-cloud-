# Azure Infrastructure as Code

## ARM Templates

### Explanation

Azure Resource Manager (ARM) templates are JSON files used to define and deploy Azure resources in a declarative way.

An ARM template describes the resources, properties, dependencies, and configuration required for an Azure environment. It allows infrastructure to be deployed repeatedly with consistent configurations.

### Steps to Deploy Using an ARM Template

1. Sign in to the Azure Portal.
2. Search for **Deploy a custom template**.
3. Select **Build your own template in the editor**.
4. Enter or paste the ARM template JSON.
5. Select **Save**.
6. Select the required **Subscription**.
7. Select or create a **Resource Group**.
8. Configure the required parameters.
9. Select **Review + create**.
10. Select **Create**.

### Screenshot

![ARM Template Deployment](../screenshot/image-01.png)

---

## Bicep

### Explanation

Bicep is a domain-specific language used to define and deploy Azure resources. It provides a simpler and more readable syntax than JSON-based ARM templates.

Bicep files normally use the `.bicep` extension and are compiled into ARM deployment representations when deployed to Azure.

### Steps to Deploy Using Bicep

1. Install **Azure CLI** or use **Azure Cloud Shell**.
2. Sign in to Azure using `az login`.
3. Create a file with the `.bicep` extension.
4. Define the required Azure resources.
5. Save the Bicep file.
6. Validate the Bicep file.
7. Create or select the required Resource Group.
8. Deploy the Bicep template.
9. Verify the deployed resources in the Azure Portal.

### Screenshot

![Azure Bicep Deployment](../screenshot/image-02.png)

---

## ARM Templates vs Bicep

### Explanation

ARM Templates and Bicep are both used for declarative Azure infrastructure deployment.

ARM Templates use JSON syntax, which can become lengthy and difficult to maintain for large deployments. Bicep provides a cleaner and more concise syntax specifically designed for Azure infrastructure.

Bicep is transpiled to ARM-compatible deployment representations, so it can deploy Azure resources using the Azure Resource Manager platform.

### Comparison

| Feature | ARM Templates | Bicep |
|---|---|---|
| Syntax | JSON | Bicep |
| Readability | More verbose | More concise |
| File Extension | `.json` | `.bicep` |
| Azure Focus | Azure Resource Manager | Azure Resource Manager |
| Reusability | Parameters, variables, modules | Parameters, variables, modules |
| Maintenance | Can be complex | Generally easier |
| Deployment | Native ARM deployment | Compiled/deployed through ARM |

---

## Terraform

### Explanation

Terraform is an Infrastructure as Code tool used to define and provision infrastructure using configuration files.

Terraform uses HashiCorp Configuration Language (HCL) and can manage resources across Azure and other cloud platforms.

For Azure, Terraform commonly uses the **AzureRM provider** to create and manage Azure resources.

### Steps to Deploy Azure Resources Using Terraform

1. Install **Terraform**.
2. Install or configure the **Azure CLI**.
3. Sign in to Azure using the Azure CLI.
4. Create a working directory for the Terraform configuration.
5. Create a `main.tf` file.
6. Define the Azure provider.
7. Define the required Azure resources.
8. Define variables if required.
9. Run `terraform init`.
10. Run `terraform validate`.
11. Run `terraform plan`.
12. Review the planned changes.
13. Run `terraform apply`.
14. Confirm the deployment.
15. Verify the resources in the Azure Portal.

### Screenshot

![Terraform Azure Deployment](../screenshot/image-03.png)

---

## Parameters

### Explanation

Parameters allow values to be supplied to an infrastructure deployment instead of hard-coding them in the template.

Parameters can be used for values such as resource names, locations, VM sizes, address spaces, and environment-specific settings.

This makes the same infrastructure definition reusable across different environments.

### Example

```bicep
param location string = resourceGroup().location
param storageAccountName string
```

## Variables

### Explanation

Variables are reusable values defined inside an Infrastructure as Code configuration.

They are used to store values that may be used multiple times in the code, such as environment names, resource names, locations, IP address ranges, or other configuration values.

Using variables reduces repetition and makes the Infrastructure as Code file easier to read, maintain, and modify.

### Example

```bicep
param environment string = 'dev'

var storageAccountName = 'storage${environment}001'
var locationName = resourceGroup().location
```
## Resources

### Explanation

Resources are the actual Azure services that are created and managed using Infrastructure as Code.

Examples of Azure resources include Virtual Machines, Storage Accounts, Virtual Networks, Subnets, Public IP Addresses, Network Security Groups, and App Services.

In Bicep, a resource block defines the type of Azure service, its name, location, and required configuration properties. Resources can also use parameters and variables to make the configuration reusable.

### Example

```bicep
param location string = resourceGroup().location
param storageAccountName string = 'mystorageaccount001'

resource storageAccount 'Microsoft.Storage/storageAccounts@2023-05-01' = {
  name: storageAccountName
  location: location
  sku: {
    name: 'Standard_LRS'
  }
  kind: 'StorageV2'
}
```
## Deployments

### Explanation

Deployment is the process of applying an Infrastructure as Code configuration to Azure to create or update resources.

During a deployment, Azure reads the configuration and creates or modifies the resources defined in the template. Deployments can be performed using ARM Templates, Bicep, Azure CLI, Azure PowerShell, or Terraform.

Before deployment, the configuration should be validated and the planned changes should be reviewed to reduce configuration errors.

### Example

```bash
az deployment group create \
  --resource-group myResourceGroup \
  --template-file main.bicep \
  --parameters environment=dev
```
