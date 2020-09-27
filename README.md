# Oracle-1Z0-1072-20                     <p>       </p>              <img src="/images/logo2.JPG" alt="logo2.JPG" style="zoom:50%;" />

## Comprehensive cheat sheet to pass Oracle 1Z0-1072-20 Exam

------

#### Terminate a compute instance:
- Users can preserve the boot volume associated with the instance


#### Terraform use to create, manage, and manipulate infrastructure resources:
- provider


#### Does NOT set a variable in Terraform:
- Setting the variable as key value pairs in a file in a subdirectory named tfvar


#### Language are Terraform and Terraform providers written:
- Go

#### Provide users access to an existing compartment:
- Add users in group, define policy to provide group access to the compartment

#### Scale out the application, stretching from on-premises to the cloud by using a common API:
- Oracle Cloud Infrastructure
- Oracle Cloud at Customer

#### Available by default when your OCI tenancy is provisioned:
- A set of images, where each image is a template of a virtual hard drive that consists of the OS and installed software and applications
- A variety of shapes, where each shape determines the number of CPUs and memory allocated to an instance

#### Minimize infrastructure costs to test application functionality including a hardware failure scenario:
- Two node real application cluster(RAC)


#### Reside in single AD:
- Compute Instance + Block Volume


#### Regional resource:
- Compartment + Dynamic Group


#### Two Resource can not be deleted in VCN:
- Default security list + Default Routing Table


#### Modes can be used to launch imported Linux VMs:
- Emulated
- Paravirtualized

#### CPU scaling for seasonal peak:
- Bare metal DB systems


#### Retain the public IP after instance reboot:
- Create a Reserved Public IP and associate it with the VNIC of your compute instance


#### Make instances resistant to hardware failure:
- Design your system with redundant compute modes in different Availability Domains to support the failover capability
- Create a custom image of your system drive each time you change the image

#### OCI Object Storage:
- It provides strong consistency
- Data is stored redundantly across multiple availability domains(ADs) in a multi-AD region.

#### File Storage Service:
- You can access multiple file systems through a single mount target.
- Security list can be used as a virtual firewall to prevent an instance from mounting an FSS mount target within the same subnet
- FSS leverages UNIX user group and permission checking for file access security.
- Mount targets use Oracle-managed keys by default
- Customer can encrypt data in their file system using their own vault encryption key

#### Unable to access the shared file system:
- There are no security list rules for mount target traffic.


#### Random reads and writes across the dataset:
- Block Volume


#### Cloning a block volume:
- A cloned volume is the same as a snapshot that has a dependency on the source volume
- You can change the block volume performance when creating a clone
- You can change the block volume size when creating a clone.

#### Block Volume Backup:
- You can restore a volume to any AD within the same region where the backup is stored.
- You can restore a block volume backup to a larger volume size

#### File Storage vs Object Storage & Block Volume:
- File Storage use NFS protocol but block volume use ISCSI
- You can move object storage buckets, block volumes and file storage mount target between compartment
- A file system is created within an availability domain, whereas object storage buckets exist at the region level

#### Replica set in OKE:
- It exposes an application running on a set of Pods


#### Encryption:
- By default object storage and block storage are encrypted at rest.
- By default DB systems offer an encrypted database.
- Customer provided encryption keys are always stored in OCI vault service.



------



#### Key Benefit of Database as a Service on Oracle Cloud Infrastructure:
- Automatic Backup


#### Migrate DB to OCI:
- On-premises database version and quantity of data, including indexes.
- On-premises host operating system platform and network bandwidth
- Snapping or cloning storage form on-premise to Oracle Cloud Infrastructure
- Performing RMAN backup to an on-premise storage device, and then shipping to Oracle Cloud Infrastructure

#### DB System in OCI:
- The database and backups are encrypted by default.
- Customer can manage the TDE wallet after DB systems are provisioned.

#### Features are offered natively on Oracle Cloud Infrastructure Database Cloud Service (DBCS):
- Data Guard in Async mode within a region.
- Backup to Object Storage

#### Determine the cause of DB Backup failure:
- Ensure that your database host can connect to the OCI object storage.
- Restart the dscagent program if it has a status of stop or waiting

#### Cross-region database backups copy feature:
- Specify an existing destination bucket.
- Write an IAM policy and authorize the object storage service to manage objects on your behalf.
  Choose an overwrite rule.

#### Scaling option Database Cloud Service (DBCS) on Bare Metal Shape offer:
- CPU


#### Business need to use Database Cloud Service (DBCS) instead of Oracle database on a compute instance:
- To lower license and infrastructure cost

#### Tools to manage Database Cloud Service (DBCS):
- SQL Developer
- Oracle Enterprise Manager

#### ATP:
- You can scale CPU & storage UP & down


#### Service Console in ATP:
- Set resource management rules.
- Monitor database activity and SQL queries.
- Reset the admin password

#### Limit Batch processes to not interface with the OLTP transactions:
- Configure ATP resource management rules to manage runtime and IO consumption for the consumer group of batch processes


#### Task Performed in OCI console for ADW:
- Increase Storage allocated for Database.
- Scale up/down CPU

#### Backup Strategy for ADW:
- Automated Backup


#### ADW Backup:
- You can backup ADW database only to a standard bucket type in OCI object storage.
- You can perform manual backups to OCI object storage in addition to automated backups available on ADW.



------



#### Pre-Authenticated Requests:
- Changing the bucket visibility does not change existing pre-authenticated request.


#### Add Secondary VNIC in existing instance:
- The primary and secondary VNIC association can be in different VCN but must be in the same availability domain.


#### IPSec VPN Connect:
- OCI IPSec VPN can be configured in tunnel mode only.
- Each OCI IPSec VPN consists of multiple redundant IPSec tunnels.

#### Required to create an IPSec VPN connection:
- Security List
- Static Route CIDR

#### Setup secure and encrypted connectivity to your workloads running in a single virtual cloud network from all company location:
- Create five IPsec connections with each company location and terminate those connections on a single DRG. Attach that DRG to your VCN


#### DRG:
- IPsec VPN.
- Remote VCN peering across region

#### True about Oracle Cloud Infrastructure DNS:
- It supports other cloud providers such as AWS and Azure.
- It supports segregation of traffic by using the private pool

#### HA in OCI:
- Distribute your application servers across all AD within a region.
- Configure your DB to have Data Guard in another AD in Sync mode within a region

#### Ensure that the OCI load balancer does not forward traffic to this backend server during maintenance:
- Drain all existing connections to this backend server and mark the backend web server offline.


#### 3 Load Balancing Policy:
- weighted round robin.
- IP Hash.
- least connection

#### Configure a load balancer to accept incoming traffic:
- A listener.
- A backend set with at least one backend server.
- A security list that is open on the listener port.

#### Certificate format is used with the load balancer:
- PEM


#### Data Guard:
- Both DB systems must be in the same compartment, same VCN, and they must be the same shape.
- Port 1521 must be open.
- Data guard implementation for Bare Metal shapes requires two DB Systems, one containing the primary DB, and one containing the standby DB.

#### Deployment architecture to deploy the Platform Service Manager based Database Cloud Service (DBCS) onto OCI:
- Two node Primary RAC database with a two node RAC Data Guard Standby in Maximum Performance mode

#### Capabilities of the dbaascli utility:
- Start and open the database instance
- Switchover and failover in an Oracle Guard configuration
- Patching the primary database deployment


#### Identity providers your administrator federate with Oracle Cloud Infrastructure:
- Oracle Identity Cloud Service.
- Microsoft Active Directory

#### Automatically install Oracle Cloud Infrastructure CLI:
- PIP


#### Three types of credentials are used to manage OCI IAM:
- API Signing Key.
- Console Password.
- Swift Password

#### Valid tagging attribute included in a payload of an audit log event:
- Free-form Tags
- Defined tags

#### Apply all the latest kernel security updates to all instances:
- OS Management


#### Transfer package:
- A transfer package is the logical representation of the physical shipment containing the HDD transfer devices that you ship to Oracle to upload to OCI.


#### Storage service is used on OCI for a Data Transfer Service job:
- An Object Bucket


------

**1Z0-1085-20:**
https://www.udemy.com/course/1z0-1085-20-oraclecloudinfrastructurefoundationsassociate/?couponCode=ORACLE

**1Z0-1067:**
https://www.udemy.com/course/oracle-cloud-infrastructure-cloud-operations-associate/?couponCode=ORACLE

**1Z0-1072-20:**
https://www.udemy.com/course/1z0-1072-oracle-cloud-infra-architect-associate/?couponCode=ORACLE

**1Z0-1084-20:**
https://www.udemy.com/course/oracle-cloud-infra-developer-2020-associate-practice-test/?couponCode=ORACLE

**1Z0-931:**
https://www.udemy.com/course/oracle-autonomous-database-cloud-specialist-1z0-931-practice-test/?couponCode=ORACLE

**1Z0-997-20:**
https://www.udemy.com/course/1z0-997-oracle-cloud-infrastructure-architect-professional-k/?couponCode=ORACLE


