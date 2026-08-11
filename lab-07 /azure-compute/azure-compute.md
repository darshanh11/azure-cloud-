# Lab 07 – Azure Compute

## 1. Azure Virtual Machines

### Explanation
Azure Virtual Machines (VMs) are virtual computers running in Microsoft Azure. 
They provide compute resources such as CPU, memory, disk, and networking.
A VM can run operating systems such as Windows Server or Linux.

### Steps to Create an Azure Virtual Machine

1. Sign in to the Azure Portal.
2. Search for **Virtual Machines**.
3. Select **Create → Azure virtual machine**.
4. Select the required **Subscription**.ā
5. Select or create a **Resource Group**.
6. Enter the **Virtual Machine name**.
7. Select the required **Region**.
8. Select the required **Availability option**.
9. Select the required **Image**, such as Windows Server or Ubuntu.
10. Select the required **VM Size**.
11. Configure the **Administrator account**.
12. Configure the **Inbound ports**, such as RDP (3389) or SSH (22).
13. Configure the **Disks**.
14. Configure the **Networking** settings.
15. Review the configuration.
16. Select **Review + create**.
17. Select **Create**.

### Screenshot
![Azure Virtual Machine Creation](screenshots/01-create-vm.png)

---

## 2. VM Sizes

### Explanation
VM size determines the compute capacity of a virtual machine. 
It defines resources such as the number of virtual CPUs, memory, disk performance, 
and network performance. Different VM sizes are selected according to workload requirements.

### Steps to Select a VM Size

1. Open **Virtual Machines** in the Azure Portal.
2. Select **Create → Azure virtual machine**.
3. Go to the **Basics** tab.
4. Locate the **Size** option.
5. Select **See all sizes**.
6. Review the available VM sizes.
7. Compare CPU, memory, temporary storage, and pricing.
8. Select the required VM size.
9. Continue with the VM configuration.

### Screenshot
![VM Sizes](screenshots/02-vm-size.png)

---

## 3. VM Disks

### Explanation
Azure VMs use disks to store the operating system, applications, and data.
The main disk types associated with a VM are the OS disk and data disks.
Azure Managed Disks provide scalable and reliable storage for virtual machines.

### Steps to Configure VM Disks

1. Open **Virtual Machines**.
2. Select **Create → Azure virtual machine**.
3. Configure the basic VM settings.
4. Open the **Disks** tab.
5. Select the required **OS disk type**.
6. Select the required disk size.
7. Configure **Data disks** if additional storage is required.
8. Select **Create and attach a new disk** when required.
9. Review the disk configuration.
10. Continue to the next configuration step.

### Screenshot
![VM Disks](screenshots/03-vm-disks.png)

---

## 4. VM Images

### Explanation
A VM image is a template used to create a virtual machine.
Azure provides images for operating systems such as Windows Server, Ubuntu, 
Red Hat Enterprise Linux, and other supported distributions.

### Steps to Select a VM Image

1. Open **Virtual Machines**.
2. Select **Create → Azure virtual machine**.
3. Go to the **Basics** tab.
4. Locate the **Image** option.
5. Select the required operating system image.
6. Review the image details.
7. Select the required VM size.
8. Continue with the remaining VM configuration.

### Screenshot
![VM Image](screenshots/04-vm-image.png)

---

## 5. VM Availability Sets

### Explanation
An Availability Set is a logical grouping of virtual machines that helps protect 
applications from planned maintenance and hardware failures.
Azure distributes VMs across fault domains and update domains.

### Steps to Configure an Availability Set

1. Open **Virtual Machines**.
2. Select **Create → Azure virtual machine**.
3. Configure the basic VM settings.
4. Locate **Availability options**.
5. Select **Availability set**.
6. Select an existing availability set or create a new one.
7. Configure the remaining VM settings.
8. Review the configuration.
9. Select **Review + create**.
10. Select **Create**.

### Screenshot
![VM Availability Set](screenshots/05-availability-set.png)

---

## 6. VM Scale Sets

### Explanation
Azure Virtual Machine Scale Sets allow you to create and manage a group of 
identical virtual machines. They can automatically increase or decrease the 
number of VM instances according to workload requirements.

### Steps to Create a VM Scale Set

1. Sign in to the Azure Portal.
2. Search for **Virtual Machine Scale Sets**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Scale Set name**.
7. Select the required **Region**.
8. Select the required **Orchestration mode** if applicable.
9. Select the required **Image**.
10. Select the required **VM size**.
11. Configure the administrator account.
12. Configure networking.
13. Configure the instance count and scaling settings.
14. Review the configuration.
15. Select **Review + create**.
16. Select **Create**.

### Screenshot
![VM Scale Set](screenshots/06-vm-scale-set.png)

---

## 7. Azure App Service

### Explanation
Azure App Service is a fully managed platform for hosting web applications, 
REST APIs, and backend services. It supports several programming languages 
and provides features such as scaling, deployment, and monitoring.

### Steps to Create an App Service

1. Sign in to the Azure Portal.
2. Search for **App Services**.
3. Select **Create → Web App**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter a unique **App Service name**.
7. Select the required **Deployment** option.
8. Select the required **Runtime stack**.
9. Select the required **Operating System**.
10. Select the required **Region**.
11. Configure the **App Service Plan**.
12. Configure additional settings if required.
13. Review the configuration.
14. Select **Review + create**.
15. Select **Create**.

### Screenshot
![Azure App Service](screenshots/07-app-service.png)

---

## 8. Containers

### Explanation
Azure provides container services for running applications packaged as 
containers. Containers provide a lightweight and consistent environment for 
deploying applications.

### Steps to Create an Azure Container Instance

1. Sign in to the Azure Portal.
2. Search for **Container Instances**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Container name**.
7. Select the required **Region**.
8. Select the required container image source.
9. Enter the container image name.
10. Configure CPU and memory.
11. Configure networking and ports if required.
12. Review the configuration.
13. Select **Review + create**.
14. Select **Create**.

### Screenshot
![Azure Container Instance](screenshots/08-container.png)

---

## 9. Azure Functions

### Explanation
Azure Functions is a serverless compute service that allows you to run 
event-driven code without managing the underlying servers.
Functions can be triggered by HTTP requests, timers, queues, events, and other services.

### Steps to Create an Azure Function App

1. Sign in to the Azure Portal.
2. Search for **Function App**.
3. Select **Create → Function App**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Function App name**.
7. Select the required **Deployment** option.
8. Select the required **Runtime stack**.
9. Select the required **Region**.
10. Select the required hosting option.
11. Configure the storage account.
12. Configure monitoring if required.
13. Review the configuration.
14. Select **Review + create**.
15. Select **Create**.

### Screenshot
![Azure Functions](screenshots/09-azure-functions.png)
