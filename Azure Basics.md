Azure Basics


1.Azure is Microsoft’s cloud computing platform that provides a wide range of services including Virtual Machines, Databases, Networking, Storage, and AI. It supports IaaS (Infrastructure as a Service), PaaS (Platform as a Service), and SaaS (Software as a Service). Azure allows organizations to build, deploy, and manage applications globally using Microsoft-managed data centers.



**2.Public Cloud**: Services offered over the internet (e.g., Microsoft Azure, AWS). Shared infrastructure.

Example: Hosting a blog or website on Azure Web App.



**Private Cloud:** Cloud environment dedicated to a single organization, often hosted on-premises.

Example: A financial firm running its secure infrastructure on VMware.



**Hybrid Cloud**: Combines public and private clouds, allowing data and applications to move between them.

Example: An enterprise running its internal ERP on-prem and connecting it with Azure for backup or DR.


3\. **Azure Region**

A region is a set of data centers deployed within a specific geographic area, such as East US, West Europe, or Central India. Each region offers redundancy and availability features. When you deploy resources, you select a region to place them physically closer to your users for better performance.


4. **Subscription**

An Azure subscription is a logical container used to provision resources in Azure. It is tied to an Azure account and used for billing, access control, and service limits. For example, a company may use separate subscriptions for Dev, Test, and Production environments for better cost tracking and isolation.


5.Resource Group (RG)

A Resource Group is a logical container that holds related Azure resources such as virtual machines, storage accounts, and databases. It helps organize resources and manage them as a single entity. You can apply RBAC (Role-Based Access Control) and tags at the RG level for governance.

6. ARM (Azure Resource Manager)

Azure Resource Manager is the deployment and management service for Azure. It provides a consistent management layer to create, update, and delete resources using templates (ARM templates), REST APIs, CLI, or Portal. It also supports role-based access and resource locking.





7.Availability Sets

An Availability Set is a logical grouping that ensures that the VMs you place within it are distributed across multiple physical servers in a data center. It provides high availability by distributing VMs across fault and update domains. This ensures that at least one VM remains available during planned or unplanned maintenance.



Fault and Update Domains

Fault Domain (FD): Represents a group of VMs that share the same physical rack, power source, and network.



Update Domain (UD): Represents a group of VMs that get updated/rebooted together during maintenance.

By placing VMs across multiple FDs and UDs, you minimize the risk of simultaneous downtime.




8\. Availability Zones

Availability Zones are physically separate data centers within an Azure region. Each zone has independent power, cooling, and networking to ensure high availability. Deploying your services across multiple zones helps protect against datacenter-level failures.




9\. Virtual Machine Scale Sets (VMSS)

VMSS lets you deploy and manage a group of identical, load-balanced VMs. They can automatically increase or decrease based on demand or a schedule. For example, a company running a retail website during a sale can use VMSS to auto-scale during traffic spikes.
✅ Vertical Scaling (Scale Up/Down)

Definition: Increasing or decreasing the capacity (CPU, RAM, storage) of a single VM or resource.

Use Case: When a database server needs more memory or processing power during peak hours.



✅ Horizontal Scaling (Scale Out/In)

Definition: Adding or removing multiple instances of a resource (like VMs) to handle more or less load.

Use Case: A web app that adds more VMs during heavy user traffic and reduces them afterward.

Aspect	         Vertical Scaling	         Horizontal Scaling

What it does	Increase size of 1 resource	Add more instances

Azure Example	Resize VM (e.g., B2s → D4s)	Use VM Scale Sets, Load Balancer

Cost Impact	May get expensive quickly	Can be more cost-efficient

Downtime Risk	Possible reboot	                No downtime






