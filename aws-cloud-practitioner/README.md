# AWS Cloud Practitioner (CLF-C01)

### IT Terminology

- **Network:** cables, routers, and servers connected with each other
- **Router:** A networking device that forwards data packets between computer networks. They know where to send your packets on the internet!
- **Switch:** Takes a packet and send it to the correct server / client on your network

### Problems With the Traditional IT Approach

- Pay rent for the data center
- Pay for power supply, cooling, and maintenance
- Adding and replacing hardware takes time
- Scaling is limited
- Hire 24/7 team to monitor the infrastructure
- How to deal with disasters? (earthquake, power shutdown, etc.)

### What is Cloud Computing?

- Cloud Computing is the **on-demand delivery** of computer power, database storage, applications, and other IT resources
- Through a cloud services platform with **pay-as-you-go pricing**
- You can **provision exactly the right type and size of computing** resources you need
- You can access as many resources as you need, **almost instantly**
- Simple way to access **servers, storage, databases** and a set of **application services**.

### Examples of Cloud services

- **Gmail**
  - E-mail cloud service
  - Pay for ONLY your emails stored (no infrastrucutre, etc)
- **Dropbox**
  - Cloud Storage service
  - Originally built on AWS
- **Netflix**
  - Built on AWS
  - Video on Demand

### The Deployment Models of the Cloud

- **Private Cloud:**
  - Cloud services used by a single organization, not exposed to the public
  - Complete control
  - Security for sensitive applications
  - Meet specific business needs
- **Public Cloud:**
  - Cloud resources owned and operated by a third-party cloud service provider delivered over the internet
  - Six advantages of Cloud Computing
- **Hybrid Cloud:**
  - Keep some servers on premises and extend some capabilities to the cloud
  - Control over sensitive assets in your private infrastructure
  - Flexibility and cost-effectiveness of the public cloud

### The 5 Characteristics of Cloud Computing

- **On-demand self service:**
  - Users can provision resources and use them without human interaction from the service provider
- **Broad network access:**
  - Resources available over the network, and can be accessed by diverse client platforms
- **Multi-tenancy and resource pooling:**
  - Multiple customers can share the same infrastructure and applications with security and privacy
  - Multiple customers are serviced from the same physical resources
- **Rapid elasticity and scalability:**
  - Automatically and quickly acquire and dispose resources when needed
  - Quickly and easily scale based on demand
- **Measured service:**
  - Usage is measured, users pay correctly for what they have used

### The 6 Advantages of Cloud Computing

- **Trade capital expense (CAPEX) for Operational Expense (OPEX):**
  - Pay on-demand: don't own hardware
  - Reduced total cost of ownership (TCO) & operational expense (OPEX)
- **Benefit from massive economies of scale:**
  - Prices are reduced as AWS is more efficient due to large scale
- **Stop guessing capacity:**
  - Scale based on actual measured usage
- **Go global in minutes:**
  - Leverage the AWS global infrastructure
- **Increase speed and agility**
- **Stop spending money running and maintaining data centers**

### Problems Solved By the Cloud

- **Flexibility:** change resource types when needed
- **Cost-Effectiveness:** pay as you go, for what you use
- **Scalability:** Accommodate larger loads by making hardware stronger or adding additional nodes
- **Elasticity:** Ability to scale out and scale-in when needed
- **High-availability & Fault-tolerance:** build across data centers
- **Agility:** rapidly develop, test, and launch software applications

### Types of Cloud Computing

- **Infrastructure as a Service (IaaS):**
  - Provide building blocks for cloud IT
  - Provides networking, computers, data storage space
  - Highest level of flexibility
  - Easy parallel with traditional on-premises IT
- **Platform as a Service (PaaS):**
  - Removes the need for your organization to manage the underlying infrastructure
  - Focus on the deployment and management of your applications
- **Software as a Service (SaaS):**
  - Completed product that is run and managed by the service provider

<br>
<br>

| Answer | Management        |
| ------ | ----------------- |
| Yes    | Managed by You    |
| No     | Managed by Others |

| Type           | On-premises | IaaS                                       | Paas                                       | SaaS                                       |
| -------------- | ----------- | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| Applications   | Yes         | Yes                                        | Yes                                        | <strike style="color: orange;">No</strike> |
| Data           | Yes         | Yes                                        | Yes                                        | <strike style="color: orange;">No</strike> |
| Runtime        | Yes         | Yes                                        | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| Middleware     | Yes         | Yes                                        | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| O/S            | Yes         | Yes                                        | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| Virtualization | Yes         | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| Servers        | Yes         | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| Storage        | Yes         | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |
| Networking     | Yes         | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> | <strike style="color: orange;">No</strike> |

### Example of Cloud Computing Types

- **IaaS**:
  - Amazon EC2 (On AWS)
  - GCP, Azure, Rackspace, Digital Ocean, Linode
- **PaaS:**
  - Elastic Beanstalk (On AWS)
  - Heroku, Google App Engine, Windwos Azure (Microsoft)
- **SaaS:**
  - Many AWS services such as **Rekognition for Machine Learning**
  - Google Apps (Gmail), Dropbox, Zoom

### Pricing of the Cloud

- AWS has 3 pricing fundamentals, following the pay-as-you-go pricing model:
  - **Compute:**
    - Pay for compute time
  - **Storage:**
    - Pay for data stored in the cloud
  - **Data transfer OUT of the cloud:**
    - Data transfer **IN** is free
  - Solves the expensive issue of traditional IT

### AWS Cloud Use Cases

- Enterprise IT, Backup & Storage, Big Data analytics
- Website hosting, Mobile & Social Apps
- Gaming

### AWS Global Infrastructure

- **AWS Regions:**
  - AWS has regions all around the world
  - Names can be **us-east-1**, **eu-west-3**
  - A region is a cluster of data centers
  - Most AWS services are region-scoped
  - **How to choose an AWS region?**
    - **Compliance with data governance and legal requirements:** data never leaves a region without your explicit permission
    - **Proximity to customers:** reduced latency
    - **Available services within a region:** new services and new features aren't available in every region
    - **Pricing** varies from region to region and is transparent in the service pricing page
- **AWS Availability Zones:**
  - Each region has many availability zones, usually 3, min is 3, and max is 6.
  - For example, we have a region called **us-west-1**, the availability zones would be:
    - us-west-1**a**
    - us-west-1**b**
    - us-west-1**c**
  - Each AZ is one or more discrete data center with redundant power, networking, and connectivity
  - They're seprate from each other, so that they're isolated from disasters
  - They're connected with high bandwidth, ultra-low latency networking
- **AWS Points of Presence (Edge Locations):**
  - Amazon has around 216 Points of Presence (205 Edge Locations & 11 Regional Caches) in 84 countries across 42 countries
  - Content is delivered to end users with low-latency

### Shared Responsibility Model Diagram

- **Customer** = Responsibility for the security **IN** the cloud
  - Customer data
  - Platform, Applications, Identity & Access Management
  - Operating System, Network & Firewall Configurations
  - Client-side data encryption & data integrity authentication
  - Server-side encryption (file system and/or data)
  - Networking traffic protection (encryption, integrity, identity)
- **AWS** = Responsibility for the security **OF** the cloud
  - Software
    - Compute
    - Storage
    - database
    - Networking
  - Hardware / AWS Global Infrastructure
    - Regions
    - Availability Zones
    - Edge Locations

### AWS Acceptable Use Policy

- No illegal, harmful, or offensive use or Content
- No security violations
- No network abuse
- No E-mail or other message abuse

<br>
<br>

## IAM: Users & Groups

- IAM = Identity and Access Management (**Global** Service)
- **Root account** created by default, shouldn't be used or shared
- **Users** are people within your organization, and can be grouped
- **Groups** only contain users, not other Groups
- Users don't have to belong to a group, and a user can belong to multiple groups

### IAM: Permissions

- **Users and Groups** can be assigned JSON documents called policies
- These policies define the **permissions** of the users
- In AWS you apply the **least priviledge principle:** don't give more permission than a user needs
