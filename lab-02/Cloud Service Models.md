# Cloud Service Models

Cloud service models describe how cloud computing resources and services are provided to users.

There are three main cloud service models:

1. IaaS – Infrastructure as a Service
2. PaaS – Platform as a Service
3. SaaS – Software as a Service

---

## 1. IaaS – Infrastructure as a Service

IaaS provides virtualized infrastructure resources over the internet. These resources include virtual machines, storage, networking, and other computing resources.

With IaaS, the cloud provider manages the physical data center, physical servers, networking hardware, and virtualization infrastructure. The customer is responsible for managing the operating system, applications, data, and configurations running on the resources.

### Examples

- Azure Virtual Machines
- Amazon EC2
- Google Compute Engine
- Azure Virtual Network
- Azure Storage

### Advantages

- Flexible infrastructure
- Easy to scale resources
- No need to purchase physical servers
- Pay for the resources used
- Provides greater control over operating systems and applications

### Example

A company needs a Windows Server but does not want to purchase a physical server.

The company can create an **Azure Virtual Machine** and install/configure Windows Server on it.

---

## 2. PaaS – Platform as a Service

PaaS provides a ready-to-use platform for developing, deploying, and managing applications.

The cloud provider manages the underlying infrastructure, operating system, runtime environment, and platform components. Developers can focus mainly on application code and data instead of managing servers and operating systems.

### Examples

- Azure App Service
- Azure Functions
- AWS Elastic Beanstalk
- Google App Engine

### Advantages

- Faster application development
- No need to manage physical servers
- Reduced infrastructure management
- Easy application deployment
- Automatic scaling options
- Developers can focus on writing application code

### Example

A developer wants to deploy a Python web application.

Instead of creating a virtual machine and manually installing the operating system, web server, and runtime, the developer can use **Azure App Service** to deploy the application.

---

## 3. SaaS – Software as a Service

SaaS provides complete software applications over the internet.

The cloud provider manages the infrastructure, operating system, application, updates, and maintenance. Users normally access the software through a web browser or application.

### Examples

- Microsoft 365
- Outlook
- Microsoft Teams
- Google Workspace
- Salesforce

### Advantages

- No installation or infrastructure management
- Accessible through the internet
- Automatic software updates
- Easy to use
- Usually subscription or usage based
- Can be accessed from different devices

### Example

Instead of installing and maintaining email software on your own server, an organization can use **Microsoft 365 Outlook** through the internet.

---

# IaaS vs PaaS vs SaaS

| Feature | IaaS | PaaS | SaaS |
|---|---|---|---|
| Infrastructure | Provider | Provider | Provider |
| Operating System | Customer | Provider | Provider |
| Runtime | Customer | Provider | Provider |
| Application | Customer | Customer | Provider |
| Data | Customer | Customer | Customer |
| Management | More customer responsibility | Shared | Mostly provider |
| Main Users | System administrators | Developers | End users |

---

# Shared Responsibility Model

In cloud computing, responsibility is shared between the cloud provider and the customer.

The cloud provider is generally responsible for the **security of the cloud**, including physical data centers, physical hardware, and core infrastructure.

The customer is responsible for the **security of what they put in the cloud**, such as data, identities, configurations, and access permissions. The exact responsibilities depend on the service model.

### IaaS

Customer has more responsibility.

Example:

**Azure VM → Customer manages OS, applications, data, and configuration.**

### PaaS

The cloud provider manages more of the underlying platform.

Example:

**Azure App Service → Provider manages infrastructure and platform; customer focuses mainly on application and data.**

### SaaS

The provider manages almost the entire application stack.

Example:

**Microsoft 365 → Provider manages the application and underlying infrastructure; customer manages users, access, and their data/configuration.**


