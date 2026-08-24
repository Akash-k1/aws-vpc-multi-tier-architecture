# AWS Multi-Tier VPC Architecture

## 📌 Project Overview

This project demonstrates the design and implementation of a secure AWS network architecture using a custom Virtual Private Cloud (VPC). The architecture separates public and private resources using subnets, route tables, Internet Gateway, NAT Gateway, and Security Groups.

## 🏗️ Architecture

The infrastructure includes:

- Custom VPC
- Public and Private Subnets
- Internet Gateway for public internet access
- NAT Gateways for secure outbound internet access from private subnets
- Public and Private Route Tables
- EC2 instances deployed in public and private subnets
- Security Groups for controlling inbound and outbound traffic
- AWS Systems Manager (SSM) Session Manager for secure access to private instances

## 🔧 AWS Services Used

- Amazon VPC
- Amazon EC2
- AWS Identity and Access Management (IAM)
- AWS Systems Manager (SSM)
- NAT Gateway
- Internet Gateway

## 🚀 Implementation

1. Created a custom VPC and configured public and private subnets.
2. Configured an Internet Gateway to provide internet connectivity to the public subnet.
3. Created NAT Gateways to enable outbound internet access for instances in private subnets.
4. Configured public and private route tables and associated them with the appropriate subnets.
5. Launched EC2 instances in public and private subnets.
6. Configured Security Groups to control HTTP, HTTPS, and SSH traffic.
7. Connected securely to the private EC2 instance using AWS Systems Manager Session Manager.
8. Tested internet connectivity from the private instance through the NAT Gateway.

## 🔐 Security Design

- Public EC2 instances allow controlled inbound web traffic.
- Private EC2 instances are not directly exposed to the internet.
- Security Groups restrict access based on required ports.
- SSM Session Manager provides secure instance access without exposing SSH directly to the internet.

## 📚 Key Learnings

- Designing public and private network architectures in AWS
- Understanding route tables and subnet associations
- Configuring Internet Gateway and NAT Gateway
- Implementing secure access to EC2 instances
- Using AWS Systems Manager Session Manager

## 📸 Project Screenshots

Screenshots demonstrating the VPC architecture, route tables, NAT Gateway configuration, and EC2 connectivity will be added here.

---

### 👨‍💻 Author

**Akash**
