## Ricardo Rosa

### ISTA422 Homework 3

### Azure


***Read chapter 3, pages 70 – 100 in the Fundamentals of Azure***

#### 1. What is Azure Virtual Machines and the terminology used in the chapter to reference?
Azure Virtual Machines supports the deployment of Windows or Linux virtual machines (VMs) in a Microsoft Azure datacenter.

Azure Virtual Machines will refer to the feature.

While virtual machine or VM will refer to an instance of an actual compute node.

#### 2. How do you stop an Azure VM, and give an example?
To stop a VM but keep it provisioned, you would need to use the Stop-AzureRmVM PowerShell

Stop-AzureRmVM -Name "AzEssentialDev3" -ResourceGroup "AzureEssentials" -StayProvisioned

#### 3. What are three main resource providers used when working with Azure Vitrual Machines, Storage, and Compute?
Network, Storage, and Compute.

The Network resource provider (Microsoft.Network) handles all aspects of network connectivity such as IP addresses, load balancers, NICs, and so on

The Storage resource provider (Microsoft.Storage) handles the storage of the disks for a VM (in the context of Azure Virtual Machines).

The Compute resource provider (Microsoft.Compute) handles details related to the VM itself, such as naming, operating system details, and configuration (size, number of disks, and so on).

#### 4. Where are durable disks stored and what are the benefits?
an OS disk and a data disk

All durable disks (the OS disk and data disks) are backed by page blobs in Azure Storage. Therefore, the disks inherit the benefits of blob storage: high availability, durability, and geo-redundancy options.

#### 5. What is required when creating a VM in Azure using the Resource Manager model?
It is required that the VM be placed within an Azure Virtual Network (VNET).


#### 6. What is a NIC and what does it do for Azure?
Network interface card

provides network access to resources in an Azure virtual network.

#### 7. Why should you deploy at least two instances of the VM? What is provided?
To avoid a single point of failure.

Azure provides an SLA only when two or more VMs are deployed into an availability set. (a logical  feature)

#### 8. How many ways can you connect to your VM, and what are they?
Two

Remotely access a virtual machine

Configuring Network Access

#### 9. Who’s responsibility is it to manage the VM?
The overall management of the VMs is largely the user’s responsibility

#### 10. What is important when determining the scale-out approach to VMs, and what model is this referred to?Classic Modelit is important to determine the maximum number of VMs