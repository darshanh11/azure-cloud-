## Azure CLI and Automation

### Azure CLI

#### Explanation

Azure CLI is a command-line tool used to create, manage, and monitor Azure resources from a terminal.

It allows cloud engineers and administrators to perform Azure operations without depending completely on the Azure Portal.

Azure CLI can also be used inside scripts to automate repetitive cloud management tasks.

#### Example

```bash
az login
az account show
az group list
az resource list
```

The `az login` command signs in to Azure.

The `az account show` command displays information about the current Azure subscription.

The `az group list` command displays the Resource Groups available in the subscription.

The `az resource list` command displays Azure resources.

#### Steps to Use Azure CLI

1. Install Azure CLI or open Azure Cloud Shell.
2. Open the terminal.
3. Run `az login`.
4. Sign in with the Azure account.
5. Check the active subscription.
6. Run the required Azure CLI command.
7. Verify the command output.
8. Check the resource in the Azure Portal if required.

---

### Azure PowerShell

#### Explanation

Azure PowerShell is a collection of PowerShell commands, called cmdlets, used to manage Azure resources.

It provides a PowerShell-based way to create, configure, monitor, and remove Azure resources.

Azure PowerShell is useful for administrators and cloud engineers who use PowerShell for automation and system management.

#### Example

```powershell
Connect-AzAccount
Get-AzResourceGroup
Get-AzResource
```

The `Connect-AzAccount` command connects to an Azure account.

The `Get-AzResourceGroup` command displays Azure Resource Groups.

The `Get-AzResource` command displays Azure resources.

#### Steps to Use Azure PowerShell

1. Install the Az PowerShell module.
2. Open PowerShell.
3. Run `Connect-AzAccount`.
4. Sign in with the Azure account.
5. Select the required subscription.
6. Run the required Azure PowerShell cmdlets.
7. Verify the command output.
8. Check the resources in the Azure Portal if required.

---

### Resource Management

#### Explanation

Resource management is the process of creating, configuring, updating, monitoring, and deleting Azure resources.

Azure CLI and Azure PowerShell can be used to manage resources such as Resource Groups, Virtual Machines, Storage Accounts, Virtual Networks, and other Azure services.

Resource management helps cloud engineers maintain Azure infrastructure efficiently and consistently.

#### Example

```bash
az group create --name MyResourceGroup --location eastus
az group show --name MyResourceGroup
az resource list --resource-group MyResourceGroup
```

The first command creates a Resource Group.

The second command displays information about the Resource Group.

The third command lists the resources inside the Resource Group.

#### Steps for Resource Management

1. Sign in to Azure.
2. Select the required subscription.
3. Identify the resource that needs to be managed.
4. Create or select the required Resource Group.
5. Create the required Azure resource.
6. Configure the resource.
7. Update the resource when required.
8. Monitor the resource.
9. Delete the resource when it is no longer required.
10. Verify the resource status.

---

### Automation Basics

#### Explanation

Automation is the process of using scripts, commands, and tools to perform repetitive Azure management tasks automatically.

Instead of manually creating and configuring resources through the Azure Portal, cloud engineers can use Azure CLI or Azure PowerShell scripts.

Automation reduces manual effort, improves consistency, and helps manage multiple Azure resources efficiently.

#### Example

```bash
az group create --name MyResourceGroup --location eastus

az storage account create \
  --name mystorageaccount001 \
  --resource-group MyResourceGroup \
  --location eastus \
  --sku Standard_LRS
```

The first command creates a Resource Group.

The second command creates an Azure Storage Account inside that Resource Group.

These commands can be placed inside a script and executed automatically whenever the infrastructure needs to be created.

#### Steps for Azure Automation

1. Identify the task that needs to be automated.
2. Select Azure CLI or Azure PowerShell.
3. Write the required commands.
4. Store the commands in a script.
5. Test the script.
6. Correct any errors.
7. Execute the automation script.
8. Verify the Azure resources.
9. Modify the script when requirements change.
10. Reuse the script for future deployments.
