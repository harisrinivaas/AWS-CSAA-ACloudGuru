This repo will house coursework from the AWS training class from A Cloud Guru for the Solutions Architect Associate Certification as well as course notes.

# Section 2: AWS - 10,000 Feet Overview

This section will cover a top-level overview on the AWS services tested in the Solutions Architect exam.

* AWS officially launched in 2006
* By the numbers, AWS services have grown from 82 in 2011 to over 1300+ in 2017

### Terminology
* What is a Region? A Region is a physical location in the world which consists of two or more AZ's
* What is an AZ? An AZ (Availability Zone) is simply a data center
* What is an Edge Location? Edge Locations are endpoints for AWS which are used for caching content. Typically this consists of CloudFront, Amazon's CDN (Content Delivery Network)

### Compute Service
* EC2 (Elastic Compute Cloud) - Virtual machines inside the AWS platform
* EC2 container service - Run and manage Docker containers at scale
* Elastic Beanstalk - For developers who do not understand AWS who just want to upload their code
* Lambda - A code uploaded to the cloud where you can control when it executes (no need to worry about physical or virtual machine)
* Lightsail - Amazon's VPN (virtual private network) service essentially a watered-down version of EC2
* Batch - Used for batch computing in the cloud

### Storage Service
* S3 (Simple Storage Service) - An object based- storage where we can upload files into buckets in the cloud
* EFS (Elastic File System) - A network-attached service
* Glacier - Data archival service
* Snowball - Way to bring in large amounts of data into the AWS data center
* Storage Gateway - Virtual Machines which will replicate information back to S3

### Database Services
* RDS (Relational Database Service) - Service which works with MySQL, PostgreSQL, Oracle
* DynamoDB - For non-relational databases
* ElastiCache - A way of caching commonly queried items from a database
* Redshift - Built for data warehousing

### Migration Services
* AWS Migration Hub - Tracking service which allows application tracking during migration
* Application Discovery Service - Automated set of tools which not only detects what applications we have but also tracks the dependencies for our application
* Database Migration Service - A way to visualize migrations in action
* Server Migration Service - Helps migrate physical and virtual servers to the cloud
* Snowball - Also a migration tool as well as a storage service

### Networking & Content Delivery
* VPC (Virtual Private Cloud) - Essentially a virtual data center where we can configure things such as firewalls, AZ's, etc.
* CloudFront - Stores information closer to the users and uses a CDN to distribute content on a global scale
* Route 53 - Amazon's DNS service which is highly scaleable
* API Gateway - Is a way of creating our own APIs for our services to talk to
* Direct Connect - A way of running a dedicated line from a data center into Amazon which will directly connect into a VPC

### Developer Tools
* CodeStar - Project management service
* CodeCommit - Source control service or place to store code
* CodeBuild - Once service is ready, this service will compile, run tests, and produce software packages which will enable deployment
* CodeDeploy - Service which automates deployments to EC2 instances, on premise instances, and lambda functions for example
* CodePipeline - Continuous delivery pipeline which will automate the steps required to release software
* X-Ray - Debug service which will help find root causes and performance bottlenecks
* Cloud9 - IDE environment which will allow development on the cloud

### Management Tools
* CloudWatch - Monitoring service
* CloudFormation - Way of scripting infrastructure
* CloudTrail - Used to log changes to the AWS environment (turned on by default and stores logs for a week)
* Config - Monitors the entire AWS environment
* OpsWorks - Similar to Elastic Beanstalk but more robust and is good tool to automate environments
* Service Catalog - A way of managing catalogs of IT services which are approved to use on AWS
* Systems Manager - A resource manager, typically used for EC2
* Trusted Advisor - Will give advice across multiple disciplines
* Managed Services - A manage service for things such as EC2 instances and auto scaling

### Media Services
* Elastic Transcoder - Resizes videos to be compatible on multiple platforms
* MediaConvert - File-based video transcoding service with broadcast grade features
* MediaLive - Broadcast grade video processing service
* MediaPackage - Prepares and protects videos for delivery over the internet
* MediaStore - Storage service optimized for media
* MediaTailor - Allows the ability to do ads on broadcast grade media

### Machine Learning
* SageMaker - Makes it easy to use deep learning
* Comprehend - Sentiment analysis around data
* DeepLens - Artificially aware camera
* Lex - A way of communicating with customers
* Machine Learning - Service to build machine learning projects
* Polly - Takes text and turns it into speech
* Rekognition - Recognizes objects of interest in images and videos
* Amazon Translate - Translation service
* Amazon Transcribe - Transcribe service

### Analytics
* Athena - Allows SQL queries or files in S3 bucket
* EMR (Elastic Map Reduce) - Used for processing large amounts of data
* CloudSearch - Search service for AWS
* ElasticSearch Service - Search service for AWS
* Kinesis - A way of ingesting large amounts of data into AWS
* Kinesis Video Streams - Allows ingesting of large amounts of data from video streams
* QuickSight - Amazon's business intelligence tool
* Data Pipeline - A way of moving data between different AWS services
* Glue - Used for ETL (Extract Transform and Load)

### Security & Identity & Compliance
* IAM (Identity Access Management) - Amazon's IAM service
* Cognito - Device authentication service
* GuardDuty - Monitors for malicious activity on the AWS account
* Inspector - An agent installed on services such as EC2 to check vulnerabilities
* Macie - Scan S3 buckets for PII (Personal Identity Info)
* Certificate Manager - Way of managing SSL certificates
* CloudHSM - Service which offers dedicated bits of hardware used to store keys
* Directory Service - Way of integrating Microsoft active directory services with AWS services
* WAF (Web Application Firewall) - A layer 7 firewall which stops cross-site scripting or SQL injections
* Shield - Service which helps mitigate DDoS attacks
* Artifact - Portal service which allows downloads of compliance reports

### Mobile Services
* Mobile Hub - Management console for mobile apps
* Pinpoint - Uses targeted push notifications to drive mobile engagement
* AWS AppSync - Updates data in web and mobile applications in real-time
* Device Farm - A way of testing apps on real-life devices
* Mobile Analytics - Analytics service for mobile

### AR/VR
* Sumerian - Used for AR, VR and 3D application design, allows you to use a common set of tools to create environments

### Application Integration
* Step Functions - A way of managing different Lambda functions
* Amazon MQ - A way of queuing messages
* SNS (Simple Notification Service) - Notification service if an account goes over some limit
* SQS (Simple Queue Service) - Queue service which is used for decoupling infrastructure
* SWF (Simple Workflow Service) - Workflow service which creates a workflow map for some processes

### Customer Engagement
* Connect - Essentially is a call center in the cloud
* Simple Email Service - Very scaleable service which helps send emails to customers

### Business Productivity
* Alexa For Business - Can use for a variety of business services and tasks
* Chime - Video conferencing similar to Google hangout
* WorkDocs - A drop box for AWS
* WorkMail - Similar to Office 365

### Desktop & App Streaming
* Workspaces - A VDI (virtual desktop infrastructure) solution (running an operating system on AWS cloud)
* AppStream 2.0 - A way to actually stream applications to your desktop

### Internet of Things
* iOT - A way of having thousands or millions of devices sending back data i.e. sensor data such as temperature or humidity to a controller
* iOT Device Management - Used for managing a ton of devices through the AWS service
* Amazon FreeRTOS - Operating system service for microcontrollers
* Greengrass - Software that lets your run local compute, messaging, data caching, sync, and ML inference capabilities for connected devices in a secure way

### Game Development
* GameLift - Service to help develop games in the AWS cloud

## Section 2 Quiz

**1. What is an AWS region?**
* A region is a geographic area that consists of different AZ's. Each region has at least two AZ's.

**2. What does an AWS region consist of?**
* An independent collection of AWS computing resources in a defined geography.

**3. Which statement best describes AZ's?**
* Distinct locations from within an AWS region that are engineered to be isolated form failures.

**4. An AWS VPC is a component of which AWS service?**
* Networking Service

**5. What is a VPC?**
* Virtual Private Cloud

**6. Which AWS service is specifically designed to run a developer's code on an infrastructure that is automatically provisioned to host that code?**
* Elastic Beanstalk

**7. Which AWS service allows you to run code without having to worry about provisioning any underlying resources (such as virtual machines, databases, etc.)**
* Lambda

**8. Amazon's highly scaleable DNS service is known as ________.**
* Route 53

**9. Which AWS compute service is specifically designed to assist you in processing large data sets?**
* Elastic Map Reduce

**10. What is the difference between Elastic Beanstalk & CloudFormation?**
* Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring based on the code you upload to it, where as CloudFormation is an automated provisioning engine designed to deploy entire cloud environments via a JSON script.

**11. Which AWS service uses a CDN to distribute content around the world?**
* CloudFront

**12. Which of the following AWS solutions offers durable, available storage for flat files?**
* S3

**13. Which of the following AWS services would be the best choice for long term data archival?**
* Glacier

**14. Which AWS service offers the following database engines: SQL, MySQL, MariaDB, PostgreSQL, Aurora, and Oracle?**
* RDS

**15. Which of the following AWS services is used primarily for data warehousing?**
* Redshift

**16. Which AWS service is used for collating large amounts of data streamed from multiple sources?**
* Kinesis

**17. You need to add users to your AWS account and set password rotation policies for these new users. Which AWS service would best fit your requirements?**
* IAM

**18. You need to supply auditors with logs detailing the individual users that provision specific resources on your AWS platform. Which service would best meet this need?**
* CloudTrail

**19. You need a configuration management service that enables your system administrators to configure and operate your web applications using Chef. Which AWS service would best suit your needs?**
* Opsworks

**20. Your digital media agency needs to convert their media files in to different formats to suit different devices. Which AWS service should you consider using to meet these needs?**
* Elastic Transcoder

---

# Section 3: Identity Access Management (IAM)

This section will cover an in-depth overview on the IAM service.

### IAM Overview
* Centralized control of your AWS account
* Shared Access to your AWS account
* Identity Federation (including Active Directory, Facebook, LinkedIn, etc.)
* Multifactor Authentication
* Provide temporary access for users/devices and services where necessary
* Allows you to set up your own password rotation policy
* Integrates with many different AWS services
* Supports PCI DSS Compliance

### Critical Terms
* Users - End Users
* Groups - A collection of users under one set of permissions
* Roles - You create roles and can then assign them to AWS resources
* Policies - A document that defines one (or more permissions)

### IAM - Lab
* IAM does not have a region as it is global
Steps to set up IAM on AWS are as follows:
 1. Delete root access keys
 2. Activate MFA on root account
 3. Create individual IAM users
 4. Use groups to assign permissions
 5. Apply an IAM password policy
* IAM roles are a secure way to grant permissions to entities that you trust.

### Create a Billing Alarm - Lab
* We can create a billing alarm by navigating to CloudWatch and configuring alarms for billing

### What Have We Learned?
* IAM consists of the following:
 1. Users
 2. Groups
 3. Roles
 4. Policy Documents
* IAM is universal, it does not apply to regions at this time
* The "root account" is simply the account created on AWS account setup. This account has complete Admin access
* New users have no permissions when first created
* New users are assigned Access Key ID and Secret Access Keys when first created
* Access Key ID & Secret Access Keys are not the same as a password and you cannot use them to login to the console. You can use these keys to access AWS via the APIs and CLI however
* You only get to view the Access Key ID & Secret Access Keys once. If lost will need to be regenerated.
* Always setup MFA (Multifactor Authentication) on the root account
* It is possible to create and customize the password rotation policies

## Section 3 Quiz

**1. Which statement best describes IAM**
* IAM Allows you to manage users, groups, roles, and their corresponding level of access to the AWS platform

**2. Which of the following is NOT a feature of IAM?**
* Allows you to set biometric authentication, so that no passwords are required

**3. Power User Access allows ___**
* Access to all AWS services except for management of groups and users within IAM

**4. What level of access does the "root" account have?**
* Administrator Access

**5. You are a solutions architect working for a large engineering company who are moving their existing legacy hardware to AWS. You have configured their first AWS account and you have set up IAM. Your company will be primarily based out of West Germany, however they will have a small subsidiary operating out of South Korea and you will need an AWS environment configured there as well. Which of the following statements is true;**
* You will need to configure Users and Policy Documents only once, as these are applied globally

**6. You have a client who is considering moving to AWS services and do not yet have an account. What is the first thing the company should do to set up an AWS Account?**
* Set up an account using their company email address

**7. You are a security administrator working for a hotel chain. You have a new member of staff who has started as a systems administrator and they will need full access to the AWS console. You have created the user account and generated the access key id and the secret access key. You have moved this user into the group where the other administrators are and you have provided the new user with their secret access key and their access key id. However when they go to log in to the AWS console, they cannot sign in. What could be the cause of this?**
* You cannot log in to the AWS console using the Access Key ID and Secret Access Key, instead you must generate a password for the user and supply the user with this password, as well as the unique link to sign in to the AWS console

**8. What is an additional way to secure IAM for both the root login and new users alike?**
* Implement MFA for all accounts

**9. By default when you create a new user in the IAM console, what level of access do they have?**
* No access to all AWS services

**10. In what language are policy documents written in?**
* JSON

---

# Section 4: AWS Object Storage and CDN - S3, Glacier and CloudFront

This section will cover an in-depth overview on the S3 (Simple Storage Service) service.

### What is S3?
* S3 provides developers and IT teams with secure, durable, highly-scalable object storage. Amazon S3 is easy to use, with a simple web services interface to store and retrieve any amount of data from anywhere on the web
* S3 is a safe place to store your files
* S3 is an object-based storage
* The data is spread across multiple devices and facilities

### S3 - The Basics
* S3 is Object-based - i.e. allows you to upload files
* Files can be from 0 Bytes to 5 TB
* There is unlimited storage
* Files are stored in Buckets
* S3 is a universal namespace - names must be unique globally
* URLs look like https://s3-eu-west-1.amazonaws.com/<name>
* When you upload a file to S3 you will receive a HTTP 200 code if the upload was successful

### Data Consistency Model for S3
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)

### S3 is a Simple Key-value Store
Objects consist of the following:
 * Key (this is the name of the object)
 * Value (this is the data and is made up of a sequence of bytes)
 * Version ID (important for versioning)
 * Metadata (Data about data you are storing)
 * Sub resources:
    * Access Control Lists
    * Torrent

### S3 - The Basics (Continued)
* Built for 99.99% availability for the S3 platform.
* Amazon guarantee 99.9% availability
* Amazon guarantee 99.99999999999% durability for S3 information (11 x 9s)
* Tiered storage available
* Lifecycle Management
* Versioning
* Encryption
* Secure your data using Access Control Lists and Bucket Policies

### S3 - Storage Tiers/Classes
* S3 Standard: 99.99% availability, 99.9999999999% durability, stored redundantly across multiple devices in multiple facilities, and is designed to sustain the loss of 2 facilities concurrently
* S3 - IA: (Infrequently Accessed): For data that is accessed less frequently, but requires rapid access when needed. Lower fee than S3 but you are charged a retrieval fee
* S3 One Zone - IA: Want a lower-cost option for infrequently accessed data but do not require the multiple AZ data resilience
* Glacier: Very cheap but used for archival only. Expedited, Standard or Bulk. A standard retrieval time takes 3-5 hours

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/s3-storage-tiers.jpg">
  <h3>Figure 4-1. S3 Storage classes and info</h3>
</div>

### S3 - Charges
In S3, we are charged for:
* Storage
* Requests
* Storage Management Pricing
* Data Transfer Pricing
* Transfer Acceleration

### What is S3 Transfer Acceleration?
AWS S3 Transfer Acceleration enables fast, easy, and secure transfers of files over long distances between your end users and an S3 bucket. Transfer Acceleration takes advantage of AWS CloudFront's globally distributed edge locations. As the data arrives at an edge location, data is routed to AWS S3 over an optimized network path.

### Create and S3 Bucket - Exam Tips
* Buckets are a universal name space
* Upload an object to S3 receives a HTTP 200 code on success
* S3, S3-IA, S3 Reduced Redundancy Storage
* Encryption
  * Client Side Encryption
  * Server Side Encryption
    * Server side encryption with Amazon S3 Managed Keys (SSE-S3)
    * Server side encryption with KMS (SSE-KMS)
    * Server side encryption with Customer Provided Keys (SSE-C)
* Control access to buckets using either a bucket ACL or using Bucket Policies
* **By default buckets are private and all objects stored inside them are private**

### S3 - Versioning Exam Tips
* Stores all versions of an object (including all writes and even if you delete an object)
* Great backup tool
* Once enabled, versioning cannot be disabled, only suspended
* Integrates with Lifecycle rules
* Versioning's MFA Delete capability, which uses multi-factor authentication, can be used to provide an additional layer of security

### S3 - Cross Region Replication Exam Tips
* Versioning must be enabled on both the source and destination buckets
* Regions must be unique
* Files in an existing bucket are not replicated automatically. All subsequent updated files will be replicated automatically
* You cannot replicate to multiple buckets or use daisy chaining
* Delete markers are replicated
* Deleting individual versions or delete markers will not be replicated
* Understand what Cross Region Replication is at a high level

### S3 - Lifecycle Management Lab
* Can be used in conjunction with versioning
* Can be applied to current versions and previous versions
* Following actions can now be done:
  * Transition to the Standard - Infrequent Access Storage Class (30 days after creation date)
  * Archive to the Glacier Storage Class (30 days after IA)
  * Permanently Delete

### What is a CDN?
A CDN (content delivery network) is a system of distributed servers (network) that delivers webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage and a content delivery server.

### CloudFront - Key Terms
* Edge Location - The location where content will be cached. This is separate to an AWS region/AZ
* Origin - The origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 Instance, and Elastic Load Balancer or Route 53
* Distribution - The name given the CDN which consists of a collection of Edge Locations

### What is CloudFront?
Amazon CloudFront can be used to deliver your entire website, including dynamic, static, streaming, and interactive content using a global network of edge locations. Requests for your content are automatically routed to the nearest edge location, so content is delivered with the best possible performance.

Amazon CloudFront is optimized to work with other services such as S3, EC2, Elastic Load Balancing, and Route 53. CloudFront also works seamlessly with any non-AWS origin server, which stores the original, definitive versions of your files.

### CloudFront - Key Terms (Continued)
* Web Distribution - Typically used for websites
* RTMP - Used for media streaming

### CloudFont - Exam Tips
* Understand the key terms: Edge Location, Origin, Distribution, Web Distribution, and RTMP
* Edge locations are not just READ only, you can write to them too
* Objects are cached for the life of the TTL (time to live)
* You can clear cached objects but you will be charged

### Securing your buckets
* By default, all newly created buckets are **private**
* You can setup access control to your buckets using:
  * Bucket Policies
  * Access Control Lists
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket

### Encryption
There are four types of Encryption for S3:
* In transit:
  * SSL/TLS
* At rest:
  * Server Side Encryption
    * S3 Managed Keys - SSE-S3
    * AWS Key Managed Service, Managed Keys - SSE-KMS
    * Server Side Encryption with Customer Provided Keys - SSE-C
  * Client Side Encryption

### Storage Gateway
AWS Storage Gateway is a service that connects an on-premises software appliance with cloud-based storage to provide seamless and secure integration between an organization's on-premises IT environment and AWS's storage infrastructure. The service enables you to securely store data to the AWS cloud for scalable and cost-effective storage.

AWS Storage Gateway's software appliance is available for download as a VM (virtual machine) image that you install on a host in your data center. Storage Gateway supports either VMware ESXi or Microsoft Hyper-V. Once you've installed your gateway and associated it with your AWS account through the activation process, you can use the AWS Management Console to create the storage gateway option that is right for you.

### Four Types of Storage Gateways
* File Gateways (NFS)
* Volumes Gateway (iSCSI)
  * Stored Volumes
  * Cached Volumes
* Tape Gateway (VTL)

### File Gateway
Files are stored as objects in your S3 buckets, accessed through a Network File System (NFS) mount point. Ownership, permissions, and timestamps are durably stored in S3 in the user-metadata of the object associated with the file. Once objects are transferred to S3, they can be managed as native S3 objects, and bucket policies such as versioning, lifecycle management, and cross-region replication apply directly to objects stored in your bucket.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/s3-file-gateway.jpg">
  <h3>Figure 4-2. Sample S3 file gateway architecture</h3>
</div>

### Volume Gateway
The volume interface presents your applications with disk volumes using the iSCSI block protocol

Data written to these volumes can be asynchronously backed up as point-in-time snapshots of your volumes, and stored in the cloud as Amazon EBS snapshots.

Snapshots are incremental backups that capture only changed blocks. All snapshot storage is also compressed to minimize your storage charges.

### Volume Gateway - Stored Volumes
Stored volumes let your primary data locally, while asynchronously backing up that data to AWS. Stored volumes provide your on-premises applications with low-latency access to their entire datasets, while providing durable, off-site backups. You can create storage volumes and mount them as iSCSI devices from your on-premises application servers. Data written to your stored volumes is stored on your on-premises storage hardware. This data is asynchronously backed up to S3 in the form of EBS (Amazon Elastic Block Store) snapshots. 1GB - 16 TB in size for Stored Volumes.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-stored-volumes.jpg">
  <h3>Figure 4-3. Sample S3 volume gateway stored volumes architecture</h3>
</div>

### Volume Gateway - Cached Volumes
Cached volumes let you use S3 as your primary data storage while retaining frequently access data locally in your storage gateway. Cached volumes minimize the need to scale your on-premises storage infrastructure, while still providing your applications with low-latency access to their frequently accessed data. You can create storage volumes up to 32 TB in size and attached to them as iSCSI devices from your on-premises application servers. Your gateway stores data that you write to these volumes in S3 and retains recently read data in your on-premises storage gateway's cache and upload buffer storage. 1 GB - 32 TB in size for Cache Volumes

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-cached-volumes.jpg">
  <h3>Figure 4-4. Sample S3 volume gateway cached volume architecture</h3>
</div>

### Volume Gateway - Tape Gateway
Tape Gateway offers a durable, cost-effective solution to archive your data in the AWS Cloud. The VTL interface it provides lets your leverage your existing tape-based backup application infrastructure to store data on virtual tape cartridges that you create on your tape gateway. Each tape gateway is preconfigured with a media changer and tape drives, which are available to your existing client backup applications as ISCSI devices. You add tape cartridges as your need to archive your data. Supported by NetBackup, Backup Exec, Veeam etc.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-tape-gateway.jpg">
  <h3>Figure 4-5. Sample S3 volume gateway tape gateway architecture</h3>
</div>

### Storage Gateway - Exam Tips
* File Gateway - For flat files, stored directly on S3
* Volume Gateway:
  * Stored Volumes - Entire dataset is stored on site and is asynchronously backed up to S3
  * Cached Volumes - Entire dataset is stored on S3 and the most frequently accessed data is cached on site
* Gateway Virtual Tape Library (VTL)
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam etc.

### Import/Export Disk
AWS Import/Export Disk accelerates moving large amounts of data into and out of the AWS cloud using portable storage devices for transport. AWS Import/Export Disk transfers your data directly onto and off of storage devices using Amazon's high-speed internal network and bypassing the Internet.

### Types of Snowballs
* Snowball
* Snowball Edge
* Snowmobile

### Snowball
* Snowball is a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of AWS. Using Snowball addresses common challenges with large-scale data transfers including high network costs, long transfer times, and security concerns. Transferring data with Snowball is simple, fast, secure, and can be as little as one-fifth the cost of high-speed Internet.

80 TB snowball in all regions. Snowball uses multiple layers of security designed to protect your data including tamper-resistant enclosures, 256-bit encryption, and an industry-standard Trusted Platform Module (TPM) designed to ensure both security and full chain-of-custody of your data. Once the data transfer job has been processed and verified, AWS performs a software erasure of the Snowball appliance.

### Snowball Edge
AWS Snowball Edge is a 100 TB data transfer device with on-board storage and compute capabilities. You can use Snowball Edge to move large amounts of data into and out of AWS, as a temporary storage tier for large local datasets, or to support local workloads in remote or offline locations.

Snowball Edge connects to your existing applications and infrastructure using standard storage interfaces, streamlining the data transfer process and minimizing setup and integration. Snowball Edge can cluster together to form a local storage tier and process your data on-premises, helping ensure your applications continue to run even when they are not able to access the cloud.

### Snowmobile
AWS Snowmobile is an Exabyte-scale data transfer service used to move extremely large amounts of data to AWS. You can transfer up to 100 PB per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi-trailer truck. Snowmobile makes it easy to move massive volumes of data to the cloud, including video libraries, image repositories, or even a complete data center migration. Transferring data with Snowmobile is secure, fast, and cost effective.

### Snowball - Exam Tips
* Understand what Snowball is
* Understand what Import/Export is
* Snowball can:
  * Import to S3
  * Export to S3

### What is S3 Transfer Acceleration?
S3 Transfer Acceleration utilizes the CloudFront Edge Network to accelerate your uploads to S3. Instead of uploading directly to your S3 bucket, you can use a distinct URL to upload directly to an edge location which will then transfer that file to S3. You will get a distinct URL to upload to.

### Summary
* Know the core fundamentals of S3:
  * Key (name)
  * Value (data)
  * Version ID
  * Metadata
  * Access control lists
* Object based storage only (for files)
* **Not suitable to install an operating system on**
* Remember that S3 is Object based i.e. allows you to upload files
* Files can be from 0 bytes to 5 TB
* There is unlimited storage
* Files are stored in buckets
* S3 is a universal namespace, that is, names must be unique globally
* Sample URL: https://s3-eu-west-1.amazonaws.com/<name>
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)

#### Summary - S3 Storage Tiers/Classes
* Know the different storage tiers/classes:
  * S3 Standard
  * S3-IA
  * S3 One Zone-IA
  * Glacier

#### Summary - S3 Versioning
* Stores all versions of an object (including all writes and even if you delete an object)
* Great backup tool
* Once enabled, cannot be disabled, only suspended
* Integrates with Lifecycle rules
* Versioning's MFA Delete capability, which uses multi-factor authentication, can be used to provide an additional layer of security
* Cross Region Replication, requires versioning enabled on the source bucket

#### Summary - S3 Lifecycle Management
* Can be used in conjunction with versioning
* Can be applied to current versions and previous versions
* Following actions can now be done:
  * Transition to the Standard - Infrequent Access Storage Class (128 Kb and 30 days after the creation date)
  * Archive to the Glacier Storage Class (30 days after IA, if relevant)
  * Permanently Delete

#### Summary - CloudFront
* Edge Location - This is the location where content will be cached. This is separate to an AWS AZ
* Origin - This is the origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 Instance, an Elastic Load Balancer or Route 53
* Distribution - This is the name given the CDN which consists of a collection of Edge Locations. There are different types:
  * Web Distribution - Typically used for websites
  * RTMP - Used for media streaming
* Edge locations are not just READ only, you can write to them too
* Objects are cached for the life of the TTL (Time to Live)
* You can clear cached objects but you will be charged

#### Summary - Securing your buckets
* By default, all newly created buckets are PRIVATE
* You can setup access control to your buckets using:
  * Bucket Policies
  * Access Control Lists
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket

#### Summary - Encryption
* In Transit:
  * SSL/TLS
* At Rest:
  * Server Side Encryption
    * S3 Managed Keys - SSE-S3
    * AWS Key Management Service, Managed Keys - SSE-KMS
    * Server Side Encryption with Customer Provided Keys - SSE-C
  * Client Side Encryption

#### Summary - Storage Gateway
* File Gateway - For flat files, stored directly on S3
* Volume Gateway:
  * Stored Volumes - Entire dataset is stored on site and is asynchronously backed up to S3
  * Cached Volumes - Entire dataset is stored on S3 and the most frequently accessed data is cached on site
* Gateway Virtual Tape Library (VTL)
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam etc.

#### Summary - Snowball
Types of snowball:
* Snowball
* Snowball Edge
* Snowmobile

#### Summary - S3 Transfer Acceleration
* You can speed up transfers to S3 using S3 transfer acceleration. This costs extra and has the greatest impact on people who are in a faraway location

#### S3 Static Websites
* You can use S3 to host static websites
* Serverless
* Very cheap, scales automatically
* STATIC only, cannot host dynamic sites

#### Summary - Last Few Tips
* Write to S3 - HTTP 200 code for a successful write
* You can load files to S3 much faster by enabling multipart upload
* Read the S3 FAQ before taking the exam. It comes up A LOT!

## Section 4 Quiz

**1. S3 has what consistency model for PUTS of new objects**
* Read After Write Consistency

**2. What is AWS Storage Gateway?**
It's an on-premise virtual appliance that can be used to cache S3 locally at a customer’s site

**3. One of your users is trying to upload a 7.5GB file to S3 however they keep getting the following error message - "Your proposed upload exceeds the maximum allowed object size.” What is a possible solution for this?**
* Design your application to use the multi-part upload API for all objects

**4. What does RRS stand for when talking about S3?**
* Reduced Redundancy Storage

**5. You have been asked by your company to create an S3 bucket with the name "acloudguru1234" in the EU West region. What would be the URL for this bucket?**
* https://s3-eu-west-1.amazonaws.com/acloudguru1234

**6. What is Amazon Glacier?**
* An AWS service designed for long term data archival

**7. What does S3 stand for?**
* Simple Storage Service

**8. You are a solutions architect who works with a large digital media company. The company has decided that they want to operate within the Japanese region and they need a bucket called "testbucket" set up immediately to test their web application on. You log in to the AWS console and try to create this bucket in the Japanese region however you are told that the bucket name is already taken. What should you do to resolve this?**
* Bucket names are global, not regional. This is a popular bucket name and is already taken. You should choose another bucket name

**9. What is the availability on RRS?**
* 99.99%

**10. What is the durability on RRS?**
* 99.99%

**11. What is the durability on S3?**
* 99.999999999%

**12. What is the availability on S3?**
* 99.99%

**13. What is the minimum file size that I can store on S3?**
* 0 bytes

**14. The difference between S3 and EBS is that EBS is object based where as S3 is block based.
* False

**15. S3 has eventual consistency for which HTTP Methods?**
* Overwrite PUTS and Deletes

**16. You work for a busy digital marketing company who currently store their data on premise. They are looking to migrate to AWS S3 and to store their data in buckets. Each bucket will be named after their individual customers, followed by a random series of letters and numbers. Once written to S3 the data is rarely changed, as it has already been sent to the end customer for them to use as they see fit. However on some occasions, customers may need certain files updated quickly, and this may be for work that has been done months or even years ago. You would need to be able to access this data immediately to make changes in that case, but you must also keep your storage costs extremely low. The data is not easily reproducible if lost. Which S3 storage class should you choose to minimize costs and to maximize retrieval times?**
* S3-IA

**17. You need to use an Object based storage solution to store your critical, non-replaceable data in a cost effective way. This data will be frequently updated and will need some form of version control enabled on it. Which S3 storage solution should you use?**
* S3

**18. You work for a health insurance company who collects large amounts of documents regarding patients’ health records. This data will be used usually only once when assessing a customer and will then need to be securely stored for a period of 7 years. In some rare cases you may need to retrieve this data within 24 hours of a claim being lodged. Which storage solution would best suit this scenario? You need to keep your costs as low as possible.**
* Glacier

**19. You run a meme creation website that frequently generates meme images. The original images are stored in S3 and the meta data about the memes are stored in DynamoDB. You need to store the memes themselves in a low cost storage solution. If an object is lost, you have created a Lambda function that will automatically recreate this meme using the original file in S3 and the metadata in DynamoDB. Which storage solution should you consider to store this non-critical, easily reproducible data on in the most cost effective solution as possible?**
* S3-RRS

**20. You run a popular photo sharing website that is based off S3. You generate revenue from your website via paid for adverts, however you have discovered that other websites are linking directly to the images on your site, and not to the HTML pages that serve the content. This means that people are not seeing your adverts and every time a request is made to S3 to serve an image it is costing your business money. How could you resolve this issue?**
* Remove the ability for images to be served publicly to the site and then use signed URLs with expiry dates

---

# Section 5: EC2 - The Backbone of AWS

This section will cover an in-depth overview on the AWS Elastic Compute Cloud (EC2) service.

### What is EC2?
Amazon EC2 (Elastic Cloud Compute) is a web service that provides resizable compute capacity in the cloud. Amazon EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.

EC2 changes the economics of computing by allowing you to pay only for capacity that you actually use. EC2 provides developers the tools to build failure resilient applications and isolate themselves from common failure scenarios.

### EC2 Options
* On Demand - Allows you to pay a fixed rate by the hour (or by the second) with no commitment
* Reserved - Provides you with a capacity reservation and offers a significant discount on the hourly charge for an instance. 1 year or 3 year terms
* Spot - Enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times
* Dedicated Hosts - Physical EC2 server dedicated for you use. Dedicated Hosts can help you reduce costs by allowing you to use your existing server-bound software licenses

### On Demand
* Perfect for users that want the low cost and flexibility of EC2 without any up-front payment or long-term commitment
* Applications with short term, spiky, or unpredictable workloads that cannot be interrupted
* Applications being developed or tested on EC2 for the first time

### Reserved
* Applications with steady state or predictable usage
* Applications that require reserved capacity
* Users can make up-front payments to reduce their total computing costs even further
  * Standard RIs (up to 75% off on-demand)
  * Convertible RIs (up to 54% off on-demand) feature the capability to change the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value
  * Schedule RIs are available to launch within the time window you reserve. This option allows you to match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, week, or month

### Spot
* Applications that have flexible start and end times
* Applications that are only feasible at very low compute prices
* Users with an urgent need for large amounts of additional computing capacity

### Dedicated Hosts
* Useful for regulatory requirements that may not support multi-tenant virtualization
* Great for licensing which does not support multi-tenancy or cloud deployments
* Can be purchased on-demand (hourly)
* Can be purchased as a Reservation for up to 70% off the on-demand price

### EC2 Instance Types

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/specialities-use-cases.jpg">
  <h3>Figure 5-1. EC2 instance types, specialties and use cases</h3>
</div>

### What is EBS?
Amazon EBS (Elastic Block Storage) allows you to create storage volumes and attach them to EC2 instances. Once attached, you can create a file system on top of these volumes, run a database, or use them in any other way you would use a block device. EBS volumes are placed in a specific AZ where they are automatically replicated to protect you from the failure of a single component.

### EBS Volume Types
* General Purpose SSD (GP2)
  * General purpose, balances both price and performance
  * Ratio of IOPS per GB with up to 10,000 IOPS and the ability to burst up to 300 IOPS for extended periods of time for volumes at 3334 GB and above
* Provisioned IOPS SSD (101)
  * Designed for I/O intensive applications such as large relational or NoSQL databases
  * Use if you need more than 10,000 IOPS
  * Can provision up to 20,000 IOPS per volume
* Throughput Optimized HDD (ST1)
  * Big data
  * Data warehouses
  * Log processing
  * Cannot be a boot volume
* Cold HDD (SC1)
  * Lowest cost storage for infrequently accessed workloads
  * File server
  * Cannot be a boot volume
* Magnetic (Standard)
* Lowest cost per GB of all EBS volume types that is bootable. Magnetic volumes are ideal for workloads where data is accessed infrequently, and applications where the lowest storage cost is important

### EC2 Exam Tips
* Know On-Demand, Reserved, Spot, and Dedicated Host EC2 services
* If a Spot instance is terminated by EC2, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for the complete hour in which the instance ran
* Know FIGHT DR MC PX acronym (EC2 instance types, specialties and use cases)
* SSD:
  * General Purpose SSD - Balance price and performance for a wide variety of workloads
  * Provisioned IOPS SSD - Highest performance SSD volume for mission-critical low-latency or high-throughput workloads

* Magnetic:
  * Throughput Optimized HDD - Low cost HDD volume designed for frequently accessed, throughput-intensive workloads
  * Cold HDD - Lowest cost HDD volume designed for less frequently accessed workloads
  * Magnetic - Previous generation. Can be boot volume

### EC2 Lab Summary
* Termination Protection is turned off by default, you must turn it on
* On an EBS-backed instance, the default action is for the root EBS volume to be deleted when the instance is terminated
* EBS root volumes of your DEFAULT AMI's cannot be encrypted. You can also use a third party tool (such as bit locker) to encrypt the root volume, or this can be done when creating AMI's in the AWS console or using the API

### Security Group Basics
* All inbound traffic is blocked by default
* All outbound traffic is allowed
* Changes to security groups take effect immediately
* You can have any number of EC2 instances within a security group
* You can have multiple security groups attached to EC2 instances
* Security groups are STATEFUL (network access control lists are STATELESS):
  * If you create an inbound rule allowing traffic in, that traffic is automatically allowed back out again
* You cannot block specific IP addresses using security groups, instead use Network Access Control Lists
* You can specify allow rules but not deny rules

### Volumes and Snapshots
* Volumes exist on EBS:
  * Virtual Hard Disk
* Snapshots exist on S3
* Snapshots are point in time copies of volumes
* Snapshots are incremental - this means that only the blocks that have changed since your last snapshot are moved to S3

### Snapshots of Root Device Volumes
* To create a snapshot for EBS volumes that serve as root devices, you should stop the instance before taking the snapshot
* However, you can take while the instance is running
* You can create AMI's from EBS-backed instances and snapshots
* You can change EBS volume sizes on the fly, including changing the size and storage type
* Volumes will ALWAYS be in the same AZ as the EC2 instance
* To move an EC2 volume from one AZ/Region to another, take a snap or an image of it, then copy it to the new AZ/Region

### Volume vs Snapshots - Security
* Snapshots of encrypted volumes are encrypted automatically
* Volumes restored from encrypted snapshots are encrypted automatically
* You can share snapshots, but only if they are unencrypted
  * These snapshots can be shared with other AWS accounts or made public

### RAID, Volumes and Snapshots
* RAID - Redundant Array of Independent Disks
  * RAID 0 - Striped, No Redundancy, Good Performance
  * RAID 1 - Mirrored, Redundancy
  * RAID 5 - Good for reads, bad for writes, AWS does not recommend ever putting RAID 5's on EBS
  * RAID 10 - Striped and Mirrored, Good Redundancy, Good Performance

### Snapshots of a RAID array
* Problem - Take a snapshot, the snapshot excludes data held in the cache by applications and the OS. This tends not to matter on a single volume, however using multiple volumes in a RAID array, this can be a problem due to interdependencies of the array
* Solution - Take an application consistent snapshot
  * Stop the application from writing to disk
  * Flush all caches to the disk
  * Ways to accomplish these tasks above:
    * Freeze the file system
    * Unmount the RAID array
    * Shutting down the associated EC2 instance

### EBS vs Instance Store
* All AMIs are categorized as either backed by EBS or backed by instance store
* For EBS volumes - The root device for an instance launched from the AMI is an EBS volume created from an EBS snapshot
* For instance store volumes - The root device for an instance launched from the AMI is an instance store volume created from a template stored in S3

### EBS vs Instance Store - Exam Tips
* Instance store volumes are sometimes called Ephemeral Storage
* Instance store volumes cannot be stopped. If the underlying host fails, you lose your data
* EBS backed instance can be stopped. You will not lose the data on this instance if it is stopped
* You can reboot both, you will not lose your data
* By default, both ROOT volumes will be deleted on termination, however with EBS volumes, you can tell AWS to keep the root device volume

### Types of Load Balancers
Three types of load balancers:
* Application load balancer - Are best suited for load balancing of HTTP and HTTPS traffic. They operate at Layer 7 and are application-aware. They are intelligent, and you can create advanced request routing, sending specified requests to specific web servers
* Network load balancer - Are best suited for load balancing of TCP traffic where extreme performance is required. Operating at the connection level (Layer 4), network load balancers are capable of handling millions of requests per second, while maintaining ultra-low latencies. Use for extreme performance
* Classic load balancer - Are the legacy ELB (Elastic Load Balancers). You can load balance HTTP/HTTPS applications and use Layer 7-specific features, such as X-Forwarded and sticky sessions. You can also use strict Layer 4 load balancing for applications that rely purely on the TCP protocol

### Load Balancer Errors
* Classic Load Balancers - If your application stops responding the ELB responds with a 504 error. This means that the application is having issues. This could be either at the Web Server layer or at the Database Layer. Identify where the application is failing and scale it up or out where possible

### ELB Exam Tips
* 3 types of load balancers:
  * Application load balancers
  * Network load balancers
  * Classic load balancers
* 504 error means that the gateway has timed out. This means that the application not responding within the idle timeout period.
  * Trouble shoot the application. Is it the Web Server or Database Server?
* If you need the IPv4 address of your end user, look for the X-Forwarded-For-Header

### Elastic Load Balancers Lab
* Instances monitored by ELB are reported as “In Service” or “Out of Service”
* Health Checks - Check the instance health by talking to it
* ELBs have their own DNS name. You are never given an IP address
* Read the ELB FAQ for Classic Load Balancers

### CloudWatch EC2 Lab
* Standard Monitoring - 5 minute
* Detailed Monitoring - 1 minute
* What can I do with CloudWatch?
  * Dashboards - Create awesome dashboards to see what is happening with your AWS environment
  * Alarms - Allows you to set Alarms that notify you when particular thresholds are hit
  * Events - CloudWatch events helps you respond to state changes in your AWS resources
  * Logs - CloudWatch logs helps you aggregate, monitor, and store logs

### The AWS Command Line and EC2
* When we configure AWS via command line we are actually storing credentials locally on the EC2 instance
* Using user credentials is not safe and storing them on EC2 instances is not recommended

### Using IAM roles with EC2
* Roles help secure credentials in AWS EC2
* Remember that all roles are global so there is no need to create a new role in another Region

### S3 CLI and Regions
* You can now actually attach a role to an EC2 instance via CLI or AWS console

### Using Bootstrap Scripts
* Bash scripts are always passed in the Advanced Details tab
* We use #!/bin/bash to start the bash script
* Bash scripts allows us to automate our web servers

### EC2 Instance Metadata
Instance metadata is data about your instance that you can use to configure or manage the running instance. Instance metadata is divided into categories.

Although you can only access instance metadata and user data from within the instance itself, the data is not protected by cryptographic methods. Anyone who can access the instance can view its metadata. Therefore, you should take suitable precautions to protect sensitive data (such as long-lived encryption keys). You should not store sensitive data, such as passwords, as user data.

You can also use instance metadata to access user data that you specified when launching your instance. For example, you can specify parameters for configuring your instance, or attach a simple script. You can also use this data to build more generic AMIs that can be modified by configuration files supplied at launch time. For example, if you run web servers for various small businesses, they can all use the same AMI and retrieve their content from the Amazon S3 bucket you specify in the user data at launch. To add a new customer at any time, simply create a bucket for the customer, add their content, and launch your AMI. If you launch more than one instance at the same time, the user data is available to all instances in that reservation.

EC2 instances can also include dynamic data, such as an instance identity document that is generated when the instance is launched.

For more information on EC2 instance metadata see the AWS EC2 guide on [Instance Metadata and User Data](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html).

### Autoscaling Lab
An important take away is that you can have instances spread across multiple AZs and even if you lose two of those AZ out of three you still won't have an outage. Route 53 can also help further protect from regional failure by detecting failure and redirecting traffic to other parts of the world.

### EC2 Placement Groups
There are two types of placement groups:
* Clustered Placement Group - A grouping of instances within a single AZ. Placement groups are recommended for applications that need low network latency, high network throughput, or both. Only certain instances can be launched into a clustered placement group
* Spread Placement Group - A group of instances that are each placed on distinct underlying hardware. Spread placement groups are recommended for applications that have a small number of critical instances that should be kept separate from each other

Things to review before the exam:
* A clustered placement group can't span multiple AZ
* A spread placement group can span multiple AZ
* The name you specify for a placement group must be unique within your AWS account
* Only certain types of instances can be launched in a placement group (Compute Optimized, GPU, Memory Optimized, Storage Optimized)
* AWS recommend homogenous instances within placement groups
* You can't merge placement groups
* You can't move an existing instance into a placement group. You can create an AMI from your existing instance, and then launch a new instance from the AMU into a placement group

### What is EFS?
Amazon EFS (Elastic File System) is a file storage service for Amazon EC2 instances. Amazon EFS is easy to use and provides a simple interface that allows you to create and configure file systems quickly and easily. With EFS, storage capacity is elastic, growing and shrinking automatically as you add and remove files, so your applications have the storage they need, when they need it.

### EFS Features
* Supports the Network File System version 4 (NFSv4) protocol
* You only pay for the storage you use (no pre-provisioning required)
* Can scale up to the petabytes
* Can support thousands of concurrent NFS connections
* Data is stored across multiple AZ's within a region
* Read After Write Consistency

Use case for EFS:
* Using EFS as a file server or a central repository for your files within your EC2 instances
* Can set restrictions which will be reflected across all EC2 instances
* EFS allows multiple EC2 instances to connect to it whereas EBS can only mount to a single EC2 instance

### What is Lambda?
AWS Lambda is a compute service where you can upload your code and create a Lambda function. AWS Lambda takes care of provisioning and managing the servers that you use to run the code. You don't have to worry about operating systems, patching, scaling, etc. You can use Lambda in the following ways:

* As an event-driven compute service where the AWS Lambda runs your code in response to events. These events could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table
* As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs

Lambda is an encapsulation of the following:
* Data Centers
* Hardware
* Assembly Code/Protocols
* High Level Languages
* Operating Systems
* Application Layer/AWS APIs
* AWS Lambda

### How is Lambda Priced?
* Number of requests:
  * First 1 million requests are free. $0.20 per 1 million requests thereafter
* Duration:
  * Calculated from the time your code begins executing until it returns or otherwise terminates, rounded up to the nearest 100 ms. The price depends on the amount of memory you allocate to your function. You are charged $0.00001667 for every GB-second used

### Why is Lambda Cool?
* No servers!
* Continuous scaling!
* Super cheap!

### Lambda - Exam Tips
* Lambda scales out (not up) automatically
* Lambda functions are independent, 1 event = 1 function
* Lambda is serverless
* Know what services are serverless!
* Lambda function can trigger other lambda functions, 1 event can = x functions if functions trigger other functions

* Architectures can get extremely complicated, AWS X-ray allows you to debug what is happening
* Lambda can do things globally, you can use it to back up S3 buckets to other S3 buckets etc.
* Know triggers

### Build a Serverless Page
Below is a schematic of how the lambda serverless website will work with Route 53, API Gateway, Lambda, and S3. The steps are as follows:

1. Get IP address
2. Route 53 returns IP address
3. Get web page from S3
4. Return static/dynamic content
5. Get request to API Gateway
6. Forward request to Lambda
7. Return data to user

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/lambda-serverless-web.jpg">
  <h3>Figure 5-2. Lambda serverless web schematic</h3>
</div>

### Using Polly
Below is a schematic of how Polly will be set up in AWS. Polly converts text into an MP3 file.

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/polly-setup.jpg">
  <h3>Figure 5-3. Overview of Polly application</h3>
</div>

### EC2 Summary
Below are the major subsections in Section 5 worth going over before the exam.

#### Exam Tips - EC2
* Know the differences between:
  * On Demand
  * Spot
  * Reserved
  * Dedicated Hosts
* Remember with spot instances:
  * If you terminate the instance, you pay for the hour
  * If AWS terminates the spot instance, you get the hour it was terminated in for free

* Know the EC2 instance types as shown in Figure 5-1

#### Exam Tips - EBS
* EBS Consists of:
  * SSD, General Purpose - GP2 - (up to 10,000 IPOS)
  * SSD, Provisioned IOPS - IO1 - (more than 10,000 IOPS)
  * HDD, Throughput Optimized - ST1 - Frequently accessed workloads
  * HDD, Cold - SC1 - Less frequently accessed data
  * HDD, Magnetic - Standard - Cheap, infrequently accessed storage

* You cannot mount a single EBS volume to multiple EC2 instances; instead use EFS

#### Exam Tips - EC2 Lab
* Termination Protection is turned off by default, you must turn it on
* On an EBS-backed instance, the default action is for the root EBS volume to be deleted when the instance is terminated
* EBS-backed root volumes can now be encrypted using AWS API or console or you can use a third party tool to encrypt the root volume
* Additional volumes can also be encrypted

#### Exam Tips - Volumes vs Snapshots
* Volumes exist on EBS:
  * Virtual hard disk
* Snapshots exist on S3
* You can take a snapshot of a volume, this will store that volume on S3
* Snapshots are point in time copies of volumes
* Snapshots are incremental. This means that only the blocks that have changed since your last snapshot are moved to S3
* It may take some time to create the first snapshot

#### Exam Tips - Volumes vs Snapshots - Security
* Snapshots of encrypted volumes are encrypted automatically
* Volumes restored from encrypted snapshots are encrypted automatically
* You can share snapshots, but only if they are unencrypted
  * These snapshots can be shared with other AWS accounts or made public

#### Exam Tips - Snapshots of Root Device Volumes
* To create a snapshot for Amazon EBS volumes that serve as root devices, you should stop the instance before taking the snapshot

#### Exam Tips - EBS vs Instance Store
* Instance store volumes are sometimes called Ephemeral Storage
* Instance store volumes cannot be stopped. If the underlying host fails, you lose your data
* EBS backed instance can be stopped. You will not lose the data on this instance if it is stopped
* You can reboot both, you will not lose your data
* By default, both ROOT volumes will be deleted on termination, however with EBS volumes, you can tell AWS to keep the root device volume

### How to take Snapshots of a RAID array
* Problem - Take a snapshot, the snapshot excludes data held in the cache by applications and the OS. This tends not to matter on a single volume, however using multiple volumes in a RAID array, this can be a problem due to interdependencies of the array
* Solution - Take an application consistent snapshot
  * Stop the application from writing to disk
  * Flush all caches to the disk
  * Ways to accomplish these tasks above:
    * Freeze the file system
    * Unmount the RAID array
    * Shutting down the associated EC2 instance

#### Exam Tips - Amazon Machine Images
AMIs are regional. You can only launch an AMI from the region in which it is stored. However you can copy AMIs to other regions using the console, command line, or the Amazon EC2 API

#### Exam Tips - CloudWatch Lab
* Standard Monitoring - 5 minute
* Detailed Monitoring - 1 minute

* CloudWatch is performance monitoring
* CloudTrail is for auditing

#### What can I do with CloudWatch?
  * Dashboards - Create awesome dashboards to see what is happening with your AWS environment
  * Alarms - Allows you to set Alarms that notify you when particular thresholds are hit
  * Events - CloudWatch events helps you respond to state changes in your AWS resources
  * Logs - CloudWatch logs helps you aggregate, monitor, and store logs

#### Exam Tips - Roles Lab
* Roles are more secure than storing your access key and secret access key on individual EC@ instances
* Roles are easier to manage
* Roles can be assigned to an EC2 instance AFTER it has been provisioned using both the command line and the AWS console
* Roles are universal - you can use them in any region

#### Exam Tips - Instance Metadata
* Used to get information about an instance (such as public IP)

#### Exam Tips - EFS Lab
* Supports the Network File System version 4 (NFSv4) protocol
* You only pay for the storage you use (no pre-provisioning required)
* Can scale up to the petabytes
* Can support thousands of concurrent NFS connections
* Data is stored across multiple AZ's within a region
* Read After Write Consistency

#### What is Lambda?
AWS Lambda is a compute service where you can upload your code and create a Lambda function. AWS Lambda takes care of provisioning and managing the servers that you use to run the code. You don't have to worry about operating systems, patching, scaling, etc. You can use Lambda in the following ways:

* As an event-driven compute service where the AWS Lambda runs your code in response to events. These events could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table
* As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs

#### What is a Placement Group?
There are two types of placement groups:
* Clustered Placement Group - A grouping of instances within a single AZ. Placement groups are recommended for applications that need low network latency, high network throughput, or both. Only certain instances can be launched into a clustered placement group
* Spread Placement Group - A group of instances that are each placed on distinct underlying hardware. Spread placement groups are recommended for applications that have a small number of critical instances that should be kept separate from each other

## Section 5 Quiz

**1. EBS Snapshots are backed up to S3 in what manner?**
* Incrementally

**2. Do Amazon EBS volumes persist independently from the life of an Amazon EC2 instance, for example, if I terminated an EC2 instance, would that EBS volume remain?**
* Only if instructed to when created

**3. Can I delete a snapshot of an EBS Volume that is used as the root device of a registered AMI?**
* No, you must deregister the AMI before being able to delete the root device

**4. A placement group can be deployed across multiple Availability Zones.**
* False

**5. While creating the snapshots using the command line tools, which command should I be using?**
* ec2-create-snapshot

**6. Can you attach an EBS volume to more than one EC2 instance at the same time?**
* No

**7. A placement group is ideal for**
* EC2 instances that require high network throughput and low latency across a single AZ

**8. Using the console, I can add a role to an EC2 instance, after that instance has been created and powered up.**
* True

**9. I can change the permissions to a role, even if that role is already assigned to an existing EC2 instance, and these changes will take effect immediately.**
* True

---

# Section 6: Route 53

This section will cover an in-depth overview on the AWS Route 53 service.

### What is DNS?
DNS is used to convert human friendly domain names into an IP (Internet Protocol) address.
* IP addresses are used by computers to identify each other on the network
* IP addresses commonly come in 2 different forms, IPv4 and IPv6

### IPv4 vs IPv6
* IPv4 space is a 32 bit field has over 4 billion (4,294,967,296) different addresses
* IPv6 had an address space of 128 bits which is 340 undecillion addresses

### Top Level Domains
* The last word in a domain name represents the top level domain name (i.e. the .com in google.com) whereas the second word in a domain name is known as the second level domain name (i.e. acloud.guru)
* Top level domain names are controlled by the IANA (Internet Assigned Numbers Authority) in a root zone database which is essentially a database of all available top level domains

### Domain Registrars
* A registrar is an authority that can assign domain names directly under one or more top-level domains. Each domain name becomes registered in a central database known as the WhoIS database.

### SOA (Start of Authority) Record
* The SOA records stores information about:
  * The name of the server that supplied that data for the zone
  * The administrator of the zone
  * The current version of the data file
  * The default number of seconds for the time-to-live file on resource records

### NS Records
* NS (Name Server) records are used by top level domain servers to direct traffic to the content DNS server which contains the authoritative DNS records

### A Records
* The address record is used by a computer to translate the name of the domain to an IP address

### TTL
* The length that a DNS record is cached on either the resolving server or the users own local PC is to the value of the TTL (Time To Live) in seconds.

### CNames
* A CName (Canonical Name) can be used to resolve one domain name to another

### Alias Records
* Alias records are used to map resource record sets in your hosted zone to Elastic Load Balancers, CloudFront distributions, or S3 buckets that are configured as websites
* Unlike a CName, an alias record can't be used for naked domain names (zone apex record). It must be either an A record or an alias.

### DNS 101 Exam Tips
* ELBS do not have pre-defined IPv4 addresses; you resolve to them using a DNS name
* Alias record vs CName
* Always choose alias record over a CName

### Common DNS Types
* SOA records
* NS records
* A records
* CNames
* MX records
* PTR records

### Routing Policies Available on AWS
There are several different routing policies on AWS
* Simple routing
* Weighted routing
* Latency-based routing
* Failover routing
* Geolocation routing
* Multivalue answer routing

### Simple Routing Policy - Lab
If you choose simple routing policy you can only have one record with multiple IP addresses. If you specify multiple values in a record, Route 53 returns all values to the user in a random order.

### Weighted Routing Policy - Lab
Weighted routing policies let you split your traffic based on different weights assigned (e.g. you can set 20% of your traffic to go to US-EAST-1 and then 80% to go to EU-WEST-1).

### Latency Routing Policy - Lab
Latency based routing allows you to route you traffic based on the lowest network latency for you end user (i.e. which region will give them the fastest response time). To use latency-based routing, you create a latency resource record set for the EC2 (or ELB) resource in each region that hosts your website. When Route 53 receives a query for your site, it selects the latency resource record set for the region that gives the user the lowest latency. Route 53 then responds with the value associated with that resource record set.

### Failover Routing Policy - Lab
Failover routing policies are used when you want to create an active/passive set up. For example, you may want your primary site to be in EU-WEST-2 and your secondary DR site in AP-SOUTHEAST-2.
* Route 53 will monitor the health or your primary site using a health check
* A health check monitors the health of your end points

### Geolocation Routing Policy - Lab
Geolocation routing lets you choose where your traffic will be sent based on the geographic location of your users.

### Multivalue Routing
If you want to route traffic approximately randomly to multiple resources, such as web servers, you can create one multivalue answer record for each resource and, optionally, associate a Route 53 health check with each record. If you create a dozen multivalue answer records, Route 53 responds to DNS queries with up to eight healthy records in response to each DNS query.

### DNS Exam Tips
Make sure to go over the sections above (mainly routing policy sections) before taking the exam.

## Section 6 Quiz

**1. Does Route 53 support MX Records?**
* Yes

**2. Route 53 is named so because**
* The DNS Port is on Port 53 and Route 53 is a DNS Service

**3. Route 53 does not support zone apex records (or naked domain names)**
* Incorrect

**4. Route53 is Amazon's DNS Service**
* True

**5. There is a limit to the number of domain names that you can manage using Route 53.**
* True and False. There is a limit of domain names, however this limit can be raised by contacting AWS support.

---

# Section 7: Databases on AWS

This section will cover an in-depth overview on databases on AWS.

### What is a relational database?
Relational databased are what most of us are all used to. They have been around since the 70's (think traditional spreadsheet):
* Database
* Tables
* Row
* Fields (columns)

<div align="center">
  <img src="relational-db.jpg">
  <h3>Figure 7-1. Example of a traditional relational database</h3>
</div>

### Relational Database Types
There are several of relational database types:
* SQL server
* Oracle
* MySQL server
* PostgreSQL
* Aurora
* MariaDB

### Non-relational Databases
A non-relational database consists of the following:
* Database
  * Collection -> Table
  * Document -> Row
  * Key value pairs -> Fields

<div align="center">
  <img src="non-relational-db.jpg">
  <h3>Figure 7-2. Example of a non-relational database</h3>
</div>

### What is Data Warehousing?
* Used for business intelligence. Tools like Cognos, Jaspersoft, SQL Server Reporting Services, Oracle Hyperion, SAP NetWeaver
* Used to pull in very large and complex data sets. Usually used by management to do queries on data (such as current performance vs targets, etc.)

### OLTP vs OLAP
* OLTP (Online Transaction Processing) differs from OLAP (Online Analytics Processing) in terms of the types of queries you will run
* OLTP: Pulls up a row of data such as name, date, delivery address, delivery status, etc.
* OLAP: Find net profit for EMEA and Pacific for the Digital Radio Product:
  1.  Pulls in large number of records
  2.  Sum of radios sold in EMEA
  3.  Sum of radios sold in Pacific
  4.  Unit cost of radio in each region
  5.  Sales price of each radio
  6.  Sales price - unit cost
* Data warehousing databases use different type of architecture both from a database perspective and infrastructure layer

### What is ElastiCache?
* ElastiCache is a web service that makes it easy to deploy, operate, and scale an in-memory cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory caches, instead of relying entirely on slower disk-based databases
* ElastiCache supports two open-source in-memory caching engines:
  * Memcached
  * Redis

### AWS Database Types - Summary
* RDS - OLTP
  * SQL
  * MySQL
  * PostgreSQL
  * Oracle
  * Aurora
  * MariaDB
* DynamoDB - No SQL
* Redshift - OLAP
* ElastiCache - In Memory Caching

### RDS - Backups, Mult-AZ, and Read Replicas
* There are two different types of backups for AWS
  * Automated backups
  * Database snapshots
* Automated backups allow you to recover your database to any point in time within a "retention period"
* The retention period can be between one and 35 days. Automated backups will take a full daily snapshot and will also store transaction logs throughout the day. When you do a recovery. AWS will first choose the most recent daily back up, and then apply transaction logs relevant to that day. This allows you to do a point in time recovery down to a second, within the retention period

### Automated Backups
* Automated backups are enabled by default. The backup data is stored in S3 and you get free storage space equal to the size of your database. SO if you have an RDS instance of 10 GB, you will get 10 GB worth of storage
* Backups are taken within a defined window. During the backup window, storage I/O may be suspended while your data is being backed up and you may experience elevated latency

### Snapshots
DB Snapshots are done manually (i.e. they are user initiated) and are stored even after you delete the original RDS instance, unlike automated backups.

### Restoring Backups
Whenever you restore either an automatic backup or a manual Snapshot, the restored version of the database will be a new RDS instance with a new DNS endpoint.

### Encryption
* Encryption at rest is supported for MySQL, Oracle, SQL Server, PostgreSQL, MariaDB, and Aurora. Encryption is done using AWS KMS (Key Management Service). Once your RDS instance is encrypted, the data stored at rest in the underlying storage is encrypted, as are its automated backups, read replicas, and snapshots
* At the present time, encrypting an existing DB instance is not supported. To use Amazon RDS encryption for an existing database, you must first create a snapshot, make a copy of that snapshot and encrypt the copy

### What is Multi-AZ?
Any changes to an RDS in US-EAST-1A for example will be synchronously replicated in another instance in US-EAST-1B for example where US-EAST-1B is an exact copy of US-EAST-1A.

<div align="center">
  <img src="multi-az.jpg">
  <h3>Figure 7-3. Example of a Multi-AZ setup for AWS RDS</h3>
</div>

### What is Multi-AZ RDS?
* Multi-AZ allows you to have an exact copy of your production database in another AZ. AWS handles the replication for you so when your production databases is written to, this will automatically be synchronized to the stand by database
* In the event of planned database maintenance, DB instance failure, or an AZ failure, Amazon RDS will automatically failover to the standby so that database operations can resume quickly without administrative intervention
* **Multi-AZ is for disaster recovery only**, it is not primarily used for improving performance. For performance improvement you need Read Replicas

### Multi-AZ Databases
Multi-AZ databases are available for the following:
* SQL server
* Oracle
* MySQL server
* PostgreSQL
* MariaDB

### What is a Read Replica?
Read replicas allow you to have a read-only copy of your production database. This is achieved by using asynchronous replication from the primary RDS instance to the read replica. You use read replicas primarily for very read-heavy database workloads.

<div align="center">
  <img src="read-replica.jpg">
  <h3>Figure 7-4. Example of a read replica (depicted in blue) setup on AWS</h3>
</div>

### Read Replica Databases
Read Replica databases are available for the following:
* MySQL server
* PostgreSQL
* MariaDB
* Aurora

In addition, read replica databases:
* Are used for scaling **not** for disaster recovery
* Must have automatic backups turned on in order to deploy a read replica
* Can have up to five read replica copies of any database
* Can have read replicas of read replicas (can create latency issues)
* Will have its own DNS end point
* **Can** have read replicas that have Multi-AZ
* **Can** create read replicas of Multi-AZ source databases
* Can be promoted to be their own databases. This breaks the replication however
* Can have a read replica in a second region

### What is DynamoDB?
Amazon DynamoDB is a fast and flexible NoSQL database service for all apps that need consistent, single-digit millisecond latency at any scale. It is a fully managed database and supports both document and key-value data models. Its flexible data model and reliable performance make it a great fit for mobile, web, gaming, ad-tech, IoT, and many other apps.

### DynamoDB
* Stored on SSD storage
* Spread across three geographically distinct data centers
* Eventual consistent reads (default)
  * Consistency across all copies of data is usually reached within a second. Repeating a read after a short time should return the updated data (best read performance)
* Strongly consistent reads
  * A strongly consistent read returns a result that reflects all writes that received a successful response prior to the read

### DynamoDB Pricing
* Provisioned throughout capacity
  * Write throughput $0.0065 per hour for every 10 units
  * Read throughput $0.0065 per hour for every 50 units
* Storage costs of $0.25 GB per month

### What is Redshift
Amazon Redshift is a fast and powerful, fully managed, petabyte-scale data warehouse service in the cloud. Customers can start small for just $0.25 per hour with no commitments or upfront costs and scale to a petabyte or more for $1,000 per terabyte per year, less than a tenth of most other data warehousing solutions.

### Redshift Configuration
* Single Node (160 GB)
* Multi-node
  * Leader Node (manages client connections and receives queries)
  * Compute Node (store data and perform queries and computations up to 128 compute nodes)

### Redshift - 10 Times Faster
* **Columnar Data Storage**: Instead of storing data as a series of rows, Amazon Redshift organizes the data by column. Since only the columns involved in the queries are processed and columnar data is stored sequentially on the storage media, column-based systems require far fewer I/O, greatly improving query performance
* **Advanced Compression**: Columnar data stores can be compressed much more than row-based data stores because similar data is stored sequentially on disk. In addition, Redshift does not require indexes or materialized view and so uses less space than traditional relational database systems. When loading data into an empty table, Redshift automatically samples your data and selects the most appropriate compression scheme
* **MPP (Massive Parallel Processing)**: Redshift automatically distributes data and query load across all nodes

### Redshift Pricing
* Compute node hours (total number of hours you run across all your compute nodes for the billing period, you are billed for 1 unit per node per hour)
* Backup
* Data transfer (only within a VPC)

### Redshift Security
* Encrypted in transit using SSL
* Encrypted at rest using AES-256 encryption
* By default Redshift takes care of key management
  * Manage your own keys through HSM
  * AWS KMS

### Redshift Availability
* Currently only available in 1 AZ
* Can restore snapshots to new AZ's in the event of an outage

### What is ElastiCache?
ElastiCache is a web service that makes it easy to deploy, operate, and scale an in-memory cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory caches, instead of relying entirely on slower disk-based databases.

### Types of ElastiCache
* Memcached
  * A widely adopted memory object caching system
* Redis
  * A popular open-source in-memory key-value store that supports data structures such as sorted sets and lists.

### ElastiCache Exam Tips
* Typically will be given a scenario where a particular database is under a lot of stress/load. You may be asked which service you should use to alleviate the load.
* ElastiCache is a good choice if your database is particularly read heavy and not prone to frequent changing
* Redshift is a good choice if the reason your database is feeling stress is because management keeps running OLAP transactions on it, etc.

### What is Aurora?
Amazon Aurora is a MySQL-compatible, relational database engine that combines the speed and availability of high-end commercial databases with the simplicity and cost-effectiveness of open source databases. Amazon Aurora provides up to five times better performance than MySQL at a price point one tenth of that of a commercial database while delivering similar performance and availability.

### Aurora Scaling
* Start with 10 GB, scales in 10 GB increments to 64 TB (storage auto scaling)
* Compute resources can scale up to 32vCPUs and 244 GB of memory
* Two copies of your data is contained in each AZ, with minimum of three AZ
* Aurora is designed to transparently handle the loss of up to two copies of data without affecting database write availability and up to three copies without affecting read availability
* Aurora storage is also self-healing. Data blocks and disks are continuously scanned for errors and repaired automatically

### Aurora Replicas
* Two types of replicas are available
* Aurora replicas (currently 15)
* MySQL Read Replicas (currently five)

### AWS Database Types - Summary
* RDS - OLTP
  * SQL
  * MySQL
  * PostgreSQL
  * Oracle
  * Aurora
  * MariaDB
* DynamoDB - NoSQL
* Redshift - OLAP
* ElastiCache - In memory caching
  * Memcached
  * Redis

### DynamoDB vs RDS
* DynamoDB offers "push button" scaling, meaning that you can scale your database on the fly, without any down time
* RDS is not so easy and you usually have to use a bigger instance size or to add a read replica

## Section 7 Quiz

**1. What AWS DB platform is most suitable for OLTP?**
* RDS/DynamoDB

**2. When replicating data from your primary RDS instance to your secondary RDS instance, what is the charge?**
* No charge, it's free

**3. What AWS service is best suited for non-relational databases?**
* DynamoDB

**4. When you add a rule to an RDS security group you do not need to specify a port number or protocol?**
* False

**5. If you are using Amazon RDS Provisioned IOPS storage with MySQL and Oracle database engines what is the maximum size RDS volume you can have by default?**
* 16 TB

**6. What happens to the I/O operations while you take a database snapshot**
* I/O operations to the database are suspended for the duration of the snapshot

**7. What AWS service is best used for Business Intelligence Tools/Data Warehousing?**
* Redshift

**8. In RDS when using multiple availability zones, can you use the secondary database as an independent read node?**
* No

**9. Amazon's ElastiCache uses which two engines?**
* Redis and Memcached

**10. By default, the maximum provisioned IOPS capacity on an Oracle and MySQL RDS instance (using provisioned IOPS) is 30,000 IOPS.**
* Limits change over time

---

# Section 8: VPC

This section will cover an in-depth overview on AWS VPC.

### What is a VPC?
Think of a VPC (Virtual Private Cloud) as a virtual data center in the cloud. A VPC lets you provision a logically isolated section of the AWS cloud where you can launch AWS resources in a virtual network that you define. You have complete control over you virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways.

<div align="center">
  <img src="aws-vpc.jpg">
  <h3>Figure 8-1. Diagram of a VPC setup on AWS</h3>
</div>

### What can you do with a VPC?
* Launch instances into a subnet of your choosing
* Assign custom IP address ranges in each subnet
* Configure route tables between subnets
* Create internet gateway and attach it to our VPC
* Much better security control over your AWS resources
* Instance security groups
* Subnet network ACLs (access control lists)

### Default VPC vs Custom VPC
* Default VPC is user friendly, allowing you to immediately deploy instances
* All subnets in default VPC have a route out to the internet
* Each EC2 instance has both a public and private IP address

### Peering VPC
* Allows you to connect one VPC with another via a direct network route using private IP addresses
* Instances behave as if they were on the same private network
* You can peer VPC's with other AWS accounts as well as with other VPC's in the same account
* Peering is in a star configuration: i.e. one central VPC peers with 4 others. No transitive peering

### VPC - Exam Tips
* Think of a VPC as a logical datacenter in AWS
* Consists of IGW (Virtual Private Gateways), route tables, network access control lists, subnets, and security groups
* 1 Subnet = 1 AZ
* Security groups are stateful; network access control lists are stateless
* **No transitive peering**

### Exam Tips - Network ACLs
* Your VPC automatically comes with a default network ACL and by default it allows all outbound and inbound traffic
* You can create custom network ACLs. By default each custom network ACL denies all inbound and outbound traffic until you add rules
* Each subnet in your VPC must be associated with a network ACL. If you do not explicitly associate a subnet with a network ACL, the subnet is automatically associated with a network ACL
* You can associate a network ACL with multiple subnets; however, a subnet can be associated with only one network ACL at a time. When you associate a network ACL with a subnet, the previous associate is removed
* Network ACLs contain a numbered list of rules that is evaluated in order, starting with the lowest numbered rule
* Network ACLs have separate inbound and outbound rules, and each rule can either allow or deny traffic
* Network ACLs are stateless; responses to allow inbound traffic are subject to the rules for outbound traffic (and vice versa)
* Block IP addresses using network ACLs not security groups

### VPC Flow Logs
* VPC Flow Logs is a feature that enables you to capture information about the IP traffic going to and from network interfaces in your VPC. Flow log data is stored using Amazon CloudWatch Logs. After you've created a flow log, you can view and retrieve its data in Amazon CloudWatch Logs.

* Flow logs can be created at 3 levels:
  * VPC
  * Subnet
  * Network interface level

### Exam Tips - VPC Flow Logs
* You cannot enable flow logs for VPCs that are peered with your VPC unless the peer VPC is in your account
* You cannot tag a flow log
* After you've created a flow log, you cannot change its configuration; for example, you can't associate a different IAM role with the flow log

### Not all IP traffic is monitored
* Traffic generated by instances when they contact the Amazon DNS server. If you use your own DNS server, then all traffic to that DNS server is logged
* Traffic generated by a Windows instance for Amazon Windows license activation
* Traffic to the reserved IP address for the default VPC router
* DHCP traffic

### Exam Tips - NATs vs Bastions
* NAT (Network Address Translation) is used to provide internet traffic to EC2 instances in private subnets
* Bastion is used to securely administer EC2 instances (using SH or RDP) in private subnets

### Exam Tips - NAT Instances
* When creating a NAT instance, disable source/destination check on the instance
* NAT instances must be in a public subnet
* There must be a route out of the private subnet to the NAT instance, in order for this to work
* The amount of traffic that NAT instances can support depends on the instance size. If you are bottlenecking, increase the instance size
* You can create high availability using auto scaling groups, multiple subnets in different AZs, and a script to automate failover
* Behind a security group

### Exam Tips - NAT Gateways
* Preferred by the enterprise
* Scale automatically up to 10 GBs
* No need to patch
* Not associated with security groups
* Automatically assigned a public IP address
* Remember to update your route tables
* No need to disable source/destination checks
* More secure than a NAT instance

### Exam Tips - ALB's
* You will need at least two public subnets in order to deploy an ALB (Application Load Balancer)

## Section 8 Quiz

**1. Security groups act like a firewall at the instance level whereas ___ are an additional layer of security that act at the subnet level.**
* ACLs

**2. How many VPC's am I allowed in each AWS Region by default?**
* Five

**3. VPC stands for:**
* Virtual Private Cloud

**4. How many internet gateways can I attach to my custom VPC?**
* One

**5. You have a VPC with both public and private subnets. You have 3 EC2 instances that have been deployed in to the public subnet and each has internet access. You deploy a 4th instance using the same AMI and this instance does not have internet access. What could be the cause of this?**
* The instance needs either an Elastic IP address/Public IP address assigned to it

---

# Section 9: Application Services

This section will cover an in-depth overview on AWS Application Services.

### What is SQS?
* Amazon SQS (Simple Queueing Service) is a web service that give you access to a message queue that can be used to store messages while waiting for a computer to process them
* SQS is a distributed queue system that enables web service applications to quickly and reliably queue messafes that one component in the application generates to be consumed by another component. A queue is a temporary repository for messages that are awaiting processing

* Using SQS you can decouple the components of an application so they run independently, easing message management between components
* Any component of a distributed application can store messages in the queue. Messages can contain up to 256 KB of text in any format. Any component can later retrieve the messages programmatically using the SQS API

* The queue acts as a buffer between the component producing and saving data, and the component receiving the data for the processing. This means that the queue resolves issues that arise if the producer is producing work faster than the consumer can process it, or if the producer or consumer are only intermittently connected to the network

### Queue Types
There are two types of queue:
* Standard queues (default)
* FIFO queues (first-in-first-out)

### Standard Queues
A standard queue is the default AWS SQS type. A standard queue lets you have nearly-unlimited number of transaction per second. Standard queues guarantee that a message is delivered at least once. However, occasionally (because of the highly-distributed architecture that allows high throughput) more than one copy of a message might be delivered out of order. Standard queues provide the best-effort ordering which ensures that messages are generally delivered in the same order as they are sent.

### FIFO Queues
The most important features of FIFO queue is the FIFO (first-in-first-out) delivery and exactly-once processing: the order in which messages are sent and received is strictly preserved and a message is delivered once and remains available until a consumer processes and deletes it; duplicates are not introduceds into the queue. FIFO queues also support message groups that allow multiple ordered message groups within a single queue. FIFO queues are limited to 300 TPS (transactions per second) but have all the capabilities of standard queues.

### SQS Key Facts
* SQS is pull-based, not pushed-based
* Messages are 256 KB in size
* Messages can be kept in the queue from one minute to 14 days
* Default retention period is four days
* SQS guarantees that you messages will be processed at least once

### SQS Visibility Timeout
* The visibility timeout is the amount of time that the messages is invisible in the SQS queue after a reader picks up that message
* Default visibility timeout is 30 seconds
* Increase it if your task takes > 30 seconds
* Maximum is 12 hours

### SQS Long Polling
* SQS long polling is a way to retrieve the messages from your SQS queues
* While the regular short polling returns immediately, long polling does not return a response until a message arrives in the message queue, or the long poll times out
* Long polling can save money

### Exam Tips - SQS
* SQS is a distributed messages queueing system
* Allows you to decouple the components of an application so that they are independent
* Pull-based not push-based
* Standard queue (default): best-effort ordering; message delivered at least once
* FIFO queues (first-in-first-out) - ordering strictly preserved, message delivered once, no duplicates, e.g. good for banking transactions which need to happen in strict order
* Visibility timeout
    * Default is 30 seconds - increase if your task takes > 30 seconds to complete
    * Max is 12 hours
* Short polling - returned immediately even if no messages are in the queue
* Long polling - polls the queue periodically and only returns a response when a message is in the queue for the timeout is reached

### SWF
Amazon SWF (Simple Workflow Service) is a web service that makes it easy to coordinate work across distributed application components. SWF enables applications for a range of use cases.

### SWF Workers
Workers are programs that interact with SWF to get tasks, process received tasks, and return the results.

### SWF Decider
The decider is a program that controls the coordination of tasks, i.e. their ordering, concurrency, and scheduling according to the application logic.

### SWF Workers and Deciders
* The workers and the decider can run on cloud infrastructure, such as AWS EC2, or on machines behind firewalls. SWF brokers the interactions between works and the decider. It allows the decider to get consistent views into the progress of tasks and to initiate new tasks in an ongoing manner
* At the same time SWF stores tasks, assigns them to workers when they are ready, and monitors their progress. SWF ensures that a task is assigned only once and is never duplicated. Since AWS maintains the application's state durably, workers and deciders don't have to keep track of execution state. They can run independently and scale quickly

### SWF Domains
* Your workflow and activity types and the workflow execution itself are all scoped to a domain. Domains isolate a set of types, executions, and task lists from others within the same account
* The parameters are specified in JSON format

### How long for workflows?
Maximum workflow can be one year and the value is always measured in seconds

### SWF vs SQS
* SWF presents a task-oriented API, whereas SQS offers a message-oriented API
* SWF ensures that a task is assigned only once and is never duplicated, with SQS you need to handle duplicated messages and may also need to ensure that a message is processed only once
* SWF keeps track of all the task and events in an application with SQS you need to implement you own application-level tracking, especially if your application uses multiple queues

### What is SNS?
* AWS SNS (Simple Notification Service) is a web service that makes it easy to set up, operate, and send notifications from the cloud. It provides developers with highly scalable, flexibile, and cost-effective capability to publish messages from an application and immediately deliver them to subscribers or other applications

* SNS allows you to group multiple recipients using topics. Topic is an "access point" for allowing recipients to dynamically subscribe for identical copies of the same notification. One topic can support deliveries to multiple endpoint types

* To prevent messages from being lost, all messages published to SNS are stored redundantly across multiple AZs

### SNS Benefits
* Instantaneous, push-based delivery (no polling)
* Simple APIs and easy integration with applications
* Flexible message delivery over multiple transport protocols
* Inexpensive, pay-as-you-go model with no up-front costs
* Web-based AWS management console offers the simplicity of a point-and-click interface

### SNS vs SQS
* Both messaging services in AWS
* SNS - Push
* SQS - Polls (Pulls)

### SNS Pricing
* User pay $0.50 per 1 million Amazon SNS Request
* $0.06 per 100,000 notification deliveries over HTTP
* $0.75 per 100 notification deliveries over SMS
* $2.00 per 100,000 notification deliveries over Email

### Elastic Transcoder
* Media transcoder in the cloud
* Convert media files from their original source format in to different formats that will play on smartphones, tablets, PCs, etc
* Provides transcoding presets for popular output formats, which means that you do not need to guess about which settings work best on particular devices
* Pay based on the minutes that you transcode and the resolution at which you transcode

### What is API Gateway?
API Gateway is a fully managed service that makes it easy for developers to publish, maintain, monitor, and secure APIs at any scale.

### What is API Caching?
API caching can reduce the number of calls made to your endpoint and also improve latency of the requests to your API. When you enable caching for a stage, API Gateway caches responses from your endpoint for a specified TTL (time-to-live) period, in seconds. API Gateway then responds to the request by looking up the endpoint response from the cache instead of making a request to your endpoint.

### What can API Gateway do?
* Low cost and efficient
* Scales effortlessly
* You can throttle requests to prevent attacks
* Connect to CloudWatch to log all requests

### Same Origin Policy
In computing, the same-origin policy (web app security model) states that a web browser permits scripts contained in a first web page to access data in a second web page but only if both web pages have the same origin.

### Cross-Origin Resource Sharing (CORS)
* CORS is one way the server at the other end (not the client code in the brower) can relax the same-origin policy
* Cross-origin resource sharing (CORS) is a mechanism that allows restricted resources (e.g. fonts) on a web page to be requested from another domain outside the domain from which the first resource was served
* Error - "Origin policy cannot be read at the remote resource?" - You need to enable CORS on API Gateway

### Exam Tips - API Gateway
* Remember what API Gateway is at a high level
* API Gateway has caching capabilities to increase performance
* API Gateway is low cost and scales automatically
* You can throttle API Gateway to prevent attacks
* You can log results to CloudWatch
* If you are using JavaScript/AJAX that uses multiple domains with API Gateway, ensure that you have enabled CORS on API Gateway

### What is streaming data?
* Streaming data is data that is generated continuously by thousands of data sources, which typically send in the data records simultaneously and in small sizes (KB)
* Streaming data includes:
    * Purchases from online stores
    * Stock prices
    * Game data
    * Social network data
    * Geospatial data
    * IoT sensor data

### What is Kinesis?
Amazon Kinesis is a platform on AWS to send your streaming data to. Kinesis makes it easy to load and analyze streaming data.

### What are the core Kinesis Services?
* Kinesis Streams
* Kinesis Firehose
* Kinesis Analytics

### Kinesis Streams
* Kinesis Streams consist of shards
    * Five transactions per second for reads, up to a maximum total data read rate of two 2 Mbps and up to 1,000 records per second for writes, up to a maximum toala data write rate of 1 Mbps
    * The data capacity of your stream is a function of the number of shards that you specify for the stream. The total capcity of the stream is the sum of the capacities of its shards

### Kinesis Firehose
Amazon Kinesis Data Firehose is the easiest way to reliably load streaming data into data stores and analytics tools. It can capture, transform, and load streaming data into Amazon S3, Amazon Redshift, Amazon Elasticsearch Service, and Splunk, enabling near real-time analytics with existing business intelligence tools and dashboards you’re already using today. It is a fully managed service that automatically scales to match the throughput of your data and requires no ongoing administration. It can also batch, compress, transform, and encrypt the data before loading it, minimizing the amount of storage used at the destination and increasing security.

### Kinesis Analytics
Amazon Kinesis Data Analytics is the easiest way to process streaming data in real time with standard SQL without having to learn new programming languages or processing frameworks. Amazon Kinesis Data Analytics enables you to query streaming data or build entire streaming applications using SQL, so that you can gain actionable insights and respond to your business and customer needs promptly.

### Exam Tips - Kinesis
* Know the difference between Kinesis Streams and Kinesis Firehose
* Understand what Kinesis Analytics is

## Section 9 Quiz

**1. What does Amazon SWF stand for?**
* Simple Work Flow

**2. What does Amazon SES stand for?**
* Simple Email Service

**3. What happens when you create a topic on Amazon SNS?**
* An Amazon Resource Name is created

**4. What is the difference between SNS and SQS?**
* SNS is a push notification service, whereas SQS is a message systemn that requires worker nodes to poll the queue

**5. What application service allows you to decouple your infrastructure using messaged based queues?**
* SQS

**6. What does a "domain" refer to in Amazon SWF?**
* A collection of related workflows

**7. By default, EC2 instances pull SQS messages from an SQS queue on a FIFO (First In First out) basis.**
* False

**8. Amazon's SQS service guarantees a message will be delivered at least once.**
* True

**9. Amazon SWF ensures that a task is assigned only once and is never duplicated.**
* True

**10. Amazon SWF restricts individuals to use specific programming languages.**
* False

---
