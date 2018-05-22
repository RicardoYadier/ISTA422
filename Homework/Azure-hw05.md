## Ricardo Rosa

### ISTA422 Homework 5

### Azure




***Read chapter 5, pages 133 – 156 in the Fundamentals of Azure, 2nd Edition book.***

#### 1. What is a VNET and what is it used for in Azure?
Virtual Network - are used in Azure to provide private connectivity for Azure Virtual Machines (Azure VMs) and some Azure services.

#### 2. The fully managed service in Azure that is used for cross-premises connectivity, is called what?
A Virtual Network Gateway

#### 3. List three things you need to know when setting up a virtual network.
The address space, subnets, and DNS servers that you want to use.

#### 4. What is the primary purpose of establishing a subnet
To break up your network into more manageable sections.

#### 5. When in the deployment process of multiple Virtual Machines(VMs) are the VMs assigned their IP address?
VMs are assigned an IP address when they are deployed.

#### 6. Why should you set the location of the Resource Group?
it’s best to specify the same Azure region that will be used for the resources when they are created.

#### 7. What are the four rules to editing a template to redeploy?
- If you remove a resource from the template that is not in the resource group, that resource will be unchanged. It won’t be removed simply because it’s gone from the template. (If you want to remove a resource, you have to specifically remove it using the Azure portal, PowerShell, the Azure CLI, etc.)


- If you add a resource to the template that is not in the resource group, it will create that resource for you when you redeploy the template.

- Resources that are unchanged but are still in the template will be ignored.

- Resources that are changed and still in the template will be updated. For example, if we change the address prefixes of our virtual network and redeploy the template, it will change them in the deployed VNet.

#### 8. Why should you not request a complete deployment using PowerShell?
Deletes resources that are in the resource group but not in the template when you redeploy.

#### 9. Why did Microsoft create NSGs?
To provide a flexible method for defining the access rules allowing traffic into and out of a VM in a VNet—or even an entire subnet in the VNet.

#### 10. What is a VPN according to the book?
A VPN gateway is a specific type of virtual network gateway that is used to send encrypted traffic between an Azure virtual network and an on-premises location over the public Internet.
