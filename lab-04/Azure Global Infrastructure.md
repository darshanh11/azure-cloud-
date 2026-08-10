# Azure Global Infrastructure

Azure Global Infrastructure is the worldwide infrastructure used by Microsoft Azure to provide cloud services with scalability, reliability, security, and high availability.

Azure infrastructure includes regions, region pairs, availability zones, geographies, datacenters, resource groups, subscriptions, and management groups.

---

## 1. Azure Regions

An Azure Region is a geographical area that contains one or more Azure datacenters connected through a dedicated, high-speed network.

When creating an Azure resource, users normally select a region where the resource will be deployed.

### Examples

- Central India
- South India
- East US
- West Europe
- Southeast Asia

### Advantages

- Choose a location close to users
- Helps reduce network latency
- Supports regulatory and data residency requirements
- Provides access to Azure services available in that region
- Helps design highly available applications

### Example

If most users of an application are located in India, an organization may deploy its Azure resources in an Indian Azure region to reduce latency.

---

## 2. Azure Region Pairs

Azure region pairs are geographically separated regions within the same geography that are paired by Microsoft.

Region pairs help organizations design solutions for business continuity, disaster recovery, and resilience.

### Benefits

- Helps support disaster recovery
- Provides geographical separation
- Helps protect applications from regional failures
- Supports resilient application architectures
- Can help with planned Azure platform updates

### Example

An organization can deploy its primary workload in one Azure region and maintain a disaster recovery workload in another suitable region.

---

## 3. Availability Zones

Availability Zones are physically separate locations within an Azure region.

Each availability zone has independent power, cooling, and networking infrastructure.

Applications can be deployed across multiple availability zones to improve availability and resilience.

### Benefits

- Protects against datacenter-level failures
- Improves application availability
- Provides redundancy
- Supports highly available architectures

### Example

An application can have virtual machines deployed across three availability zones.

If one zone experiences a failure, workloads in the other zones can continue operating.

---

## 4. Azure Geographies

An Azure geography is a defined area of the world that contains one or more Azure regions.

Azure geographies help organizations meet requirements related to data residency, compliance, and data sovereignty.

### Examples

- India
- United States
- Europe
- Asia Pacific

### Benefits

- Helps meet data residency requirements
- Supports compliance requirements
- Provides geographical boundaries for Azure services
- Helps organizations plan where data and workloads are stored

### Example

An organization with data residency requirements in India can select Azure services and regions that support those requirements.

---

## 5. Azure Datacenters

An Azure datacenter is a physical facility containing servers, networking equipment, storage systems, power systems, cooling systems, and other infrastructure used to provide cloud services.

Microsoft operates datacenters around the world to support Azure services.

### Components

- Physical servers
- Networking equipment
- Storage systems
- Power infrastructure
- Cooling systems
- Security systems

### Benefits

- Provides the physical infrastructure for Azure services
- Supports scalability
- Provides redundancy
- Supports high availability
- Enables cloud services to run globally

### Example

When an Azure Virtual Machine is created, it runs on Microsoft's physical infrastructure within an Azure datacenter.

---

## 6. Azure Resource Groups

A Resource Group is a logical container used to organize and manage related Azure resources.

Resources such as virtual machines, virtual networks, storage accounts, and other services can be placed in a resource group.

### Benefits

- Organizes related resources
- Simplifies resource management
- Helps manage access using Azure RBAC
- Makes it easier to monitor and manage resources
- Resources can be managed as a group

### Example

A web application can have the following resources in one resource group:

- Azure Virtual Machine
- Virtual Network
- Network Security Group
- Storage Account

---

## 7. Azure Subscriptions

An Azure Subscription is a logical boundary used to organize Azure resources, manage access, and track usage and billing.

Resources are created within an Azure subscription.

A subscription can contain multiple resource groups and resources.

### Benefits

- Tracks Azure usage and costs
- Provides an access boundary
- Helps organize resources
- Supports governance and policies
- Allows organizations to separate workloads

### Example

A company can have separate subscriptions for:

- Development
- Testing
- Production

This helps separate workloads, access, and costs.

---

## 8. Management Groups

Management Groups provide a level of management above Azure subscriptions.

They allow organizations to organize multiple Azure subscriptions into a hierarchy and apply governance consistently across those subscriptions.

### Hierarchy

The Azure management hierarchy can be represented as:

Management Group
↓
Subscriptions
↓
Resource Groups
↓
Resources

### Benefits

- Manage multiple subscriptions
- Apply Azure policies at a higher level
- Organize subscriptions
- Improve governance
- Control access across multiple subscriptions

### Example

A large organization can create a management group called `Production` and place multiple production subscriptions under it.

Policies and governance settings can then be applied at the management group level.

---

# Azure Global Infrastructure Hierarchy

The physical and management concepts should be understood separately.

### Physical Infrastructure

Geography
→ Region
→ Availability Zones
→ Datacenters

### Resource Management Hierarchy

Management Group
→ Subscription
→ Resource Group
→ Resources

---

# Azure Global Infrastructure Summary

| Component | Purpose |
|---|---|
| Azure Region | Geographical location containing Azure datacenters |
| Region Pair | Paired regions used to support resilience and disaster recovery |
| Availability Zone | Physically separate location within an Azure region |
| Azure Geography | Geographical boundary containing one or more regions |
| Azure Datacenter | Physical facility hosting Azure infrastructure |
| Resource Group | Logical container for related Azure resources |
| Subscription | Boundary for resources, access, usage, and billing |
| Management Group | Organizes and governs multiple Azure subscriptions |

---

# Example Azure Structure

A company can organize its Azure environment like this:

Management Group
- Production Subscription
  - Web Application Resource Group
    - Virtual Machine
    - Virtual Network
    - Storage Account
  - Database Resource Group
    - Azure Database

- Development Subscription
  - Development Resource Group
    - Virtual Machine
    - Virtual Network
    - Storage Account
