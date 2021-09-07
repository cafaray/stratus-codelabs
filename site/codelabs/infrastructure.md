summary: Cloud basics
id: resources
categories: cloud
tags: CXB,cloud
status: Published 
authors: cafarias
Feedback Link: https://cafarias.io

# Cloud infrastructure
<!-- ----- -->
## Overview
Duration: 00:01:00

The infrastructure layer is the foundation of the cloud. This layer consists of physical resources that are housed in Regions, Zones and Data Centers. A Cloud provider’s IT environment is typically distributed across many Regions around the world.

- Region: is a geographic area or location where a Cloud provider’s infrastructure is clustered, and may have names like NA South or US East. The cloud Regions are isolated from each other so that if one Region was impacted by a natural disaster like an Earthquake, the Cloud operations in other Regions would keep running.

- Zone: Each Cloud Region can have multiple Zones (or Availability Zones), which are typically distinct Data Centers with their own power, cooling and networking resources. These Zones can have names like DAL-09 or us-east-1. The isolation of zones improves the cloud’s overall fault tolerance, decreases latency, and avoids creating a single shared point of failure.

<aside class="positive">
A cloud Data center is a huge room or a warehouse containing cloud infrastructure. These data centers contain pods and racks or standardized containers of computing resources such as servers, as well as storage, and networking equipment - virtually everything that a physical IT environment has.
</aside>

The Availability Zones (and DataCenters within them) are connected to other AZs and regions, private datacenters and the Internet using very high bandwidth network connectivity.

### What You’ll Learn 

Basic architecture for:

- Compute resources and services 
- Network resources and services
- Storage resources and services

<!-- ------------------------ -->

## Computing
Duration: 00:03:00

Cloud providers offer several computing resources:

- Virtual Servers
- Bare Metal Servers, and 
- Serverless

Most of the servers in a cloud datacenter run hypervisors to create virtual servers or virtual machines (VMs for short), that are software-based computers, based on virtualization technologies.

### Virtual Machines

Virtualization is a fairly old technology, but it's still super relevant to building our cloud computing strategy today. 

<aside class="positive">

**What is virtualization?**

Is the process of creating a software based, or virtual, version of something, whether that be compute, storage, networking, servers, or applications. 
</aside>

Hypervisor is what makes virtualization feasible, it's simply a piece of software that runs above the physical server, or host. And there are a couple different types of hypervisors out there. What they do is essentially pull the resources from the physical server and allocate them to your virtual environments. 

There are two main types of hypervisors out there. 

- Bare-metal hypervisors: The hypervisor is installed directly on top of the physical server. So we'll write that up here. Remember these are the most frequently typed of use hypervisors and they're most secure, they lower the latency, and these are the ones that you'll see in the market the most. Some examples would be VMware, ESXi, or Microsoft Hyper-v, or even open-source KVM. 

- Hosted. These are a lot less frequent. What makes these different is that there is a layer of host OS that sits between the physical server and the hypervisor. They're mostly used for end-user virtualization. You might see some in the market that are called: Oracle, VirtualBox, or VMware Workstation.

<aside class="negative">
Hosted hypervisors have higher latency than Bare-metal. So once you have your hypervisor installed, you can build virtual environments, or virtual machines, or simply put, VMs. So let's spin up some environments.
</aside>

<aside class="positive">
Dedicated hosts offer single-tenant isolation, are typically used for meeting compliance and regulatory requirements or meet specific licensing terms.
</aside>

### Virtual Machine (VM)

A VM is simply a software based computer. They're run like a physical computer. They have an operating system and applications, and they're completely independent of one another, but you can run multiple of them on a hypervisor. And the hypervisor manages the resources that are allocated to these virtual environments from the physical server. Because they're independent you can run different operating systems on different virtual machines. You could run Windows here, or Linux here, or UNIX here for example.

Because they're independent they're also extremely portable. You can move a virtual machine from one hypervisor to another hypervisor on a completely different machine almost instantaneously, which gives you a lot of flexibility and a lot of portability within your environment. So looking at all of this, this's the core virtualization as a process. 

### key benefits. 

1) **Cost savings**. When you think about this and the fact that you can run multiple virtual environments from one piece of infrastructure, means that you can drastically reduce your physical infrastructure footprint. This is consolidation at its core. And the fact that you don't have to maintain nearly as many servers, run as much electricity, save on maintenance costs, means that you save on your bottom line at the end of the day. 

2) **Agility and speed**. Like I said, spinning up a virtual machine is relatively easy and quick - a lot more simple than provisioning an entire new environment for your developers if they say they want to spin up a new environment so that they can run a test scenario. Whatever it might be, virtualization makes that process a lot simpler and quicker. 

3) **Lowers your downtime**. Let's say that this host goes out unexpectedly. The fact that you can move virtual machines from one hypervisor to another, on a different physical server, means that you have a great backup plan in place. So, if this host goes down you can simply move your VMs very quickly to another hypervisor on a machine that is working. Virtualization and VMs are at the center of cloud computing and provide many benefits.

<aside class="positive">
Other servers in the racks are bare metal servers that are physical servers that aren’t virtualized. Customers can provision VMs and Bare Metals servers as and when they need them and run their workloads on them.
</aside>

Cloud users can also run their workloads on serverless computing resources, which are an abstraction layer on top of virtual machines.

## Storage

Information and data can consist of files, code, documents, images, videos, backups, snapshots, and databases and can be stored in many different types of storage options on the Cloud.

Bare Metal Servers and Virtual Servers are provisioned with default storage in local drives. Since these cloud servers can be provisioned and decommissioned by customers on demand and freed up for use by other users, any information stored in a local drive can be lost when you delete or decommission a cloud server.

However there are other storage options available on the cloud to persist data that you can choose depending on factors like how important your data is, how quickly you want to be able to access it, how often you access it, and how secure you need it to be.

These additional storage options include 

- File storage
- Block storage 
- Object storage


Block and file storage modes are commonly used in traditional data centers, but "often struggle with scale, performance and distributed characteristics of cloud."

Object storage is the most common mode of storage in the cloud as it’s both highly distributed and resilient.

### File Storage

Like direct attached storage, file storage must be attached to a compute node before it can be accessed and have data stored on it. However, **File Storage** can be less expensive, more resilient to failure, and involve lesser disk management and maintenance for you as the user to do , as compared to direct attached storage. You can also provision much larger amounts of File Storage and present it as a disk to a server.

File storage is mounted from remote storage appliances. That is, the physical disks are contained in a separate, specialised piece of hardware and they are then connected to the compute node via the underlying infrastructure in the datacentre.

These storage appliances are not only extremely resilient to failure, the data is also far more secure in them as these storage appliances offer services such as encryption in transit and encryption at rest. These appliances are all managed by the service provider.

Sometimes can be referred to as "Network Attached Storage", "Network File Storage" or simply **NFS**. One of the issues with ethernet networks is that their speed can vary *the more loaded an ethernet network is, the more likely it becomes that it's speed or bandwidth will be affected*.

<aside class="positive">
File storage tends to be used for workloads where consistently high network speeds are not a requirement.
</aside>

#### IOPS

When you provision file storage, one consideration you need to take into account is the Input/Output Operations Per Second (IOPS) capacity of the storage, and refers to the speed at which the disks can write and read data.

The higher the IOPS value, the faster the speed of the underlying disk. A higher IOPS will also normally cost more. Understanding IOPS is important because if the IOPS value is too low for your application, the storage can become a bottleneck and cause your application to run slowly. Alternatively, if the IOPS is too high, you will probably be paying more that you need to for your storage.

<aside class="negative">

**NOTE**: *this is not the speed of the network between the storage and the compute node*

</aside>

For example, a file share may be mounted on 30 different compute nodes and an application writes and requests data to and from that share 60 times per minute. You can average that out to 1 operation per second. With this simple example, you can see that each application has different IOPS requirements.

### Block Storage

Block storage breaks files into chunks (or blocks) of data and Stores each block separately under a unique address. Like direct attached storage and file storage, block storage also must be attached to a compute node before it can be utilized for your workloads.

Block storage, like file storage, can be mounted from remote storage appliances, making it extremely resilient to failure, and keeping data far more secure in them, on account of encryption in transit, and encryption at rest services.

Block storage is mounted as a volume to compute nodes using a dedicated network of fibres, through which signals move at the speed of light. These fibre optic networks are more expensive to build than the ethernet ones which deliver File Storage, which is one reason why Block Storage tends to have a higher price-point.

However, since the traffic is moving faster and with speed consistency, they are perfect for workloads that need low-latency storage to work effectively. In terms of workloads, it is important to note that unlike File Storage, which can be
mounted onto 80 computer nodes or more, Block storage is normally mounted onto only one compute node at a time.

Since these disks run at a consistent high speed, they are perfect for workloads that need consistently fast storage, such as databases and mail servers.

### Main differences between FS and BS

So, to summarise the commonalities and differences between these two storage types:

- Block and File Storage is taken from appliances which are maintained by the service provider.
- Both are normally highly available and resilient and will often include data encryption at rest and in transit.
- **File storage** is attached to compute nodes using an ethernet network, so it is sometimes called **Network attached** or NFS Storage.
- **File storage** is very reliable, but the speed of the connecting network can vary, based on load.
- **Block storage** is attached via a high-speed fibre network, which is very reliable and consistent.
- **File storage can be attached to multiple compute nodes at once.**
- **Block storage can only be attached to one node at a time.**
- **File storage** is a good choice where **file shares are required**, where workloads **do not require lightning fast connectivity** to storage, or where **cost is a factor**.
- **Block storage** is a good choice when supporting an application that needs **consistent fast access to disk**, such as databases.


### Object Storage

The first thing to note about Object Storage is that you do not connect it to a particular compute node in order to use it. Instead, you provision an Object Storage service instance and use an API (or Application Program Interface) to upload, download, and manage your data.

<aside class="positive" >
This means you can directly use Object Storage with anything that can call an API and you don’t need an underlying compute node.
</aside>

The second thing to note about Object Storage is that it’s less expensive that other cloud storage options. It’s per gigabyte cost is typically a couple of US cents per month and in some cases, even less, depending on the storage tier used.

The third and possibly most important thing to note about Object Storage is that it’s effectively infinite. With file and block storage, you specify the size of the storage you want in gigabytes or terabytes and then pay a fee based on the size you provisioned. 

<aside class="positive">
With Object Storage, you just consume the storage you need and pay per gigabyte cost for what you use. **You can keep uploading files and the storage will never run out.**
</aside>

Object Storage is great for storing large amounts of unstructured data. By unstructured this means that the data is not stored in any kind of hierarchical folder or directory structure – Object Storage uses *buckets*, and objects are stored within these buckets in a structurally flat way.

A *bucket* is a bit like a folder, in the sense that you can give them meaningful names, and of course have different buckets for different object-types but you cannot place a bucket within a bucket.

When an object is placed in a bucket, it also has some metadata (data about the data) added to it, such as an object ID. This metadata helps applications to both locate and access the object, as well as provide information on the time that the data was stored or last accessed.

When you create a bucket, you don’t need to provide or define any sizing information the bucket will just hold the data that you place inside it and the service provider ensures that there is sufficient storage capacity available.

Buckets can hold as little as a few bytes of data, right up to multiple petabytes and you can build up the amount of data stored as slowly or quickly as you like—as well as shrink it back down again. The service provider also takes care of resilience and making sure that the Object Storage solution is highly available.

Some cloud providers offer different types of buckets with different levels of resilience. For example, they offer buckets which are resilient, but the data is only stored in one data centre.

This is a good option where data needs to reside in a particular geographical location or in situations where high availability is less of an issue. They will then offer buckets which are highly available across regions, where the data is stored multiple times in different datacentres (or zones) in the same region or even in multiple regions. These options usually cost more but they provide both the highest level of resilience as well as availability for your data. 

This data can be anything from text files to audio and video files, from IOT data to virtual machine images, from backup files to data archives.
Pretty much any data which is static and where fast read and write speeds are not necessary would make a good fit for object storage.

Object Storage would, however, not be suitable for running operating systems, nor applications such as databases or anything else where the contents of the files changes.

### Use case
Object Storage is used to store files—or Objects—which are static. The data that you can store using Object Storage can be anything from text files to audio and video files, from IOT data to virtual machine images, from backup files to data archives.

<aside class="negative">
You cannot run operating systems or other applications such as databases using Object Storage.
</aside>

Objects are stored in Buckets. It is possible to have multiple buckets, but you cannot place buckets within buckets. It is not need to specify a size for a bucket, you can just use as little or as much space as need.

Many providers offer different types of buckets with different charges for each. Some are based on resilience and availability, while others are based on the frequency at which the objects inside are accessed.

## Networking

Networking infrastructure in a cloud datacenter includes traditional networking hardware like routers and switches, but more importantly for users of the Cloud, the Cloud providers have Software Defined Networking (or SDN) options where certain networking resources are virtualized or made available programmatically, through APIs.

This allows for easier network provisioning, configuration, and management in the cloud. When servers in the cloud are provisioned, you need to setup their public and private network interfaces.

The public network interfaces, as the name suggests, connect the servers to the public internet, whereas the private ones provide connectivity to your other cloud resources and help keep them secure.

As in the physical IT world, network interfaces in the cloud need to have **IP addresses** and subnets either assigned automatically or configured. In a cloud environment it is even more important to configure which network traffic and users
can access your resources, which can be done by setting up **Security Groups and Access Control Lists** (or ACLs).

For further security and isolation of your resources in the cloud, most Cloud providers provide 
- **Virtual Local Area Networks** (VLANs)
- **Virtual Private Clouds** (VPCs)
- **Virtual Private Networks** (VPNs).

Some of the traditional hardware appliances such as firewalls, load balancers, gateways and traffic analyzers can also be virtualized and made available as services in the cloud. Another networking capability provided by the Cloud Providers is Content Delivery Networks or CDNs, that distribute content to multiple points throughout the world so users accessing
the content can access it more quickly by getting it from a point nearest to them.

### Secure Networking in Cloud

As one might expect, the notion of building a cloud network is not much different from deploying a network in an on-premises data center. The main difference stems from the fact, that in the cloud, we use logical instances of networking elements as opposed to physical devices.

![Virtual Networks](./assets/virtual_networks.jpg)

For example, Network Interface Controllers (NICs) would be represented by vNICs in cloud environments.

Cloud networks are deployed in networking spaces that are logically separated segments of the networks using options, including **Virtual private Cloud** (VPC) that in turn can be divided into smaller segments called subnets. Logically segmented cloud networks are private carveout of the cloud that offer customers the security of private clouds and the scalability of public clouds.

Cloud resources, such as VMs or **Virtual Server Instances** (VSIs), Storage, network connectivity and load balancers are deployed into subnets. Using subnets allows users to deploy enterprise applications using the same multi-tier concepts used in on-premises environments. 

Subnets are also the main area where security is implemented in the cloud. Every subnet is protected by Access Control Lists (ACLS) that serve as a subnet-level fire wall. Within the subnet, one could create **Security Groups** that provide security at the instance level such as VSIs. Once you build a subnet, then it is time to add some VSIs and storage to it so that you could run your applications.

Let’s say you have a 3-tier application that require web access VSIs, applications tier VSIs and backend database VSIs. In this case, we would place the web facing VSIs into one Security Group, the Application VSIs in a second Security Group, while the database VSIs in a third SG. It goes without saying that the web facing VISs need Internet access.

A public Gateway instance is added to the network to enable user's access to the application in the internet tier. While public gateways are great for Internet access to the cloud, enterprises are interested in extending their on-premises resources to the cloud by securely connecting them using **Virtual Private Networks**, or VPNs.

When building many subnets and deploying several workloads, it becomes necessary to ensure that applications continue to be responsive. That is achieved with Load Balancers that ensure availability of bandwidth for the different applications. Enterprises with hybrid cloud environment find using dedicated high-speed connections between clouds and on-premises resources is a more secured and more efficient way than public connectivity solutions.

Some cloud service providers offer such connectivity, such as IBM Cloud and its Direct Link solution that enables extending on-premises resources to the cloud as needed. Building a cloud network entails creating a set of logical constructs that deliver networking functionality that is akin to the data center networks that all IT professionals have come to rely on for securing their environments and ensuring high performing business applications.
