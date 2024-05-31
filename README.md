# Capstone Project: WordPress Site on AWS

## Project Scenario
A small to medium-sized digital marketing agency, "DigitalBoost", aimed to enhance its online presence by creating a high-performance WordPress-based website for their clients. The agency required a scalable, secure, and cost-effective solution that could handle increasing traffic and integrate seamlessly with their existing infrastructure. As an AWS Solutions Architect, I designed and implemented a WordPress solution using various AWS services, such as Networking, Compute, Object Storage, and Databases.

## Project Overview
This project involved setting up a WordPress-based website using AWS services. The architecture included a Virtual Private Cloud (VPC), a managed MySQL database using Amazon RDS, scalable storage using Amazon Elastic File System (EFS), and an Application Load Balancer (ALB) with an Auto Scaling Group (ASG) for high availability and fault tolerance.

## Project Deliverables
1. **Documentation:**
   - Detailed documentation for each component setup.
   - Explanation of security measures implemented.
2. **Demonstration:**
   - Live demonstration of the WordPress site.
   - Showcased auto-scaling by simulating increased traffic.

## Components and Setup

### 1. Virtual Private Cloud (VPC)
**Objective:** Create a VPC to isolate and secure the WordPress infrastructure.

**Steps:**
1. Defined IP address range for the VPC.
2. Created the VPC with public and private subnets.
3. Configured route tables for each subnet.

### 2. Secure Network Architecture
**Objective:** Set up a secure network architecture with public and private subnets. Used a NAT Gateway for private subnet internet access.

**Steps:**
1. Set up public subnets for resources accessible from the internet.
2. Created private subnets for resources with no direct internet access.
3. Configured a NAT Gateway for private subnet internet access.

### 3. Managed MySQL Database using Amazon RDS
**Objective:** Deploy a managed MySQL database using Amazon RDS for WordPress data storage.

**Steps:**
1. Created an Amazon RDS instance with MySQL engine.
2. Configured security groups for the RDS instance.
3. Connected WordPress to the RDS database.

### 4. Amazon Elastic File System (EFS) for WordPress Files
**Objective:** Use Amazon Elastic File System (EFS) to store WordPress files for scalable and shared access.

**Steps:**
1. Created an EFS file system.
2. Mounted the EFS file system on WordPress instances.
3. Configured WordPress to use the shared file system.

### 5. Application Load Balancer (ALB)
**Objective:** Distribute incoming traffic among multiple instances to ensure high availability and fault tolerance.

**Steps:**
1. Created an Application Load Balancer.
2. Configured listener rules for routing traffic to instances.
3. Integrated the Load Balancer with an Auto Scaling group.

### 6. Auto Scaling
**Objective:** Automatically adjust the number of instances based on traffic load.

**Steps:**
1. Created an Auto Scaling group.
2. Defined scaling policies based on metrics like CPU utilization.
3. Configured launch configurations for instances.

## Demonstration
1. **Live Demonstration:**
   - Showcased the running WordPress site.
   - Demonstrated site functionality and performance.

2. **Auto-scaling Simulation:**
   - Used tools like Apache JMeter to simulate increased traffic.
   - Monitored and demonstrated how Auto Scaling adjusted the number of instances.

## Conclusion
The project successfully implemented a scalable, secure, and high-performance WordPress site for DigitalBoost using AWS services. The infrastructure is capable of handling increased traffic and integrates seamlessly with the agency's existing infrastructure.

## Acknowledgements
Thanks to the team at DigitalBoost for providing the opportunity to work on this exciting project. Special thanks to AWS for their comprehensive cloud solutions and documentation.
