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
