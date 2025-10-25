# ☁️ AWS Network Engineering Series

🚀 A 3-project hands-on series covering **AWS Networking Fundamentals** — from designing Virtual Private Clouds to securing data traffic with private endpoints.  

---

## 🔧 Projects Overview

### 🧱 **1. VPC Architecture & Connectivity**
**Goal:** Build a secure VPC with public/private subnets and controlled internet access.  
**Highlights:**
- Designed a full VPC topology (10.0.0.0/16)
- Configured subnets, route tables, IGW, and NACLs
- Launched EC2 instances and validated connectivity (ping & curl tests)

**Key Skills:** VPC • Subnets • Route Tables • Security Groups • NACLs • EC2  

---

### 🌉 **2. VPC Peering & Flow Logs**
**Goal:** Enable private communication between two VPCs and monitor traffic.  
**Highlights:**
- Created two isolated VPCs (10.1.0.0/16 & 10.2.0.0/16)
- Established VPC Peering with bidirectional routing
- Implemented Flow Logs streaming to CloudWatch for network visibility

**Key Skills:** VPC Peering • Routing • IAM Roles • CloudWatch Logs • Monitoring  

---

### 🔐 **3. Private S3 Access via VPC Endpoint**
**Goal:** Access S3 privately within AWS without using the public internet.  
**Highlights:**
- Configured a Gateway VPC Endpoint for S3  
- Created IAM Access Keys and tested with AWS CLI  
- Applied a restrictive bucket policy using `aws:sourceVpce` for private access  
- Validated security by toggling endpoint policy (Allow ↔ Deny)

**Key Skills:** VPC Endpoints • S3 Policies • IAM • CLI Automation • Network Security  

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

---

## 🧑‍💻 Author
**Chandana Krishna**  
_Master’s in Computer Science | Texas State University_  
🎓 Cloud • DevOps • Security Enthusiast  

---

