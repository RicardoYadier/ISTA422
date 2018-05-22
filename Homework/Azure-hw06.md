## Ricardo Rosa

### ISTA422 Homework 6

### Azure



***Read chapter 6, pages 157 – 180 in the Fundamentals of Azure, 2nd Edition book.***

#### 1. What is the target of Azure SQL Databases.
Azure SQL Database provides a relational database as a service, targeted at online transaction processing (OLTP; that is, data entry and retrieval transactions) workloads.

#### 2. By default, how many logical SQL Database servers can you have per Azure subscription?
You can have up to six logical SQL Database servers per Azure subscription.

#### 3. Why does the connection string set the TrustServerCertificate property to False and the Encrypt property to True?
To provide additional protection while accessing SQL Database over the Internet. Doing so helps thwart potential man-in the-middle attacks.

#### 4. What are transient errors?
are errors that are intermittent and likely will be resolved if the command is retried.

#### 5. What three things contribute to the total cost for running a SQL Server deployment on Azure Virtual Machines?
First is the cost of the Windows VM itself.

Second is the SQL Server license cost.

Finally, you’ll also pay for the Azure Storage cost.

#### 6. Why do you need to be concerned about high availability and disaster recovery for SQL Server in Azure Virtual Machines?
Azure provides high-availability features for the VMs, but not necessarily for SQL Server running on the VM. It is possible for the VM to be online but the SQL Server instance to be offline, unhealthy, or both. Additionally, it is possible for the VM to unavailable due to hardware failure or software upgrades.

#### 7. What are six SQL Server features that are not currently supported in SQL Database (according to the book)?
- Windows authentication.

- FILESTREAM data.

- Database mirroring.

- Extended stored procedures.

- SQL Server Agent/Jobs.

- SQL Server Reporting Services (SSRS) and SQL Server Integration Services (SSIS) are not supported. Alternatively, run a SQL Server on-premises or in an Azure VM and connect to a SQL database.

#### 8. Name four factors to consider when choosing between SQL Database and SQL Server in Azure Virtual Machines.
Database size, existing application versus new application, level of administrative control (including hardware infrastructure), business continuity strategy, and hybrid scenarios,

#### 9. Who did Microsoft collaborate with to bring their ClearDb database as a service for MySQL to the Azure platform?
SuccessBrick

#### 10. What two options exist in Azure if you don't need a relational database management system (RDBMS) based data storage solution such as SQL Database or SQL Server in Azure Virtual Machines?
DocumentDB and Azure Table storage.