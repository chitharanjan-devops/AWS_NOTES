# AWS Networking Concepts

## 1. AWS Region
An AWS Region is a geographical location where AWS has multiple data centers. Each region operates independently to provide high availability and fault tolerance.

🔹 Example:
us-east-1 (N. Virginia)
us-west-2 (Oregon)
ap-south-1 (Mumbai)

✅ Best Practices:
Choose a region close to users for lower latency.


## 2. Availability Zone (AZ)
An Availability Zone (AZ) is a physically isolated data center within a region. AWS regions have multiple AZs to provide fault tolerance.

🔹 Example:
us-east-1a, us-east-1b, us-east-1c (Three AZs in N. Virginia Region)

✅ Best Practices:
Deploy resources in multiple AZs for high availability


## 3. Virtual Private Cloud (VPC)
AWS VPC (Virtual Private Cloud) is a logically isolated network in AWS, where users can deploy AWS resources securely.

🔹 Key Components of a VPC:
CIDR Block – Defines the IP range (e.g., 10.0.0.0/16).
Subnets – Divide the VPC into smaller networks.
Internet Gateway (IGW) – Provides internet access.
Route Tables – Control traffic flow.

✅ Best Practices:
Use separate VPCs for different environments (Production, Testing, Dev).
Implement VPC Peering to connect multiple VPCs securely.


## 4. Internet Gateway (IGW)
An Internet Gateway (IGW) allows traffic from a VPC to access the internet and enables external users to access resources in a public subnet.

🔹 Key Points:
It is attached to a VPC to provide internet connectivity.
Works with route tables to allow external traffic.

✅ Best Practices:
Attach only one IGW per VPC.


## 5. Route Table
A Route Table defines how network traffic flows inside a VPC. It contains rules (routes) that determine how requests are forwarded.

🔹 Key Points:
Each subnet must be associated with a route table.
Route tables contain destination (CIDR) and target (next hop).

✅ Best Practices:
Default route table applies to all subnets unless overridden.
Use custom route tables for private and public subnets.

## 6. Public Subnet
A Public Subnet is a subnet that has direct internet access via an Internet Gateway (IGW).

🔹 Key Requirements for a Public Subnet:
The subnet must be associated with a route table pointing to the IGW.
EC2 instances in the public subnet must have Elastic IP or Public IP.

🔹 Example Public Subnet CIDR Block:
10.0.1.0/24 (A small portion of the VPC 10.0.0.0/16)

✅ Best Practices:
Place web servers in a public subnet.



 ![Image Description](/Images/VPC-Intro.jpg)
