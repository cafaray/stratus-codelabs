summary: Cloud basics
id: cloud_services
categories: cloud
tags: CXB,cloud
status: Published 
authors: cafarias
Feedback Link: https://cafarias.io

# Cloud services
<!-- ------------------------ -->
## Overview 
Duration: 00:01:00

So let's start with the foundation here with **Infrastructure as a service**. IaaS is a set of compute networking and storage resources that have been virtualized by a vendor so that a user can access and configure them any way they want. In design we have a concept of talking about users, called personas, and the persona for IaaS is a system admin, or an IT admin. 

Let's jump up to the top with **Software as a Service** that's the easy one. Software as a Service is just software that you
don't have to install on your machine and you don't have to manually update. And so the user for Software as a Service could be anyone. In fact, if you're watching this on YouTube right now, then you're a user of Software as a Service. It's usually charged on a subscription model rather than a one-time license fee.

And that brings us to **Platform as a Service**. PaaS takes advantage of all the virtualized resources from Iaas and then just abstracts them away, so the user doesn't have to worry about managing any of those virtualized resources. The user for PaaS is not a system admin, usually. It's usually a dev.

### Metaphor: Having a car. 

- IaaS is like leasing a car. So if you've ever leased a car, you probably did a lot of research, and you care about the specs of the car and their performance. You care about the color of the car, what kind of car it is. You're the one driving and you're the one paying for it. You're also paying for the gas and any tolls or maintenance. 

- Platform as a Service, is more like renting a car. So say you're on vacation and you just got off at the air Airport and you're going to pick up your rental car. You don't really care what color it is. You don't even care about the specs of it, but you're still driving and you're paying for the gas and any tolls you go through. 

- Software as a Service is again the easiest one. That one's more like getting a taxi or an uber. So with the taxi or an uber, you don't care at all about what kind of car it is, what color it is. And in fact, you're not even the one driving, or paying for gas, or any tolls because that's baked into the price. 

### Resume
So let's see what it means in terms of cloud computing and its three service models with **IaaS** the cloud provider manages the physical resources, data centers, cooling power, Network and security, as well as computing resources that include servers and storage. 

With **PaaS**, the provider, in addition to the computing resources, also manages the platform infrastructure which includes the operating systems, development tools, databases, and business analytics. 

In the **SaaS** model, in addition to the infrastructure and the platform resources, the provider also hosts and manages the applications and data.

### What You’ll Learn 

Understand model service, key concepts and use cases for: 

- Infrastructure as a service 
- Platform as a service 
- Software as a service

<!-- ------------------------ -->

## Infrastructure as a Service 
Duration: 00:03:00

### Overview 

It's a form of cloud computing that delivers fundamental compute, network, and storage resources to consumers on-demand, over the Internet, on a pay-as-you-go basis.

![Image with main three elements in cloud computing](./assets/main_three.jpg)

The cloud provider hosts the infrastructure components traditionally present in an on-premises data center as well as the virtualization or hypervisor layer.

In an IaaS Cloud environment, customers can create or provision virtual machines (VMs) in their choice of Region and Zone available from the Cloud Provider. 

These VMs typically come pre-installed the customer’s choice of operating system. The customers can then deploy middleware, install applications, and run workloads on these VMs. They can also and create storage for their workloads and backups.

![Diagram VMs](./assets/vms.jpg)

<aside class="positive">
Cloud providers often provide customers the ability to track and monitor the performance and usage of their cloud services and manage disaster recovery.
</aside>

### Key components

- Physical data centers: 
IaaS providers manage large data centers that contain the physical machines required to power the various layers of abstraction on top of them. In most IaaS models, end users do not interact directly with the physical infrastructure
but experience it as a service provided to them.

- Compute: 
IaaS providers manage the hypervisors and end-users programmatically provision virtual instances with desired amounts of compute, memory, and storage resources. Cloud compute typically comes with supporting services like auto scaling and load balancing that provide scalability and high performance.

- Network: 
Users get access to networking resources on the cloud through virtualization or programmatically, through APIs.

- Storage: 
There are three types of cloud data storage: object, file, and block storage. Object storage is the most common mode of storage in the cloud, given that it is highly distributed and resilient. 

### Use cases.

Organizations today are using cloud infrastructure services to enable their teams to set up **test and development** environments faster, helping create new applications more quickly. By abstracting the low-level components, cloud infrastructure is helping developers focus more on business logic than infrastructure management.

**Business continuity and disaster recovery** require a significant amount of technology and staff investments. IaaS is helping organizations reduce this cost and make applications and data accessible as usual during a disaster or outage.

Organizations are using cloud infrastructure to deploy their web applications **faster and also scale infrastructure up and down** as demand fluctuates.

Organizations are leveraging the **high-performance computing** capabilities of cloud infrastructure to solve complex problems involving millions of variables and calculations, such as climate and weather predictions and financial modeling.

**Big data analysis**, mining massive data sets to locate valuable patterns, trends, and associations requires a huge amount of processing power.
Cloud infrastructure not only provides the required high-performance computing but also makes it economically viable.

<aside class="positive">
While there are some concerns regarding the lack of transparency in the cloud infrastructure’s configuration and management and dependency on a third-party for workload availability and performance Infrastructure-as-a-Service is the fastest growing cloud model today.
</aside>

## Platform  as a Service
Duration: 00:03:00

### Overview

Commonly referred to as “PaaS,” is a cloud computing model that **provides customers a complete platform hardware, software, and infrastructure** to:

- develop, 
- deploy, 
- manage, and 
- run 

applications created by them or acquired from a third-party.

The PaaS provider hosts everything 

servers, 
networks, 
storage, 
operating system, 
application runtimes, 
APIs, 
middleware, 
databases, 

Also include other tools at their data center.

The provider also takes responsibility for the installation, configuration, and operation of the application infrastructure, leaving the user responsible for only the application code and its maintenance.

Customers pay for this service on a usage basis and purchase resources on-demand. 

<aside class="negative">
With IaaS, the cloud provider offers access to ‘raw’ computing resources, such as servers, storage, and networking, while the user is responsible for the platform and application software.
</aside>

With PaaS, the cloud service provider delivers and manages the entire platform infrastructure, abstracting users from the lower-level details of the environment.

![Piramid Infrastructure-Platform-Software](./assets/piramid.jpg)


### Essential characteristics

- PaaS clouds are distinguished by the **high level of abstraction** they provide to the users, eliminating the complexity of deploying applications, configuring infrastructure, and provisioning and configuring supporting technologies like load balancers and databases.

- PaaS clouds **provide services and APIs** that help simplify the job of developers in delivering elastically scalable and highly available cloud applications. These services typically include a variety of capabilities such as APIs for distributed
caching, queuing and messaging, file and data storage, workload management, user identity, and analytics, thus eliminating the need to integrate disparate components.

- The PaaS **runtime environment** executes end-user code according to policies set by the application owner and cloud provider.

- Many of the PaaS offerings provide developers with **rapid deployment mechanisms**, or “push and run” mechanism, for deploying and running applications.

- PaaS offerings support a range of application infrastructure or **middleware capabilities**, such as application servers, database management systems, business analytics services, mobile back-end services, integration services, business process management systems, rules engines, and complex event processing systems.

<aside class="positive">
Such an application infrastructure assists developers by reducing the amount of code that must be written while expanding the application’s functional capabilities. The most important use case for PaaS is strategic—build, test, deploy, enhance, and scale applications rapidly and cost-effectively.
</aside>

### Use cases

- API development and management: 
Organizations are using PaaS to develop, run, manage, and secure APIs and microservices, which are loosely
coupled, independently deployable components and services.

- Internet of Things, or IoT: 
PaaS clouds support a broad range of application environments, programming languages, and tools used for IoT deployments.

- Business analytics/intelligence: 
PaaS tools allow organizations to analyze their data to find business insights that enable more informed business decisions and predictions.

- Business Process Management, or BPM: 
Organizations are using the PaaS cloud to access BPM platform delivered as a service.

- Master data management, or MDM: 
Organizations are leveraging the PaaS cloud to provide a single point of reference for critical business data such as information about customer transactions and analytical data to support decision making.

### Advantages 

- Scalability. 
made possible because of the rapid allocation and deallocation of resources with a pay-as-you-use model offered by PaaS.  The APIs, support services, and middleware capabilities that PaaS clouds provide assist developers in focusing their efforts on application development and testing, 

- Faster time to market
For their products and services and middleware capabilities also reduce the amount of code that needs to be written while expanding the application’s functional capabilities.

- Greater agility and innovation 
Because using PaaS platforms means that you can experiment with multiple operating systems, languages, and tools without having to invest in these resources. You can evaluate and prototype ideas with very low risk exposure resulting in faster, easier, less-risky adoption of a wider range of resources.

### Risks

- Information security threats.

- Dependency on the service provider’s infrastructure.

- Services can get impacted when a service provider’s infrastructure experiences downtime.

- Customers lack control over the changes in its strategy, service offerings, or tools.

<aside class="positive">
But the benefits can far outweigh these risks—PaaS continues to experience strong growth and is predicted to become the prevailing platform delivery model moving forward.
</aside>

## Software as a Service
Duration: 00:03:00

### Overview

It's a cloud offering that provides users with access to a service provider’s cloud-based software.

SaaS providers maintain the servers, databases, and code that constitute an application.

They also manage access to the application, including security, availability, and performance.

Applications reside on a remote cloud network, and users use these applications without having to maintain and update the infrastructure.

Core business processes supported by SaaS today / include 

- email and collaboration via offerings such as Microsoft's Office 365 and Google's Gmail, 
- Customer Relationship Management via services such as NetSuite CRM and Salesforce, 
- Human Resource Management via services from Workday and SAP SuccessFactors, 
- financial management, billing and collaboration, and many more.

According to Forrester Research, SaaS has overtaken on-premises solutions in categories such as human capital management (HCM), customer relationship management (CRM), and collaboration.

Solutions once available with several different deployment options are now SaaS-only.

### Characteristics 

- SaaS clouds have a multitenant architecture. Infrastructure and code are maintained centrally and accessed by all users.

- SaaS makes it easy for users to manage privileges, monitor data use, and ensure everyone sees the same information at the same time. 

- Security, compliance, and maintenance are all part of the offering.

- Users can customize applications to fit their business processes with point-and-click ease. Users can customize the UI to work with their branding guidelines; they can modify data fields and enable or disable features within the business process.

- Users pay for the use of the services via a subscription model. The use of resources can be scaled easily, depending on service needs.

### Key benefits

Businesses can directly procure solutions without upfront capital and assistance from IT, **greatly reducing the time from decision **to value from months to days.

SaaS greatly **increases workforce productivity and efficiency**. Users can access core business apps from wherever they; they can also buy and deploy apps in minutes reducing the typical obstacles enterprises have to to test the products they they might use.

Using SaaS applications, individuals and small enterprises can **spread out their software costs** over time.

### Use cases

Organizations are moving to SaaS for their core business needs as part of their strategic transformation to 

- Reduce on-premises IT infrastructure and reduce capital expenditure

- Avoid the need for ongoing upgrades, maintenance, and patching, done traditionally by internal IT resources

- Applications run reliably with minimal input, for example, email servers and office collaboration and productivity tools

- To manage their websites, marketing, sales, and operations

- Take advantage of the resilience and business continuity of the cloud provider

<aside class="positive">
Enterprises are now developing SaaS integration platforms (or SIPs) for building additional SaaS applications, moving SaaS beyond standalone software functionality to a platform for mission-critical applications.
</aside>

### Concerns.

Primary among them being **data ownership and data safety**. Security is an important consideration when you’re allowing a **third-party to maintain business-critical data**.

And application access relies on **a good internet connection** if you’re not connected, you cannot access the apps.
