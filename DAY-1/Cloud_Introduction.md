# Introduction to Cloud Computing

## What is Cloud Computing?
Cloud computing is the delivery of computing services—such as servers, storage, databases, networking, software, and more—over the internet ("the cloud"). Instead of owning and maintaining physical infrastructure, users can access computing resources on-demand from cloud providers.

## Key Characteristics of Cloud Computing
1. On-Demand Self-Service – Users can provision resources as needed without human intervention.
2. Broad Network Access – Cloud services are accessible over the internet from anywhere.
3. Resource Pooling – Computing resources are shared among multiple users dynamically.
4. Rapid Elasticity – Resources can scale up or down based on demand.
5. Measured Service – Users pay only for the resources they use (pay-as-you-go model).

## Types of Cloud Computing
1. Public Cloud – Services are offered over the internet by third-party providers (e.g., AWS, Azure, Google Cloud).
2. Private Cloud – Dedicated infrastructure for a single organization, offering better control and security.
3. Hybrid Cloud – A combination of public and private clouds, allowing data and applications to be shared between them.

## Cloud Service Models
1. Infrastructure as a Service (IaaS) – Provides virtualized computing resources like servers, storage, and networking (e.g., AWS EC2, Google Compute Engine).
2. Platform as a Service (PaaS) – Offers a platform for developers to build and deploy applications (e.g., AWS Elastic Beanstalk, Google App Engine).
3. Software as a Service (SaaS) – Delivers software applications over the internet (e.g., Gmail, Dropbox, Microsoft 365).

## Benefits of Cloud Computing
Cost Efficiency – No need for upfront investment in hardware.

Scalability – Easily scale resources up or down.

Flexibility – Access resources from anywhere.
Security & Reliability – Cloud providers offer advanced security features and backup options.

Automatic Updates – Providers handle maintenance and software updates


# Introduction to AWS
## 1. What is AWS?
Amazon Web Services (AWS) is a cloud computing platform provided by Amazon. It offers a wide range of services such as computing power, storage, databases, networking, and security. AWS enables businesses and developers to build, deploy, and manage applications efficiently without investing in physical infrastructure.

## Key Features of AWS
Scalability – Resources can be scaled up or down as per demand.
Cost-Effective – Pay-as-you-go pricing model.
Security – Built-in security features and compliance with global standards.
Flexibility – Supports multiple programming languages and platforms.
Global Reach – Available in multiple regions worldwide.

## 2. AWS Global Infrastructure
AWS operates in different locations worldwide. Understanding the AWS infrastructure is crucial for designing scalable and resilient applications.

### Key Components:
Regions – A geographical area containing multiple AWS data centers.
Availability Zones (AZs) – Data centers within a region that provide redundancy.
Edge Locations – Used by AWS CloudFront for content delivery and caching.
📌 Example: A company hosting a website on AWS should choose a region closest to its users for better performance.

## 3. AWS Core Services
AWS provides a wide range of services categorized into different domains:

## A. Compute Services
Amazon EC2 (Elastic Compute Cloud) – Virtual servers in the cloud.
AWS Lambda – Serverless compute service that runs code in response to events.
Amazon ECS (Elastic Container Service) – Manages Docker containers.
Amazon EKS (Elastic Kubernetes Service) – Manages Kubernetes clusters.


## B. Storage Services
Amazon S3 (Simple Storage Service) – Scalable object storage.
Amazon EBS (Elastic Block Store) – Persistent storage for EC2.
Amazon EFS (Elastic File System) – Scalable file storage.
AWS Backup – Centralized backup service.


## C. Database Services
Amazon RDS (Relational Database Service) – Managed database service for MySQL, PostgreSQL, MariaDB, Oracle, and SQL Server.
Amazon DynamoDB – Fully managed NoSQL database.
Amazon Redshift – Data warehousing service.
Amazon Aurora – High-performance relational database.


## D. Networking & Content Delivery
Amazon VPC (Virtual Private Cloud) – Isolated cloud environment.
AWS Route 53 – Domain Name System (DNS) service.
AWS CloudFront – Content delivery network (CDN).
AWS Direct Connect – Dedicated network connection to AWS.


## E. Security & Identity
AWS IAM (Identity and Access Management) – Manages user permissions.
AWS KMS (Key Management Service) – Encryption key management.
AWS WAF (Web Application Firewall) – Protects applications from attacks.
AWS Shield – DDoS protection service.


## 4. AWS Billing & Pricing
AWS follows a pay-as-you-go model, meaning you pay only for what you use.

Pricing Models:
On-Demand – Pay for what you use, no long-term commitment.
Reserved Instances – Commit for 1-3 years for a discount.
Spot Instances – Purchase unused capacity at lower prices.
Savings Plans – Flexible pricing model based on usage commitment.


## 5. AWS Management & Monitoring
AWS CloudWatch – Monitoring service for logs and performance metrics.
AWS CloudTrail – Logs all AWS API calls for auditing.
AWS Config – Tracks changes in AWS resources.
AWS Trusted Advisor – Provides recommendations for security and cost optimization.