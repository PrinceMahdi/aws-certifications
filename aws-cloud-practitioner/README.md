# AWS Cloud Practitioner (CLF-C01)

#### : : : Notes taken from **Stephane Maarek's** course on Udemy : : :

### IT Terminology

- **Network:** cables, routers, and servers connected with each other
- **Router:** A networking device that forwards data packets between computer networks. They know where to send your packets on the internet!
- **Switch:** Takes a packet and sends it to the correct server/client on your network

### Problems With the Traditional IT Approach

- Pay rent for the data center
- Pay for power supply, cooling, and maintenance
- Adding and replacing hardware takes time
- Scaling is limited
- Hire a 24/7 team to monitor the infrastructure
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
  - Pay for ONLY your emails stored (no infrastructure, etc)
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
  - Keep some servers on-premises and extend some capabilities to the cloud
  - Control over sensitive assets in your private infrastructure
  - Flexibility and cost-effectiveness of the public cloud

### The 5 Characteristics of Cloud Computing

- **On-demand self-service:**
  - Users can provision resources and use them without human interaction from the service provider
- **Broad network access:**
  - Resources available over the network, and can be accessed by diverse client platforms
- **Multi-tenancy and resource pooling:**
  - Multiple customers can share the same infrastructure and applications with security and privacy
  - Multiple customers are serviced from the same physical resources
- **Rapid elasticity and scalability:**
  - Automatically and quickly acquire and dispose of resources when needed
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
- **Elasticity:** Ability to scale out and scale in when needed
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
  - Heroku, Google App Engine, Windows Azure (Microsoft)
- **SaaS:**
  - Many AWS services such as **Rekognition for Machine Learning**
  - Google Apps (Gmail), Dropbox, Zoom

### Pricing of the Cloud

- AWS has 3 pricing fundamentals, following the pay-as-you-go pricing model:
  - **Compute:**
    - Pay for computing time
  - **Storage:**
    - Pay for data stored in the cloud
  - **Data transfer OUT of the cloud:**
    - Data transfer **IN** is free
  - Solves the expensive issue of traditional IT

### AWS Cloud Use Cases

- Enterprise IT, Backup & Storage, Big Data Analytics
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
    - **Pricing** varies from region to region and is transparent on the service pricing page
- **AWS Availability Zones:**
  - Each region has many availability zones, usually 3, min is 3, and max is 6.
  - For example, we have a region called **us-west-1**, the availability zones would be:
    - us-west-1**a**
    - us-west-1**b**
    - us-west-1**c**
  - Each AZ is one or more discrete data centers with redundant power, networking, and connectivity
  - They're separate from each other so that they're isolated from disasters
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
    - Database
    - Networking
  - Hardware / AWS Global Infrastructure
    - Regions
    - Availability Zones
    - Edge Locations

### AWS Acceptable Use Policy

- No illegal, harmful, or offensive use of Content
- No security violations
- No network abuse
- No E-mail or other message abuse

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
- In AWS you apply the **least privilege principle:** don't give more permission than a user needs

### IAM: Policies Structure

- Consists of:
  - **Version:** Policy language version, always include "2012-10-17"
  - **ID:** An identifier for the policy (optional)
  - **Statement:** One or more individual statements (required)
- Statements consist of:
  - **Sid:** An identifier for the statement (optional)
  - **Effect:** Whether the statement allows or denies access (Allow, Deny)
  - **Principal:** Account/user/role to which this policy is applied to
  - **Action:** A list of actions this policy allows or denies
  - **Resources:** A list of resources to which the actions applied to
  - **Conditions** for when this policy is in effect (optional)

### IAM: Password Policy

- Strong passwords = higher security for your account
- You can set up a password policy:
  - Set a minimum password length
  - Require specific character types:
    - Including uppercase letters
    - Lowercase letters
    - Numbers
    - Non-alphanumeric characters
  - Allows all IAM users to change their own passwords
  - Require users to change their password after some time
  - Prevent password re-use

### Multi-Factor Authentication - MFA

- Users have access to your account and can change configurations or delete resources in your AWS account
- **You want to protect your Root Accounts and IAM users**
- MFA = password you know + security device you own
- Main benefits of MFA: if a password is stolen or hacked, the account is not compromised

### MFA Device Options in AWS

- Virtual MFA device (e.g. Google Authenticator)
- Universal 2nd Factor (U2F) Security Key (e.g. YubiKey by Yubico )
- Hardware Key Fob MFA Device provided by Gemalto
- Hardware Key Fob MFA Device for AWS GovCloud provided by SurePassID

### How can users access AWS?

- To access AWS, you have 3 options:
  - AWS Management Console (protected by password + MFA)
  - AWS Command Line Interface (CLI): protected by access keys
  - AWS Software Developer Kit (SDK) - for code: protected by access keys
- Access keys are generated through the AWS Console
- Users manage their access keys
- Access keys are secret, just like a password. **Don't share them.**

### What is AWS CLI?

- It's a tool that enables you to interact with AWS services using commands in your command-line shell
- Direct access to the public APIs of AWS services
- You can develop scripts to manage your resources
- It's open-source
- Alternative to using AWS Management Console

### What's the AWS SDK?

- AWS Software Development Kit
- Language-specific APIs (set of libraries)
- Enables you to access and manage AWS services programmatically
- Embedded within your application
- Supports:
  - SDKs (JavaScript, Python, PHP, .NET, Ruby, Java, Go, Node.js, C++)
  - Mobile SDKs (Android, iOS)
  - IoT Device SDKs (Embedded C, Arduino)
- AWS CLI is built on AWS SDK for Python

### IAM: Roles For Services

- Some AWS services will need to perform actions on your behalf
- To do so, we will assign permissions to AWS services with IAM roles

### IAM: Security Tools

- **IAM Credentials Report (account-level)**
  - It's a report that lists all your account's users and the status of their various Credentials
- **IAM Access Advisor (user-level)**
  - Access advisor shows the service permissions granted to a user and when those services were last accessed
  - You can use this information to revise your policies

### IAM: Guidelines & Best Practices

- Don't use the root account except for the AWS account setup
- One physical user = one AWS user
- **Assign users to groups** and assign permissions to groups
- Create a **strong password policy**
- Use and enforce the user of **Multi-Factor Authentication (MFA)**
- Create and use **roles** for giving permissions to AWS services
- Use Access Keys for Programmatic Access (CLI/SDK)
- Audit permissions of your account using the IAM Credentials Report & IAM Access Advisor
- Never share IAM users & Access Keys

### Shared Responsibility Model for IAM

- **AWS:**
  - Infrastructure (global network security)
  - Configuration and vulnerability analysis
  - Compliance validation
- **You:**
  - Users, Groups, Roles, Policies management, and monitoring
  - Enable MFA on all Accounts
  - Rotate all your keys often
  - Use IAM tools to apply for appropriate permissions
  - Analyze access patterns & review permissions

<br>

## EC2 (Elastic Compute Cloud)

- EC2 is one of the most popular AWS' offering
- EC2 is an IaaS
- It mainly consists of the capability of:
  - Renting virtual machines (EC2)
  - Storing data on virtual drives (EBS)
  - Distributing load across machines (ELB)
  - Scaling the services using an auto-scaling group (ASG)
- Knowing EC2 is essential to understanding how the Cloud works

### EC2: Sizing & Configuration Options

- **Operating System (OS):** Linux, Windows, or Mac OS
- How much compute power & cores **(CPU)**
- How much random-access memory **(RAM)**
- How much storage space:
  - Network-attached (EBS & EFS)
  - Hardware (EC2 Instance Store)
- Network card: Speed of the card, public IP address
- Firewall rules: **security group**
- Bootstrap script (configure at first launch): EC2 User Data

### EC2: User Data

- It is possible to bootstrap our instances using an **EC2 User Data** script
- **Bootstraping** means launching commands when a machine starts
- That script is **only run once** at the instance **first start**
- EC2 user data is used to automate boot tasks such as:
  - Installing updates
  - Installing software
  - Downloading common files from the internet
  - Anything you can think of
- The EC2 User Data Script runs with the root user

### EC2: Instance types

- You can use different types of EC2 instances that are optimised for different use Cases (https://aws.amazon.com/ec2/instance-types/)
- AWS has the following naming convention:
  - m5.2xlarge
  - **m:** instance class
  - **5:** generation of the instance(AWS improves them over time)
  - **2xlarge:** size within the instance class

### EC2: Instance types - General Purpose

- Great for a diversity of workloads such as web servers or code repositories
- Balance between:
  - Compute
  - Memory
  - Networking
- The **t2.micro** is a general purpose EC2 instance

### EC2: Instance types - Compute Optimized

- Great for compute-intensive tasks that require high-performance processors:
  - Batch processing workloads
  - Media transcoding
  - High-performance web servers
  - High-performance computing (HPC)
  - Scientific modeling & Machine Learning
  - Dedicated gaming servers

### EC2: Instance types - Memory Optimized

- Fast performance for workloads that process large data sets in memory
- Use cases:
  - High-performance, relational/non-relational databases
  - Distributed web-scale cache stores
  - In-memory databases optimized for BI (Business Intelligence)
  - Applications performing real-time processing of big unstructured data

### EC2: Instance types - Storage Optimized

- Great for storage-intensive tasks that require high, sequential read and write access to large data sets on local storage
- Use cases:
  - High-frequency online transaction processing (OLTP) systems
  - Relational & NoSQL databases
  - Cache for in-memory databases (for example, Redis)
  - Data warehousing applications
  - Distributed file systems

### Security Groups & Classic Ports

- Security Groups are fundamental to network security in AWS
- They control how traffic is allowed into or out of our EC2 instances
- Security groups only contain **allow** rules
- Security groups rules can reference by IP or by security group
- Security groups are acting as a "firewall" on EC2 instances
- They regulate:
  - Access to Ports
  - Authorised IP ranges - IPv4 and IPv6
  - Control of inbound network (from other to the instance)
  - Control of outbound network (from the instance to other)

### Security Groups (The Good to Knows)

- Can be attached to multiple instances
- Locked down to a region / VPC combination
- It lives "outside" the EC2 - If traffic is blocked the EC2 instance won't see
- It's good to maintain one separate security group for SSH access
- If your application is not accessible **(time out)**, then it's a security group issue
- If your application gives a **"connection refused"** error, then it's an application error or it's not launched
- All inbound traffic is **blocked** by default
- All outbound traffic is **authorised** by default

### Classic Ports to Knowing

- **22 = SSH** (Secure Shell) - log into a Linux instance
- **21 = FTP** (File Transfer Protocol) - upload files into a file share
- **22 = SFTP** (Secure File Transfer Protocol) - upload files using SSH
- **80 = HTTP** - access unsecured websites
- **443 = HTTPS** - access secured websites
- **3389 = RDP** (Remote Desktop Protocol) - log into a windows instance

### SSH Overview

|               | SSH     | Putty   | EC2 Instance Connect |
| ------------- | ------- | ------- | -------------------- |
| Mac           | &#9745; | &#9744; | &#9745;              |
| Linux         | &#9745; | &#9744; | &#9745;              |
| Windows < 10  | &#9744; | &#9745; | &#9745;              |
| Windows >= 10 | &#9745; | &#9745; | &#9745;              |

- SSH is one of the most important functions. It allows you to control a remote machine, all using the command line

### EC2: Instances Purchasing Options

- **On-demand instances:** short workload, predictable pricing, pay by second
- **Reserved (1 & 3 years)**:
  - Reserved Instances - long workloads
  - Convertible Reserved Instances - long workloads with flexible instances
- **Savings Plan (1 & 3 years)** - commitment to an amount of usage, long workload
- **Spot Instances:** short workloads, cheap, can lose instances (less reliable)
- **Dedicated Hosts:** book an entire physical server, control instance placement
- **Dedicated Instances:** no other customers will share your hardware

**(The discount % in the following section changes frequently and they aren't essential to passing the AWS Cloud Practitioner Exam)**

### EC2: On Demand

- Pay for what you use:
  - Linux or Windows - billing per second, after the first minute
  - All other operating systems - billing per hour
- Has the highest cost but no upfront payment
- No long-term commitment
- Recommended for **short-term** and **un-interrupted workloads**, where you can't predict how the application will behave

### EC2: Reserved Instances

- Up to 72% discount compared to On-demand
- You reserve specific instance attributes (Instance Type, Region, Tenancy, OS)
- **Reservation Period** - **1 year** (+discount) or 3 years (+++discount)
- **Payment options** - No Upfront (+), Partial Upfront (++), All Upfront (+++)
- **Reserved Instance's Scope** - Regional or Zonal (reserve capacity in an AZ)
- Recommended for steady-state usage applications (think database)
- You can buy and sell in the reserved instance marketplace
- **Convertible Reserved Instance**
  - Can change the EC2 instance type, instance family, OS, scope, and tenancy

### EC2: Savings Plan

- Get a discount based on long-term usage (up to 72% - same as RIs)
- Commit to a certain type of usage ($10/hour for 1 or 3 years)
- Usage beyond the EC2 savings plan is billed at the on-demand Prices
- Locked to specific instance family & AWS region
- Flexible across:
  - Instance size
  - OS
  - Tenancy (Host, Dedicated, Default)

### EC2: Spot Instances

- Can get a discount of up to 90% compared to on-demand
- Instances that you can "lose" at any point in time if your max price is less than the current spot price
- The **MOST cost-efficient** instances in AWS
- **Useful for workloads that are resilient to failure**

  - Batch jobs
  - Data analysis
  - Image processing
  - Any **distributed** workloads
  - Workloads with a flexible start and end time

- **NOT suitable for critical jobs or databases**

### EC2: Dedicated Hosts

- A physical server with EC2 instance capacity fully dedicated to your use
- Allows you to address **compliance requirements** and **use your existing server-bound software licenses** (per-socket, per-core, per-VM software licenses)
- Purchasing options:
  - **On-demand** - pay per second for active Dedicated Host
  - **Reserved** - 1 or 3 years (no upfront, partial upfront, all upfront)
- The most expensive option
- Useful for software that has a complicated licensing model (BYOL - bring your own license)
- Or for companies that have strong regulatory or compliance needs

### EC2: Dedicated Instances

- Instances run on hardware that's dedicated to you
- May share hardware with other instances in same account
- No control over instance placement (can move hardware after Stop/Start)

### EC2: Capacity Reservations

- Reserve **On-Demand** instances capacity in a specific AZ for any duration
- You have access to EC2 capacity when you need it
- **No time commitment** (create/cancel anytime), **no billing discounts**
- Combine with regional reserved instances and savings plan to benefit from billing discounts
- You're charged at on-demand rate whether you run instances or not
- Suitable for short-term, uninterrupted workloads that needs to be in a specific AZ

### Which purchasing option is right for me?

- Let's take an example of a resort:
  - **On demand:** coming and staying in resort whenever we like, we pay the full price
  - **Reserved:** like planning ahead and if we plan to stay for a long time, we may get a good discount
  - **Savings Plans:** pay a certain amount per hour for certain period and stay in any room type (King, Suite, Sea View)
  - **Spot Instances:** The resort allows people to bid for the empty rooms and the highest bider keeps the rooms. You can get kicked out at any time
  - **Dedicated Hosts:** We book an entire building of the resort
  - **Capacity Reservations:** You book a room for a period with full price even you don't stay in it
