# ☁️ AWS Network Engineering Series
# 🚀 AWS VPC Infrastructure Deployment

🚀 A 3-project hands-on series covering **AWS Networking Fundamentals** — from designing Virtual Private Clouds to securing data traffic with private endpoints.  
![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws&logoColor=white)
![DevOps](https://img.shields.io/badge/DevOps-Workflow-blue?logo=githubactions)
![Infrastructure as Code](https://img.shields.io/badge/IaC-Terraform-purple?logo=terraform)
![Status](https://img.shields.io/badge/Status-Completed-success)

---
## 🌐 Overview
This project demonstrates the **deployment of a robust AWS Virtual Private Cloud (VPC)** infrastructure designed for production environments.  
The configuration ensures **high availability, scalability, and enhanced security** by leveraging multiple AWS services and architectural best practices.

## 🔧 Projects Overview
---

### 🧱 **1. VPC Architecture & Connectivity**
**Goal:** Build a secure VPC with public/private subnets and controlled internet access.  
**Highlights:**
- Designed a full VPC topology (10.0.0.0/16)
- Configured subnets, route tables, IGW, and NACLs
- Launched EC2 instances and validated connectivity (ping & curl tests)
## 🧩 Key Implementations

**Key Skills:** VPC • Subnets • Route Tables • Security Groups • NACLs • EC2  
- 🌍 **Public & Private Subnets** – Structured architecture with segregated tiers for security and performance  
- 🏗️ **Multi-AZ Deployment** – Enhanced fault tolerance and redundancy  
- ⚖️ **Application Load Balancer (ALB)** – Efficiently distributes traffic across instances  
- 🌐 **NAT Gateways** – Enable secure outbound internet access for private resources  
- 📈 **Auto Scaling Groups** – Automatically handle traffic fluctuations and maintain elasticity  
- 🔐 **Security Groups & Route Tables** – Granular control of inbound/outbound traffic  
- 🧭 **Internet Gateway** – Managed access for public-facing components  
- 🧱 **Private EC2 Isolation** – Ensured no direct public exposure to sensitive instances  

---

### 🌉 **2. VPC Peering & Flow Logs**
**Goal:** Enable private communication between two VPCs and monitor traffic.  
**Highlights:**
- Created two isolated VPCs (10.1.0.0/16 & 10.2.0.0/16)
- Established VPC Peering with bidirectional routing
- Implemented Flow Logs streaming to CloudWatch for network visibility
## 💡 Insights & Learnings

**Key Skills:** VPC Peering • Routing • IAM Roles • CloudWatch Logs • Monitoring  
Through this deployment, I gained practical experience with:
- Designing **subnets for workload isolation and network segmentation**  
- Configuring **secure routing and traffic flow management**  
- Implementing **high-availability** setups across multiple AZs  
- Managing **auto-scaling and elasticity** for compute resources  
- Strengthening **access control** using Security Groups and NAT Gateways  
- Applying **AWS networking best practices** for security and cost optimization  

---

### 🔐 **3. Private S3 Access via VPC Endpoint**
**Goal:** Access S3 privately within AWS without using the public internet.  
**Highlights:**
- Configured a Gateway VPC Endpoint for S3  
- Created IAM Access Keys and tested with AWS CLI  
- Applied a restrictive bucket policy using `aws:sourceVpce` for private access  
- Validated security by toggling endpoint policy (Allow ↔ Deny)

**Key Skills:** VPC Endpoints • S3 Policies • IAM • CLI Automation • Network Security  
## 🧰 Technologies Used
- **AWS Services**: VPC, EC2, ALB, NAT Gateway, Auto Scaling, IAM, CloudWatch  
- **Tools**: Terraform (optional), AWS CLI, CloudFormation  
- **Networking Concepts**: CIDR, Subnetting, Route Tables, Gateways, Security Groups  

---

## 🧭 Learning Outcomes
✔️ Mastered core AWS networking services (VPC, Subnets, IGW, Endpoints)  
✔️ Established secure cross-VPC and private cloud communication  
✔️ Automated AWS access with CLI and IAM configurations  
✔️ Monitored and analyzed traffic through Flow Logs  

---

## ⚙️ Tools & Technologies
| Category | Tools / Services |
|-----------|-----------------|
| **Compute** | Amazon EC2 |
| **Storage** | Amazon S3 |
| **Networking** | VPC, Subnets, IGW, Route Tables, Endpoints |
| **Monitoring** | CloudWatch Logs, Flow Logs |
| **Security** | IAM Roles, Bucket Policies, Security Groups |
| **CLI & Automation** | AWS CLI, EC2 Instance Connect |
## 📚 References
- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)  
- [AWS Architecture Best Practices](https://aws.amazon.com/architecture/)


# 🚀 AWS VPC Infrastructure Deployment

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws&logoColor=white)
![DevOps](https://img.shields.io/badge/DevOps-Workflow-blue?logo=githubactions)
![Infrastructure as Code](https://img.shields.io/badge/IaC-Terraform-purple?logo=terraform)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 🌐 Overview
This project demonstrates the **deployment of a robust AWS Virtual Private Cloud (VPC)** infrastructure designed for production environments.  
The configuration ensures **high availability, scalability, and enhanced security** by leveraging multiple AWS services and architectural best practices.

---

## 🧩 Key Implementations

- 🌍 **Public & Private Subnets** – Structured architecture with segregated tiers for security and performance  
- 🏗️ **Multi-AZ Deployment** – Enhanced fault tolerance and redundancy  
- ⚖️ **Application Load Balancer (ALB)** – Efficiently distributes traffic across instances  
- 🌐 **NAT Gateways** – Enable secure outbound internet access for private resources  
- 📈 **Auto Scaling Groups** – Automatically handle traffic fluctuations and maintain elasticity  
- 🔐 **Security Groups & Route Tables** – Granular control of inbound/outbound traffic  
- 🧭 **Internet Gateway** – Managed access for public-facing components  
- 🧱 **Private EC2 Isolation** – Ensured no direct public exposure to sensitive instances  

---

## 💡 Insights & Learnings

Through this deployment, I gained practical experience with:
- Designing **subnets for workload isolation and network segmentation**  
- Configuring **secure routing and traffic flow management**  
- Implementing **high-availability** setups across multiple AZs  
- Managing **auto-scaling and elasticity** for compute resources  
- Strengthening **access control** using Security Groups and NAT Gateways  
- Applying **AWS networking best practices** for security and cost optimization  

---

## 🧰 Technologies Used
- **AWS Services**: VPC, EC2, ALB, NAT Gateway, Auto Scaling, IAM, CloudWatch  
- **Tools**: Terraform (optional), AWS CLI, CloudFormation  
- **Networking Concepts**: CIDR, Subnetting, Route Tables, Gateways, Security Groups  

---

## 📸 Architecture Diagram
> Below is the architecture I implemented:

![VPC Architecture](./vpc-architecture.png)

---

## 📚 References
- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)  
- [AWS Architecture Best Practices](https://aws.amazon.com/architecture/)

---

## 🏷️ Tags
`#AWS` `#VPC` `#Networking` `#CloudComputing` `#DevOps` `#InfrastructureAsCode` `#HandsOnLearning`

---

⭐ **If you liked this project, consider giving it a star!** 🌟  
👩‍💻 *Author: [Chandana Krishna](https://github.com/ChandanaKrishna27)*
