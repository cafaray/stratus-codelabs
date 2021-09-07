summary: Cloud basics
id: basics
categories: cloud
tags: CXB,cloud
status: Published 
authors: cafarias
Feedback Link: https://cafarias.io

# Cloud computing
<!-- ------------------------ -->
## Overview 
Duration: 00:05:00

Cloud computing is the on-demand delivery of IT resources over the Internet with pay-as-you-go pricing. Instead of buying, owning, and maintaining physical data centers and servers, you can access technology services, such as computing power, storage, and databases, on an as-needed basis from a cloud provider like AWS, Google, Azure, IBM.

<!-- ------------------------ -->

### Computing resources 

- Networks
- Computing
- Storage
- Applications
- Services

<aside class="positive">
<b>IBM Cloud</b> model is composed of five essential characteristics, three deployment models, and three service models.
</aside>

<!-- ------------------------ -->

### Essential characteristics of the cloud

- On-demand self-service
You get access to cloud resources such as the processing power, storage, and network you need, using a simple interface, without requiring human interaction with each service provider.

- Broad network access
Cloud computing resources can be accessed via the network through standard mechanisms and platforms such as mobile phones, tablets, laptops, and workstations. 

- Resource pooling
Gives cloud providers economies of scale, which they pass on to their customers, making cloud cost-efficient. Using a multi-tenant model, computing resources are pooled to serve multiple consumers; cloud
resources are dynamically assigned and reassigned, according to demand, without customers needing to concern themselves with the physical location of these resources. 

- Rapid elasticity
Implies that you can access more resources when you need them, and scale back when you don’t—because resources are elastically provisioned and released.

- Measured service
Only pay for what you use or reserve as you go; if you’re not using resources, you’re not paying. Resource usage is monitored, measured, and reported transparently based on utilization.

<aside class="positive">
<b>Cloud computing is really about</b> utilizing technology "as a service", leveraging remote systems on-demand over the open internet, scaling up and scaling back, and paying for what you use.
</aside>

<!-- ----------------- -->

### Types of deployment models

The deployment model indicates where the infrastructure resides, who owns and manages it, and how cloud resources and services are made available to users.

The three cloud deployment models include:

- Public Cloud, 
- Private Cloud, and 
- Hybrid Cloud.

### What You’ll Learn 

* Define what cloud computing is 
* Identify cloud deployment models
* Types of cloud computing
* Essential characteristics
* Benefits of cloud computing 
* Use cases

## Public
Duration: 00:05:00

Leverage cloud services over the open internet on hardware owned by the cloud provider, but its usage is shared by other companies.


Users get access to servers, storage, network, security, and applications as services delivered by cloud service providers over the internet.

Using web consoles and APIs, users can provision the resources and services they need.

The cloud provider owns, manages, provisions, and maintains the infrastructure, renting it out to customers either for a subscription charge or usage-based fee.

Users don’t own the servers their applications run on or storage their data consumes, or manage the operations of the servers, or even determine how the platforms are maintained.

In very much the same way that we consume and pay for utilities such as water, electricity, or gas in our everyday lives, we don’t own any of these cloud resources—we make an agreement with the service provider, use the resources, and pay for what we use within a certain period.

Public clouds offer significant cost savings as the provider bears all the capital, operational, and maintenance expenses for the infrastructure and the facilities they are hosted in. It makes scalability as easy as requesting more capacity.

<aside class="negative">
However, with a public cloud, the user does not have any control over the computing environment and is subject to the performance and security of the cloud provider’s infrastructure.
</aside>

There are several public cloud providers in the market today, such as Amazon Web Services, Microsoft Azure, IBM Cloud, Google Cloud Platform, and Alibaba Cloud.

While all providers include a common set of core services, such as servers, storage, network, security, and databases, they also offer a wide spectrum of niche services with varied payment options.

### Characteristics of a public cloud:
A public cloud is a virtualized multi-tenant architecture enabling tenants or users to share computing resources, residing outside their firewalls.

The cloud providers pool of resources, including infrastructure, platforms, and software, are NOT dedicated for use by a single tenant or organization.

Resources are distributed on an as-needed basis offered through a variety of subscription and pay-as-you-go models.

### Benefits

Vast on-demand resources are available, allowing applications to respond seamlessly to fluctuations in demand.

Considering the large number of users that share the centralized cloud resources on-demand, the public cloud offers the most significant economies of scale.

The sheer number of server and network resources available on the public cloud means that a public cloud is highly reliable—if one physical component fails, the service still runs unaffected on the remaining available components.

It’s also important to note some concerns users have regarding public clouds—key among them being security and data sovereignty compliance.

Security issues such as data breaches, data loss, account hijacking, insufficient due diligence, and system and application vulnerability seem to be some of the fears users continue to have concerning security in the public cloud.

With data being stored in different locations and accessed across national borders, it has also become increasingly critical for companies to be compliant with data sovereignty regulations governing the storage, transfer, and security of data.

A service provider’s ability to not just keep up with the regulations, but also the interpretation of these regulations, is a concern shared by many businesses.

### Use cases

Organizations are increasingly opting to access cloud-based applications and platforms so their teams can focus on building and testing applications, and **reducing time-to-market** for their products and services.

Businesses with **fluctuating capacity and resourcing needs** are opting for the public cloud.

Organizations are using public cloud computing resources to build secondary infrastructures for **disaster recovery, data protection, and business continuity**.

More and more organizations are using cloud storage and data management services for **greater accessibility, easy distribution, and backing up** their data.

IT departments are outsourcing the management of less critical and standardized business platforms and applications to pubic cloud providers.


## Private
Duration: 00:05:00

Cloud infrastructure is provisioned for exclusive use by a single organization. It could run on-premises or it could be owned, managed, and operated by a service provider

The National Institute of Standards and Technology defines Private Cloud as:

 <aside class="positive">
 Cloud infrastructure provisioned for exclusive use by a single organization comprising multiple consumers, such as the business units within the organization. It may be owned, managed, and operated by the organization, a third party, or some combination of them, and it may exist on or off premises.
 </aside>

#### Internally implementation 

When the platform is provisioned over an organization’s internal infrastructure, it runs **on-premises** and is owned, managed, and operated by the organization.

#### Externally implementation

When it is provisioned over a cloud provider’s infrastructure, it is owned, managed, and operated by the service provider.
This external private cloud offering that resides on a cloud service provider’s infrastructure is called a *Virtual Private Cloud* (VPC).

### Virtual Private Cloud

A VPC is a public cloud offering that lets an organization establish its own private and secure cloud like computing environment in a logically isolated part of a shared public cloud.

Using a VPC, organizations can leverage the dynamic scalability, high availability, and lower cost of ownership of a public cloud, while having the infrastructure and security tailored to the organization’s unique needs.

Virtual Private Clouds are offered by most Public Cloud providers such as Google, Amazon, and IBM Cloud. A private cloud is a virtualized environment modeled to bring in the benefits of a public cloud platform without the perceived disadvantages of an open and shared public platform.

![VPC](./assets/vpc.jpg)

### Benefits

Users of a private cloud, such as Developers and Business Units in an organization, still get to leverage benefits such as: 

* economies of scale, 
* granular scale, 
* operational efficiencies, and 
* user self-service

While exercising full control over 

* access, 
* security, and 
* compliances specific to their organization and business.

Private clouds provide you with the ability to leverage the value of cloud computing using systems that are directly managed or under perceived control of the organization’s internal IT.

The ability to better utilize internal computing resources, such as the organization’s existing investments in hardware and software, thereby reducing costs.

Better scalability through virtualization and "cloud bursting" i.e., leveraging public cloud instances for a period of time but returning to the private cloud when the surge is met.

Controlled access and greater security measures customized to specific organizational needs.

The ability to expand and provision things in a relatively short amount of time, providing greater agility.

### Use cases

Organizations may choose to opt for private cloud because of various reasons. Their applications provide a unique competitive advantage, there are security and regulatory concerns, or because the data is highly sensitive and subject to strict industry or governmental regulations.

- A private cloud is an opportunity for organizations to **modernize and unify** their in-house and legacy applications. Moving these applications from their dedicated hardware to the cloud also allows them to leverage the power of the compute resources and multiple services available on the cloud.

- Using the private cloud, organizations are **integrating data** and application services from their existing applications with public cloud services. This allows them to leverage their private cloud’s compute capability for the larger jobs while pulling data into an application on a private cloud to leverage public cloud services—essentially opening their data centers to work with cloud services.

- **Application portability** is a key feature of cloud platforms. Using the private cloud gives organizations the flexibility to build applications anywhere, and move them anywhere, without having to compromise security and compliance in the process.

- Some of the key reasons that may prevent an organization from moving to a public cloud include **security and regulatory concerns, and data sensitivity**. A private cloud offers these organizations the benefits of on-demand enterprise resources while exercising full control over critical security and compliance issues from within the environment of their dedicated cloud.

## Hybrid
Duration: 00:05:00

Hybrid cloud is a computing environment that connects an organization’s on-premise private cloud and third-party public cloud into a single, flexible infrastructure for running the organization’s applications and workloads.

The mix of public and private cloud resources gives organizations the **flexibility** to choose the optimal cloud for each application or workload.

Workloads **move freely** between the two clouds as needs change. 

Organizations can **choose to run the sensitive**, highly-regulated, and mission-critical applications or workloads with reasonably constant performance and capacity requirements on private cloud infrastructure while deploying the less-sensitive and more-dynamic workloads on the public cloud.

With proper integration and orchestration between the public and private clouds, you can leverage both clouds for the same workload.

<aside class="positive">
<b>Cloud Bursting</b>: Leverage additional public cloud capacity to accommodate a spike in demand for a private cloud application.
</aside>

### Three tenets of a hybrid cloud:

- Interoperability
Hybrid cloud is interoperable which means that the public and private cloud services can understand each other’s APIs, configuration, data formats, and forms of authentication and authorization.

- Scalability
When there is a spike in demand, a workload running on the private cloud can leverage the additional public cloud capacity, making it scalable.

- Portability 
A hybrid cloud is also portable since you’re no longer locked-in with a specific vendor, you can move applications and data not just between on-premise and cloud systems, but also between cloud service providers.

Hybrid is about taking the best of both worlds.

### Types of Hybrid cloud

- Monocloud
A hybrid monocloud is a hybrid cloud with one cloud provider, while a hybrid multicloud is an open standards-based stack that can be deployed on any public cloud infrastructure.

The difference lies in the flexibility that the hybrid multicloud offers organizations to move workloads and environments from one vendor to another.

- Multicloud
There is also a variant of hybrid multicloud, called the composite multicloud, which makes this flexibility even more granular as it distributes single applications across multiple providers, allowing you to move application components across cloud services and vendors as needed.

### Benefits

Hybrid cloud offers significant benefits in areas of 

- Security and compliance
A hybrid cloud lets organizations deploy highly regulated or sensitive workloads in a private cloud while running the less-sensitive workloads on a public cloud.

- Scalability and resilience 
Using a hybrid cloud, you can scale up quickly, inexpensively, and even automatically using the public cloud infrastructure, all without impacting the other workloads running on your private cloud.

- Resource optimization 
Because you’re not locked-in with a specific vendor and also don’t have to make either or decisions between the different cloud models, you can make the most cost-efficient use of your infrastructure budget.

- Cost saving
You can maintain workloads where they are most efficient, spin-up environments using pay-as-you-go in the public cloud, and rapidly adopt new tools as you need them.

### Use cases

Let’s look at some increasingly common hybrid cloud use cases:

- Software-as-a-Service integration.
Through hybrid integration, organizations are connecting Software-as-a-Service applications available in the public cloud to their existing public cloud, private cloud, and traditional IT applications to deliver new solutions.

- Data and AI integration. 
Organizations today are creating richer and more personal experiences by combining new data sources on the public cloud—such as weather, social, the Internet of Things, CRM, and ERP—with existing data and analytics, machine learning, and AI capabilities.

- Enhancing legacy apps. 
An increasing number of organizations are using public cloud services to upgrade the user experience of their on-premises applications and deploy them globally to new devices, while incrementally modernizing their core business systems.

- VMware migration.
More and more organizations are “lifting and shifting” their on-premises virtualized workloads to a public cloud without conversion or modification to reduce their on-premises data center footprint and position themselves to scale without added capital expense.

<!-- --------------------------- -->


## Deployment models 
Duration: 00:03:00

There are three types of deployment models at the cloud computing resurces.

### PaaS

PaaS removes the need for you to manage underlying infrastructure (usually hardware and operating systems), and allows you to focus on the deployment and management of your applications. This helps you be more efficient as you don’t need to worry about resource procurement, capacity planning, software maintenance, patching, or any of the other undifferentiated heavy lifting involved in running your application. 

### SaaS

SaaS provides you with a complete product that is run and managed by the service provider. In most cases, people referring to SaaS are referring to end-user applications (such as web-based email). With a SaaS offering, you don’t have to think about how the service is maintained or how the underlying infrastructure is managed. You only need to think about how you will use that particular software. 

### IaaS

IaaS contains the basic building blocks for cloud IT. It typically provides access to networking features, computers (virtual or on dedicated hardware), and data storage space. IaaS gives you the highest level of flexibility and management control over your IT resources. It is most similar to the existing IT resources with which many IT departments and developers are familiar. 

<!-- ------------------------ -->

## Benefits of using cloud computing
Duration: 00:05:00

### Agility

The cloud gives you easy access to a broad range of technologies so that you can innovate faster and build nearly anything that you can imagine. You can quickly spin up resources as you need them-from infrastructure services, such as compute, storage, and databases to Internet of Things (IoT), Machine learning (ML), data lakes and analytics, and much more.

You can deploy technology services in a matter of minutes, and get from idea to implementation several orders of magnitude faster than before. This gives you the freedom to experiment, test new ideas to differentiate customer experiences, and trasform business.

### Elasticity

With cloud computing, you don't have to over-provision resources up front to handle peak levels of business activity in the future. Instead, you provision the amount of resources that you actually need. You can scale these resources up or down to instantly grow and shrink capacity as your business needs change.

### Cost savings

The cloud allows you to trade capital expenses (such as data centers and physical servers) for variable expenses, and only pay for IT as you consume it. Plus, the variable expenses are much lower than what you would pay to do it yourself because of the economies of scale. 

### Deploy globally in minutes

With the cloud, you can expand to new geographic regions and deploy globally in minutes. Cloud providers usually have a set of CPD's all over the world, so you can deploy your application in multiple physical locations with just a few clicks. Putting applications in closer proximity to end users reduces latency and improves their experience. 

<!-- ------------------------ -->
