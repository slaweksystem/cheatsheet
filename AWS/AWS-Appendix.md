# AWS SCOPE

## Appendix

In-scope AWS services and features
The following list contains AWS services and features that are in scope for the exam.
This list is non-exhaustive and is subject to change. AWS offerings appear in
categories that align with the offerings’ primary functions:

## Analytics

- Amazon OpenSearch Service
Application Integration:
- Amazon EventBridge - Pomaga w budowaniu architektury eventowej. Mozna triggerowac eventy w taki czy inny sposób.
  - Amazon EventBridge Event Bus is a serverless event bus that helps you receive, filter, transform, route, and deliver events.
- Amazon Simple Notification Service (Amazon SNS) Fully managed Pub/Sub service for A2A (Application 2 Application)and A2P(Application 2 Person) messaging
- Amazon Simple Queue Service (Amazon SQS)

## Cloud Financial Management

- AWS Cost and Usage Report  
The AWS Cost and Usage Report (CUR) provides the most detailed information available about your AWS costs and usage. It breaks down your costs by the hour, day, and month, and by each service and usage type. This report is useful for analyzing spending patterns, optimizing your costs, and gaining insights into your AWS bill.

- AWS Cost Explorer  
AWS Cost Explorer is a tool that allows you to visualize and manage your AWS costs and usage over time. It provides a set of preconfigured views that help you identify trends, detect anomalies, and understand your spending patterns. You can create custom reports, forecast future costs, and receive cost-saving recommendations through its intuitive interface.

- Savings Plans  
  Savings Plans are flexible pricing models that provide significant savings on AWS usage in exchange for a commitment to use a specific amount of compute power (measured in $/hour) for a one- or three-year term. There are two types of Savings Plans:

  - Compute Savings Plans: Offer the most flexibility and apply automatically to any EC2 instance usage, regardless of region, instance family, operating system, or tenancy.
  - EC2 Instance Savings Plans: Provide the lowest prices but are specific to a particular instance family and region, with more restrictions compared to Compute Savings Plans.
These plans help reduce costs by offering lower prices on AWS services in return for consistent usage.

## Compute

- AWS Auto Scaling
AWS Auto Scaling helps you ensure that you have the right number of Amazon EC2 instances available to handle the load for your application. It automatically adjusts the number of instances in a group based on your specified policies, scaling up during demand spikes and scaling down during lulls to optimize costs.

- Amazon EC2
  Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. It allows you to run virtual servers (instances) on demand, providing the scalability and flexibility to build and deploy applications quickly and efficiently. You can choose from various instance types optimized for different use cases, including compute, memory, and storage-intensive applications.

- Amazon EC2 Auto Scaling
  Amazon EC2 Auto Scaling is a feature within EC2 that allows you to automatically increase or decrease the number of EC2 instances based on criteria you define. This ensures that you have the optimal number of instances to handle the load of your applications, maintaining performance and cost-efficiency. It can automatically replace unhealthy instances and maintain application availability.

- Amazon EC2 Image Builder
  Amazon EC2 Image Builder is a service that simplifies the creation, maintenance, and deployment of customized EC2 machine images. It provides a graphical interface and automation features to create images that include your application code, runtime environment, and security configurations. This helps ensure consistency and compliance across multiple EC2 instances.

- AWS Lambda
  AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. You can execute your code in response to events, such as changes in data, system state, or user actions, and Lambda automatically manages the compute resources required. It supports various programming languages and scales automatically to accommodate the workload.

## Database

- Amazon Aurora
  Amazon Aurora is a fully managed relational database engine that is compatible with MySQL and PostgreSQL. It provides performance and availability similar to commercial databases at a fraction of the cost. Aurora is designed for high durability and availability, with replication across multiple Availability Zones and continuous backups to Amazon S3.

- Amazon DynamoDB
  Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. It allows you to offload the administrative burdens of operating and scaling distributed databases so that you don't have to worry about hardware provisioning, setup, and configuration, replication, software patching, or cluster scaling.

- Amazon ElastiCache
  Amazon ElastiCache is a fully managed in-memory data store and cache service that supports two open-source caching engines: Redis and Memcached. It improves the performance of web applications by retrieving data from high-throughput, low-latency in-memory data stores, reducing the need for slower disk-based databases.

- Amazon RDS
  Amazon Relational Database Service (Amazon RDS) is a managed service that makes it easy to set up, operate, and scale a relational database in the cloud. It supports several database engines, including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, and SQL Server. RDS automates common administrative tasks such as backups, patching, and hardware provisioning, allowing you to focus on your applications.

## Developer Tools

AWS provides a variety of tools and SDKs to help developers manage and interact with AWS services. Here are brief descriptions:

- AWS Command Line Interface (CLI)
 The AWS CLI is a unified tool that allows you to manage your AWS services from the command line. It provides commands for interacting with AWS services, enabling you to automate them through scripts. The CLI supports a wide range of operations and is available on multiple platforms, including Windows, macOS, and Linux.
- AWS Software Development Kits (SDKs)
  AWS SDKs provide a set of libraries and tools for various programming languages that simplify the process of integrating and using AWS services within your applications. SDKs are available for many popular languages, including:
  - AWS SDK for Java: Provides Java APIs for interacting with AWS services.
  - AWS SDK for Python (Boto3): Offers Python APIs for AWS services.
  - AWS SDK for JavaScript: Enables JavaScript developers to use AWS services in both browser and server-side environments.
  - AWS SDK for .NET: Provides .NET APIs for AWS services.
  - AWS SDK for Ruby: Offers Ruby APIs for AWS services.
  - AWS SDK for PHP: Provides PHP APIs for AWS services.
  - AWS SDK for Go: Offers Go APIs for AWS services.
  - AWS SDK for C++: Provides C++ APIs for AWS services.
  - AWS CloudFormation

- AWS CloudFormation allows you to define and provision AWS infrastructure as code. Using a simple text file, you can model and set up all the resources needed for your applications across all regions and accounts. CloudFormation automates the provisioning and updating of infrastructure in a safe and controlled manner.
- AWS Cloud Development Kit (CDK)
  AWS CDK is an open-source software development framework that allows you to define cloud infrastructure using familiar programming languages. It provides high-level components called constructs that preconfigure cloud resources with proven defaults, making it easier to build and manage your AWS infrastructure.

- AWS Elastic Beanstalk
  AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services. It supports various platforms, including Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker. Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, and auto-scaling to application health monitoring.

- AWS CodeStar
  AWS CodeStar provides a unified user interface, enabling you to easily manage software development activities in one place. It integrates with various AWS services like CodeCommit, CodeBuild, CodeDeploy, and CodePipeline, simplifying the process of setting up your entire continuous delivery toolchain.

These tools and SDKs facilitate the development, deployment, and management of applications on AWS, providing a wide range of functionalities to cater to different programming languages and use cases.

## Management and Governance

- AWS CLI
  The AWS Command Line Interface (CLI) is a unified tool for managing AWS services from the command line. It provides commands for a wide range of AWS services, enabling you to automate operations and manage your infrastructure using scripts.

- AWS CloudFormation
  AWS CloudFormation allows you to define and provision AWS infrastructure as code using simple text files (JSON or YAML). It automates the setup and configuration of resources, ensuring consistent and repeatable deployments across multiple environments.

- AWS CloudTrail
  AWS CloudTrail is a service that enables governance, compliance, and operational and risk auditing of your AWS account. It records AWS API calls and events for your account, providing a history of actions taken, which helps in troubleshooting, security analysis, and compliance auditing.

- Amazon CloudWatch
  Amazon CloudWatch is a monitoring and observability service that provides data and actionable insights for AWS, hybrid, and on-premises applications and infrastructure resources. It collects and tracks metrics, logs, and event data, enabling you to monitor applications, respond to system-wide performance changes, and optimize resource utilization.

- AWS Compute Optimizer
  AWS Compute Optimizer recommends optimal AWS resources for your workloads to reduce costs and improve performance. It analyzes historical utilization metrics and provides recommendations for Amazon EC2 instances, Auto Scaling groups, EBS volumes, and Lambda functions.

- AWS Config
  AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. It continuously monitors and records AWS resource configurations and allows you to automate the evaluation of recorded configurations against desired configurations.

- AWS Control Tower
  AWS Control Tower offers a straightforward way to set up and govern a secure, multi-account AWS environment based on AWS best practices. It provides a landing zone, automates the setup of an environment, and implements governance controls for ongoing operations.

- AWS Health Dashboard
  AWS Health Dashboard provides personalized information about the health of your AWS services and resources. It offers detailed insights into the performance and availability of your services, including real-time alerts and notifications.

- AWS License Manager
  AWS License Manager helps you manage software licenses from vendors like Microsoft, SAP, Oracle, and IBM across AWS and on-premises environments. It simplifies the tracking and compliance of your licenses, reducing the risk of non-compliance and unnecessary costs.

- AWS Management Console
  The AWS Management Console is a web-based interface for accessing and managing AWS services. It provides an intuitive user interface to manage your cloud resources, launch and configure services, monitor your account, and automate tasks using the console's integrated features.

- AWS Organizations
  AWS Organizations helps you centrally manage and govern your environment as you grow and scale your AWS resources. It allows you to create multiple AWS accounts and consolidate them into an organizational structure for easier management, applying policies, and automating account creation and management.

- AWS Service Catalog
  AWS Service Catalog allows organizations to create and manage catalogs of IT services that are approved for use on AWS. It enables you to centrally manage commonly deployed IT services, ensuring compliance with business requirements, and helping users quickly find and deploy approved services.

- AWS Systems Manager
  AWS Systems Manager provides a unified interface to view and control your AWS infrastructure. It offers operational data from multiple AWS services and allows you to automate tasks such as patch management, software inventory, and configuration management across your resources.

- AWS Trusted Advisor
  AWS Trusted Advisor is an online resource that provides real-time guidance to help you provision your resources following AWS best practices. It offers recommendations in areas such as cost optimization, performance, security, fault tolerance, and service limits to help you optimize your AWS environment.

## Migration and Transfer

- AWS DataSync
  AWS DataSync is a managed service that simplifies, automates, and accelerates the process of moving large amounts of data between on-premises storage and AWS storage services, as well as between AWS storage services themselves. It can transfer data to and from Amazon S3, Amazon EFS, and Amazon FSx for Windows File Server, providing encryption and data integrity validation during the transfer process.

- AWS Transfer Family
  AWS Transfer Family is a suite of fully managed services that enable you to transfer files directly into and out of Amazon S3 or Amazon EFS using the Secure File Transfer Protocol (SFTP), File Transfer Protocol over SSL (FTPS), and File Transfer Protocol (FTP). It allows you to easily migrate, automate, and monitor file transfers without needing to modify existing applications or manage file transfer infrastructure.

## Networking and Content Delivery

- Amazon CloudFront
  Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency and high transfer speeds. CloudFront integrates with AWS services such as Amazon S3, AWS Shield, AWS WAF, and Amazon Route 53.

- Elastic Load Balancing (ELB)
  Elastic Load Balancing (ELB) automatically distributes incoming application traffic across multiple targets, such as EC2 instances, containers, IP addresses, and Lambda functions. ELB supports three types of load balancers: Application Load Balancer (for HTTP/HTTPS traffic), Network Load Balancer (for TCP/UDP/TLS traffic), and Gateway Load Balancer (for third-party virtual appliances).

- AWS Global Accelerator
  AWS Global Accelerator is a networking service that improves the availability and performance of your applications with global users. It provides two static IP addresses that act as a fixed entry point to your application endpoints, such as EC2 instances, load balancers, and S3 buckets, routing traffic to the optimal endpoint based on performance, health, and geographic location.

- Amazon Route 53
  Amazon Route 53 is a scalable and highly available Domain Name System (DNS) web service designed to route end-user requests to internet applications running in AWS. It provides domain registration, DNS routing, and health checking to ensure that your application remains available and responsive.

- AWS Transit Gateway
  AWS Transit Gateway enables you to connect your Amazon Virtual Private Clouds (VPCs) and on-premises networks through a central hub. This simplifies your network architecture and streamlines cross-VPC and cross-account connectivity, as well as hybrid workloads.

- Amazon VPC
  Amazon Virtual Private Cloud (VPC) allows you to provision a logically isolated section of the AWS cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including IP address ranges, subnets, route tables, and network gateways.

- AWS VPN
  AWS VPN (Virtual Private Network) allows you to establish secure and private connections from your on-premises networks or client devices to your AWS environment. It includes two services: AWS Site-to-Site VPN, which connects your on-premises network to an AWS VPC over an IPsec VPN connection, and AWS Client VPN, which enables your users to securely access AWS resources from any location using OpenVPN-based clients.

## Security, Identity, and Compliance

- AWS Certificate Manager (ACM)
  AWS Certificate Manager (ACM) is a service that lets you easily provision, manage, and deploy SSL/TLS certificates for use with AWS services and your internal connected resources. ACM handles the complexity of creating and maintaining certificates, including renewal and deployment.

- Amazon Detective
  Amazon Detective simplifies the process of investigating security issues across your AWS workloads. It automatically collects log data from your AWS resources and uses machine learning, statistical analysis, and graph theory to build a linked set of data that helps you conduct faster and more efficient security investigations.

- AWS Directory Service
  AWS Directory Service provides multiple ways to set up and run Microsoft Active Directory (AD) on AWS. It supports AWS Managed Microsoft AD, which is a managed Active Directory in the AWS Cloud, as well as AD Connector, which allows you to connect your existing on-premises AD to AWS, and Simple AD, a standalone managed directory.

- AWS Firewall Manager
  AWS Firewall Manager is a security management service that makes it easier to centrally configure and manage AWS WAF rules across your accounts and applications. It ensures that all security policies are consistently enforced across all resources, simplifying compliance and security management.

- Amazon GuardDuty
  Amazon GuardDuty is a threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts, workloads, and data. It uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats.

- AWS Identity and Access Management (IAM)
  AWS Identity and Access Management (IAM) enables you to manage access to AWS services and resources securely. With IAM, you can create and manage AWS users and groups and use permissions to allow and deny their access to AWS resources.

- AWS Identity and Access Management Access Analyzer
  AWS IAM Access Analyzer helps you identify the resources in your organization and accounts that are shared with an external entity. It continuously monitors resource policies and generates findings to help you identify and remediate unintended access.

- Amazon Inspector
  Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. It automatically assesses applications for vulnerabilities or deviations from best practices and provides detailed findings on security issues.

- AWS Key Management Service (AWS KMS)
  AWS Key Management Service (KMS) is a managed service that enables you to create and control the encryption keys used to encrypt your data. KMS integrates with most AWS services to make it easy to encrypt data you store and manage across AWS.

- AWS Secrets Manager
  AWS Secrets Manager helps you protect access to your applications, services, and IT resources without the upfront cost and operational overhead of managing your own hardware security module (HSM) infrastructure. It enables you to rotate, manage, and retrieve database credentials, API keys, and other secrets throughout their lifecycle.

- AWS Security Hub
  AWS Security Hub provides a comprehensive view of your high-priority security alerts and compliance status across AWS accounts. It aggregates, organizes, and prioritizes your security findings from multiple AWS services and AWS Partner solutions, helping you monitor your environment more effectively.

- AWS Shield
  AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards web applications running on AWS. It comes in two tiers: Shield Standard, which provides protection against most common attacks, and Shield Advanced, which offers additional detection and mitigation capacity, 24/7 access to the AWS DDoS Response Team, and protection against financial impact.

- AWS WAF
  AWS WAF (Web Application Firewall) helps protect your web applications from common web exploits and vulnerabilities that could affect availability, compromise security, or consume excessive resources. You can create custom security rules that control bot traffic and block common attack patterns such as SQL injection and cross-site scripting (XSS).

## Storage

- AWS Backup
  AWS Backup is a fully managed service that centralizes and automates the backup of data across AWS services. It simplifies and consolidates the process of backing up your AWS resources, such as Amazon EC2 instances, Amazon EBS volumes, Amazon RDS databases, Amazon DynamoDB tables, Amazon EFS file systems, and AWS Storage Gateway volumes, helping you meet your business and regulatory backup compliance requirements.

- Amazon Elastic Block Store (Amazon EBS)
  Amazon Elastic Block Store (Amazon EBS) provides block-level storage volumes for use with Amazon EC2 instances. EBS volumes are highly available and reliable storage volumes that can be attached to any running instance in the same Availability Zone, offering consistent and low-latency performance.

- Amazon Elastic File System (Amazon EFS)
  Amazon Elastic File System (Amazon EFS) provides simple, scalable, and fully managed elastic NFS (Network File System) file storage for use with AWS Cloud services and on-premises resources. EFS automatically grows and shrinks as you add and remove files, providing unlimited capacity and supporting thousands of concurrent connections.

- Amazon FSx
  Amazon FSx provides fully managed third-party file systems, optimized for a variety of workloads:

  - Amazon FSx for Windows File Server: Delivers a fully managed native Windows file system with features such as user quotas, end-user file restore, and Microsoft Active Directory integration.
  - Amazon FSx for Lustre: Provides a high-performance file system for compute-intensive workloads, tightly integrated with Amazon S3, enabling you to process cloud datasets quickly and cost-effectively.
  - Amazon FSx for NetApp ONTAP: Combines the popular features of ONTAP file systems with AWS’s agility, scalability, and cost-efficiency.
  - Amazon FSx for OpenZFS: Offers a high-performance file system based on the open-source OpenZFS file system, providing robust data management capabilities.

- Amazon S3
  Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. S3 provides durable and secure storage for a wide range of data types, with a simple web services interface to store and retrieve any amount of data from anywhere on the web.

- Amazon S3 Glacier
  Amazon S3 Glacier and S3 Glacier Deep Archive are secure, durable, and extremely low-cost storage services for data archiving and long-term backup. Glacier is optimized for infrequent access, offering retrieval times from minutes to hours, while Glacier Deep Archive provides the lowest-cost storage for long-term retention with retrieval times within 12 hours.

- AWS Storage Gateway
  AWS Storage Gateway is a hybrid cloud storage service that enables your on-premises applications to seamlessly use AWS cloud storage. It offers three different types of gateways:

  - File Gateway: Presents a file-based interface and provides seamless integration with Amazon S3.
  - Tape Gateway: Allows you to archive backup data in the cloud using your existing tape-based backup infrastructure.
  - Volume Gateway: Provides block storage volumes that can be backed up to Amazon S3 and restored to on-premises or in AWS.

These services provide various storage solutions tailored to different needs, from high-performance file systems to long-term archival storage.

## Out-of-scope AWS services and features

The following list contains AWS services and features that are out of scope for the
exam. This list is non-exhaustive and is subject to change. AWS offerings that are
entirely unrelated to the target job roles for the exam are excluded from this list:

## Analytics out

- Amazon EMR

## Business Applications out

- Amazon Chime
- Amazon Connect
- Amazon WorkDocs
- Amazon WorkMail

## Compute out

- Amazon Lightsail

## Containers out

- Amazon Elastic Container Registry (Amazon ECR)
- Amazon Elastic Container Service (Amazon ECS)

## Database out

- Amazon Redshift

## Developer Tools out

- AWS CodeBuild
- AWS CodeCommit
- AWS CodeDeploy
- AWS CodeStar
- AWS X-Ray

End User Computing:

- Amazon AppStream 2.0
- Amazon WorkSpaces

Frontend Web and Mobile:

- AWS Device Farm
- AWS Mobile SDKs
- Amazon Pinpoint

Game Tech:

- Amazon GameLift

Internet of Things (IoT):

- AWS IoT Button
- AWS IoT Greengrass
- AWS IoT Platform

Machine Learning:

- AWS Deep Learning AMIs (DLAMI)
- Amazon Lex
- Amazon Lumberyard
- Amazon Machine Learning (Amazon ML)
- Apache MXNet on AWS
- Amazon Polly
- Amazon Rekognition

Management and Governance:

- AWS Managed Services (AMS)

Media Services:

- Amazon Elastic Transcoder

Migration and Transfer:

- AWS Schema Conversion Tool (AWS SCT)

Security, Identity, and Compliance:

- Amazon Cloud Directory

Storage:

- AWS Snowmobile