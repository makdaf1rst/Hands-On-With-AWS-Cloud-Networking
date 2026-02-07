<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# 🌐 AWS Cloud Networking Series

**Author:** Mack (Saqib Hossain)  
**Email:** saqibh49@gmail.com  
**Series:** Get Hands On with Cloud Networking - NextWork Cloud Engineering Roadmap

---

## 📋 Series Overview

A comprehensive deep-dive into AWS networking fundamentals through 11 hands-on projects. This series covers everything from basic VPC architecture to advanced concepts like VPC peering, flow logs monitoring, and VPC endpoints. Each project builds upon the last, creating a complete understanding of how to architect secure, scalable cloud networks.

**What I Built:**
- Multi-tier VPC architectures with public/private subnet isolation
- Secure networking with route tables, security groups, and NACLs
- Direct EC2 instance access using SSH and key pairs
- VPC peering for secure inter-VPC communication
- CloudWatch Flow Logs for network traffic monitoring
- VPC endpoints for private AWS service connectivity

**Duration:** ~8 hours across 11 projects  
**Difficulty:** Beginner to Intermediate

---

## 🎯 Learning Objectives

By completing this series, I gained hands-on experience with:

✅ **VPC Architecture** - Designing isolated cloud environments with CIDR planning  
✅ **Network Security** - Implementing security groups, NACLs, and layered defense  
✅ **Traffic Management** - Configuring route tables and internet/NAT gateways  
✅ **EC2 Integration** - Launching instances with SSH authentication  
✅ **Network Troubleshooting** - Using ping, curl, and EC2 Instance Connect  
✅ **VPC Peering** - Creating secure connections between VPCs  
✅ **Monitoring & Logging** - Analyzing traffic with VPC Flow Logs and CloudWatch  
✅ **AWS CLI** - Managing infrastructure through command-line automation  
✅ **S3 Integration** - Accessing S3 buckets from VPCs securely  
✅ **VPC Endpoints** - Implementing gateway endpoints for private connectivity

---

## 📚 Project Index

### Phase 1: Foundations (Projects 1-2)
Before diving into networking, I established AWS fundamentals:

**1. [Host a Website on Amazon S3]((https://github.com/makdaf1rst/aws-host-a-website-on-s3))**
- Created S3 buckets and enabled static website hosting
- Configured bucket policies and ACLs for access control
- Learned about globally unique bucket names and endpoint URLs
- ⏱️ Duration: 1 hour

**2. [Cloud Security with AWS IAM](link-to-iam-repo)**
- Built IAM policies using JSON for role-based access control
- Created user groups and managed permissions across environments
- Implemented tagging strategies for resource organization
- Used IAM Policy Simulator for safe permission testing
- ⏱️ Duration: 1 hour

---

### Phase 2: Core Networking (Projects 3-7)

**3. [Build a Virtual Private Cloud](link-to-vpc-repo)**
- Created custom VPC with IPv4 CIDR block configuration
- Set up public/private subnets across availability zones
- Configured internet gateways for external connectivity
- Automated VPC creation using AWS CLI and CloudShell
- ⏱️ Duration: 2-3 hours

**4. [VPC Traffic Flow and Security](link-to-traffic-security-repo)**
- Configured route tables for traffic direction
- Implemented security groups for resource-level control
- Set up network ACLs for subnet-level security
- Deployed multi-region architecture for high availability
- Used EC2 Global View for resource management
- ⏱️ Duration: 1 hour

**5. [Creating a Private Subnet](link-to-private-subnet-repo)**
- Designed backend infrastructure with complete isolation
- Created dedicated route tables without internet gateway
- Implemented restrictive network ACLs (deny all traffic)
- Understood private vs public subnet architecture
- ⏱️ Duration: 30 minutes

**6. [Launching VPC Resources](link-to-vpc-resources-repo)**
- Deployed EC2 instances in public and private subnets
- Configured SSH key pairs for secure access
- Set up security groups with source-based restrictions
- Used VPC and More wizard for rapid deployment
- Learned about NAT gateways for private subnet internet access
- ⏱️ Duration: 20 minutes

**7. [Testing VPC Connectivity](link-to-connectivity-repo)**
- Used EC2 Instance Connect for SSH access
- Performed connectivity testing with ping and curl commands
- Debugged security group and NACL configurations
- Validated traffic flow across subnet architectures
- Distinguished between ping (connectivity) and curl (data retrieval)
- ⏱️ Duration: 40 minutes

---

### Phase 3: Advanced Networking (Projects 8-11)

**8. [VPC Peering](link-to-peering-repo)**
- Created peering connections between VPCs
- Updated route tables for inter-VPC communication
- Configured Elastic IP addresses for stable connectivity
- Troubleshot ICMP traffic and security group rules
- Ensured non-overlapping CIDR blocks
- ⏱️ Duration: 45 minutes

**9. [VPC Monitoring with Flow Logs](link-to-flow-logs-repo)**
- Set up VPC Flow Logs with CloudWatch integration
- Created IAM roles and trust policies for log delivery
- Analyzed network traffic patterns and rejected connections
- Used CloudWatch Logs Insights for log querying
- Debugged connectivity issues using flow log data
- ⏱️ Duration: 1 hour

**10. [Access S3 from a VPC](link-to-s3-access-repo)**
- Configured AWS CLI on EC2 instances
- Set up access keys for AWS service authentication
- Listed and uploaded objects to S3 from EC2
- Learned IAM roles as best practice alternative
- Used commands: `aws s3 ls`, `aws s3 cp`, `aws configure`
- ⏱️ Duration: 30 minutes

**11. [VPC Endpoints](link-to-endpoints-repo)**
- Created S3 Gateway endpoints for private connectivity
- Implemented bucket policies restricting traffic to VPC endpoint
- Configured endpoint policies for granular traffic control
- Updated route tables to use gateway endpoints
- Eliminated internet gateway dependency for S3 access
- ⏱️ Duration: 45 minutes

---

## 🛠️ Technologies & Services Used

**AWS Services:**
- Amazon VPC (Virtual Private Cloud)
- Amazon EC2 (Elastic Compute Cloud)
- Amazon S3 (Simple Storage Service)
- AWS IAM (Identity and Access Management)
- Amazon CloudWatch (Flow Logs)
- AWS CloudShell
- VPC Peering
- VPC Endpoints (Gateway)

**Tools & Concepts:**
- AWS CLI
- SSH & Key Pairs
- Security Groups
- Network ACLs (NACLs)
- Route Tables
- Internet Gateways
- NAT Gateways
- CIDR Blocks
- Elastic IP Addresses
- EC2 Instance Connect
- CloudWatch Logs Insights

**Command Line:**
- `ping` - Network connectivity testing
- `curl` - HTTP request testing
- `aws ec2` - EC2 resource management
- `aws s3` - S3 bucket operations
- `aws configure` - AWS CLI configuration

---

## 🎓 Key Takeaways

### Network Architecture
- **Multi-tier design** - Separating public and private resources for security
- **CIDR planning** - Ensuring non-overlapping IP ranges across VPCs
- **Availability zones** - Distributing resources for high availability
- **VPC isolation** - Creating secure boundaries for different workloads

### Security Best Practices
- **Layered security** - Combining security groups, NACLs, and route tables
- **Least privilege** - Restricting access to only what's necessary
- **Private connectivity** - Using VPC endpoints instead of internet gateways
- **Traffic monitoring** - Implementing Flow Logs for visibility

### Troubleshooting Skills
- **Security group debugging** - Understanding allow vs deny rules
- **Route table analysis** - Tracing traffic paths through VPCs
- **Flow log interpretation** - Reading network traffic metadata
- **EC2 Instance Connect** - Resolving SSH and IP address issues

### Automation & Efficiency
- **AWS CLI proficiency** - Managing resources via command line
- **VPC wizard usage** - Rapid deployment of complete architectures
- **CloudWatch Insights** - Querying logs programmatically
- **Infrastructure patterns** - Reusable VPC templates

---

## 📊 Architecture Diagrams

### Basic VPC Architecture
```
┌─────────────────────────────────────────────────────────┐
│                        VPC (10.0.0.0/16)                │
│  ┌──────────────────────┐  ┌──────────────────────┐    │
│  │  Public Subnet       │  │  Private Subnet      │    │
│  │  (10.0.1.0/24)       │  │  (10.0.2.0/24)       │    │
│  │                      │  │                      │    │
│  │  ┌────────────┐      │  │  ┌────────────┐     │    │
│  │  │ EC2        │      │  │  │ EC2        │     │    │
│  │  │ Instance   │      │  │  │ Instance   │     │    │
│  │  └────────────┘      │  │  └────────────┘     │    │
│  │         │            │  │         │           │    │
│  └─────────│────────────┘  └─────────│───────────┘    │
│            │                         │                │
│     ┌──────▼──────┐          ┌──────▼──────┐         │
│     │   Route     │          │   Route     │         │
│     │   Table     │          │   Table     │         │
│     └──────┬──────┘          └─────────────┘         │
│            │                                          │
│     ┌──────▼──────┐                                   │
│     │  Internet   │                                   │
│     │  Gateway    │                                   │
│     └─────────────┘                                   │
└─────────────────────────────────────────────────────────┘
```

### VPC Peering Architecture
```
┌─────────────────────┐         ┌─────────────────────┐
│   VPC 1             │         │   VPC 2             │
│   (10.1.0.0/16)     │◄───────►│   (10.2.0.0/16)     │
│                     │ Peering │                     │
│  ┌────────────┐     │         │  ┌────────────┐     │
│  │ EC2        │     │         │  │ EC2        │     │
│  │ Instance   │     │         │  │ Instance   │     │
│  └────────────┘     │         │  └────────────┘     │
└─────────────────────┘         └─────────────────────┘
```

### VPC Endpoint Architecture
```
┌──────────────────────────────────────────────────┐
│                   VPC                            │
│                                                  │
│  ┌────────────┐                                  │
│  │ EC2        │                                  │
│  │ Instance   │                                  │
│  └──────┬─────┘                                  │
│         │                                        │
│         ▼                                        │
│  ┌─────────────┐           ┌──────────────┐     │
│  │   Route     │──────────►│ VPC Gateway  │     │
│  │   Table     │           │   Endpoint   │     │
│  └─────────────┘           └──────┬───────┘     │
│                                   │             │
└───────────────────────────────────┼─────────────┘
                                    │
                            ┌───────▼────────┐
                            │  Amazon S3     │
                            │  Bucket        │
                            └────────────────┘
```

---

## 💡 Unexpected Learnings

Throughout this series, several insights stood out:

1. **Private subnets are structurally identical to public subnets** - The only difference is the internet gateway connection in the route table

2. **Security is layered by default** - AWS requires explicit rules at multiple levels (security groups, NACLs, bucket policies)

3. **The VPC wizard is a game-changer** - What took hours manually can be done in minutes

4. **Flow logs are incredibly detailed** - Every packet is logged with source, destination, port, and action

5. **Command line gives more control** - CLI provides options not always visible in the console

6. **Organization matters at scale** - Managing multiple subnets, NACLs, and security groups requires careful naming conventions

7. **Troubleshooting is methodical** - Network issues require checking each layer: route tables → security groups → NACLs → bucket policies

---

## 🚀 What's Next

This networking series is Phase 2 of the complete Cloud Engineering roadmap. Next phases include:

**Phase 3: Databases** - Aurora MySQL, DynamoDB, and application integration  
**Phase 4: Security** - KMS encryption, GuardDuty, Secrets Manager  
**Phase 5: Containers & Compute** - Lambda, Kubernetes, Docker, three-tier apps  
**Phase 6: DevOps** - CI/CD pipelines, Terraform, CloudFormation, multi-cloud  
**Phase 7: AI on Cloud** - Amazon Lex chatbots, AI transcription, Lambda integration

---

## 📂 Documentation Links

**Individual Project Repositories:**
- [Project 1: Host a Website on S3](link-to-s3-repo)
- [Project 2: Cloud Security with IAM](link-to-iam-repo)
- [Project 3: Build a Virtual Private Cloud](link-to-vpc-repo)
- [Project 4: VPC Traffic Flow and Security](link-to-traffic-security-repo)
- [Project 5: Creating a Private Subnet](link-to-private-subnet-repo)
- [Project 6: Launching VPC Resources](link-to-vpc-resources-repo)
- [Project 7: Testing VPC Connectivity](link-to-connectivity-repo)
- [Project 8: VPC Peering](link-to-peering-repo)
- [Project 9: VPC Monitoring with Flow Logs](link-to-flow-logs-repo)
- [Project 10: Access S3 from a VPC](link-to-s3-access-repo)
- [Project 11: VPC Endpoints](link-to-endpoints-repo)

**Project Documentation (PDFs):**
- [VPC Connectivity Testing Documentation](link-to-connectivity-pdf)
- [VPC Monitoring with Flow Logs Documentation](link-to-monitoring-pdf)

**External Resources:**
- [NextWork Cloud Engineering Roadmap](https://learn.nextwork.org/projects/aws-networks-monitoring?explore=series:cloud%20engineer)
- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/)
- [AWS CLI Reference](https://docs.aws.amazon.com/cli/)

---

## 🤝 Connect With Me

💼 [LinkedIn](https://linkedin.com/in/saqibhos)  
📧 Email: saqibh49@gmail.com  
🐙 GitHub: [@makdaf1rst](https://github.com/makdaf1rst)  
📘 [Facebook](https://facebook.com/mackdaf1rst)  
📷 [Instagram](https://instagram.com/mackdaf1rst)  
🤖 [Reddit](https://reddit.com/user/Mak_Mark_One)

---

## 📝 License

This project documentation is for educational purposes as part of the NextWork Cloud Engineering curriculum.

---

## 🙏 Acknowledgments

Special thanks to **NextWork** for providing a structured, hands-on cloud engineering curriculum that emphasizes real-world scenarios and practical troubleshooting.

---

<div align="center">

**⭐ If you found this helpful, please star this repository!**

*Building secure, scalable cloud infrastructure one project at a time.*

</div>

---

<!-- Proudly created as part of NextWork's Cloud Engineering Roadmap -->
