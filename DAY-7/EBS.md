# EBS

## What is AWS EBS?
Amazon Elastic Block Store (EBS) is a block-level storage service provided by AWS.
It is primarily used to store data for EC2 instances (Virtual Servers) in AWS. EBS volumes can be attached to EC2 instances to provide persistent storage, meaning the data remains even if the EC2 instance is stopped or terminated.

## Key Concepts
EBS Volumes: These are virtual disks that you attach to EC2 instances. They appear as block devices, similar to hard drives, but they reside in the cloud.

Persistence: Data stored in EBS volumes remains intact after you stop or terminate your EC2 instance (unlike instance store volumes, which are temporary).

Snapshots: You can create backups of EBS volumes using snapshots, which can be stored in Amazon S3. Snapshots allow you to restore the data or create new volumes from them.

Performance: EBS provides various volume types that vary in performance, including General Purpose SSD (gp2, gp3), Provisioned IOPS SSD (io1, io2), and Magnetic (st1, sc1).

## Volume Types
General Purpose SSD (gp2/gp3): Good for most workloads, like boot volumes and small-to-medium databases.

Provisioned IOPS SSD (io1/io2): High-performance volumes for workloads that require low latency and high throughput (e.g., large databases).

Throughput Optimized HDD (st1): Designed for workloads with large, sequential I/O, such as big data or log processing.

Cold HDD (sc1): Ideal for infrequently accessed data like backups.

Magnetic (standard): Older, lower-cost option. Rarely used now in modern environments.

## How to Create and Attach an EBS Volume
### Create a Volume

Go to the EC2 dashboard in AWS Management Console.

Select Volumes from the sidebar, then click Create Volume.

Choose the volume type, size, and availability zone (must match the EC2 instance's zone).

### Attach the Volume

Select the created volume, click Actions, and select Attach Volume.
Select the instance to attach it to and assign a device name (e.g., /dev/sdf).
Mount the Volume (after attachment)

### Log into the EC2 instance and mount the volume on the operating system