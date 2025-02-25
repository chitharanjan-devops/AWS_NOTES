#  Amazon EC2 (Elastic Compute Cloud)
Amazon EC2 is a cloud-based virtual server that allows you to run applications without maintaining physical hardware.

You can launch different types of instances based on your needs (CPU, RAM, storage, etc.).

EC2 instances are scalable, meaning you can increase or decrease resources as required.

Instances are billed on a pay-as-you-go model.

## EC2 Instance Types
EC2 instances come in different types optimized for various workloads

General Purpose – Balanced CPU & Memory (e.g., t3.micro, t3.large)

Compute Optimized – High-performance CPU (e.g., c5.large, c5.xlarge)

Memory Optimized – Large RAM (e.g., r5.large, x1e.2xlarge)

Storage Optimized – High disk throughput (e.g., i3.large, d2.xlarge)

GPU Instances – Used for ML, gaming (e.g., p3.large, g4dn.xlarge)

## EC2 Key Pair
A Key Pair (Public & Private Key) is used to securely connect to EC2 instances.

AWS stores the Public Key, and you download the Private Key (.pem file).

You use this key with SSH to log in:

```ssh -i <your-key.pem> ec2-user@your-instance-ip```

Losing the private key means you cannot access the instance.

## What is User Data in EC2?
User Data is a script or set of commands that you can pass to an EC2 instance during its launch. It is used to automate initial configurations, install software, and execute scripts when the instance starts for the first time.

### Basic User Data Script for Linux
This example installs Apache Web Server automatically on an Amazon Linux instance
```bash
#!/bin/bash
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
echo "<h1>Welcome to EC2</h1>" > /var/www/html/index.html