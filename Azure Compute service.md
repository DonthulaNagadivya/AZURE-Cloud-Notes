**What is Azure Compute**

Azure Compute is a cloud service that provides processing power, memory, and networking resources to run applications using services like Azure VMs, App Services, and Functions. or 

Azure Compute Services provide on-demand computing resources like Virtual Machines, containers, functions, and App Services. These services allow you to run applications and services in the cloud with flexibility in resource allocation and scaling.





**What are the different types of compute services available in Azure.**



The different compute services in Azure include Virtual Machines (VMs) for IaaS, App Services for hosting web apps (PaaS), Azure Functions for serverless computing, and Azure Container Instances and Kubernetes for containerized workloads.



**What is the difference between Azure App Service and Azure Virtual Machine**



Azure App Service is a PaaS offering to deploy and run applications without managing infrastructure. Azure Virtual Machine is an IaaS offering that gives full control over the OS, CPU, memory, and storage for hosting apps in the cloud.



**What is the difference between Azure App Services and Azure Functions**



Azure app service is a PAAS offering for deploying and running web applications, with azure managing the underlying infrastructure.

Azure functions is a serverless computing service, where code runs only in response to events and resources are allocated automatically based on demand.





**What is the difference between Availability Set and VM Scale Set?**



**Availability Set**: Protects against datacenter failure by distributing VMs across fault and update domains.



**VM Scale Set**: Automatically scales VM instances based on demand and integrates with load balancer for high availability. 




**What are Availability Zones in Azure and how are they different from Availability Sets**



**Availability Zones** protect workloads from datacenter-level failures by distributing VMs across physically separate zones within a region. Unlike Availability Sets (which protect against rack-level failures), Zones ensure high availability even if an entire datacenter goes down.


**What are VM sizes in Azure?**

&nbsp;		

VM sizes define compute resources like CPU, RAM, and disk. Categories include:



B-Series: Burst workloads (low-cost, test environments)

Use When: Low CPU most of the time, occasional spikes

Example: Dev/test servers, internal apps



D-Series (General Purpose)

Use When: Balanced CPU and memory needs

Example: Web servers, small to medium applications



E-Series (Memory Optimized)

Use When: High memory is needed

Example: Databases like SQL Server, SAP



F-Series (Compute Optimized)

Use When: High CPU is needed, less memory

Example: Batch jobs, gaming servers, compute-heavy tasks



L-Series (Storage Optimized)

Use When: Fast disk speed and high IOPS needed

Example: Big data apps, NoSQL DBs like MongoDB or Cassandra





