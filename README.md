# Cost Optimization And Monitoring On Microsoft Azure Project

## Project Summary
You have been invited to a meeting with the CEO of your engineering company, Company "X", which has offices in both the US East Coast and US West Coast. They currently host all their data and applications in a single East Coast data center and are constantly worried about both cost and resiliency.

## Project Statement
Company "X" currently hosts all their data and applications in a single East Coast data center and are constantly worried about both cost and resiliency. Below is how their current servers are configured.

### Server(s):
* Purpose: Windows/Linux Server
* Environment: Physical Servers
* Operating System: Windows
* Operating System License: DataCenter
* Servers: 10
* Procs per server: 2
* Core(s) per proc: 8 Cores
* RAM: 256 GB
* Optimize By: CPU
* GPU: None
* Usage: These are the servers where all your engineering workloads happen. Currently they all are being leveraged at regular capacity.

### Server(s):
* Purpose: Web App
* Type: Physical Machines
* Operating System: Windows
* Operating System License: Data Center
* Servers: 3
* Procs per server: 1
* Core(s) per proc: 8 Cores
* RAM: 64 GB
* Optimized By: CPU
* GPU: None
* Usage: These are the web app servers for your company. Currently, they all are being leveraged at regular capacity.

## Server(s):
* **Source**: Database Server
	- Database: Microsoft SQL Server
	- License: Enterprise
	- Environment: Physical  Servers
	- Operating System: Windows
	- Operating System License: Datacenter
	- Servers: 3
	- Procs per server: 1
	- Cores per proc: 16 Cores
	- RAM: 64 GB
	- Optimized By: CPU
	- Usage: These three servers are running Microsoft SQL Server and provide the database for your engineering company. It is critical that they are always running.

* **Destination**:
	- Service: SQL Database
	- Purchase Model: vCore
	- Service Tier: Business Critical
	- Instance Cores: 2
	- SQL Server Storage: 5
	- SQL Server backup: 0

### Storage:
* Purpose: Storage
* Type: Local Disk / SAN
* Disk Type: HDD
* Capacity: 1 TB
* Back-Up: None, currently
* Archive: None

### Networking:
* Amount of network bandwidth you currently consume in your on-premises environment: 1 GB
