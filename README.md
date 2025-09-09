# AWS Quick Revision Guide (Interview Prep)

This document covers key AWS concepts with theory + common interview questions & answers.

---

## 🔹 1. AWS Basics

### Theory
- **AWS**: Cloud platform offering IaaS, PaaS, SaaS.
- **Global Infrastructure**: Regions, Availability Zones, Edge Locations.
- **Pricing Models**: On-demand, Reserved, Spot, Savings Plans.

### Interview Q&A
- **What is AWS?** → Cloud platform with 200+ services.
- **Region vs AZ?** → Region = geographic location, AZ = isolated datacenters.
- **IaaS vs PaaS vs SaaS?** → EC2/S3 (IaaS), Elastic Beanstalk (PaaS), WorkMail (SaaS).
- **Pricing models?** → On-demand, Reserved, Spot, Savings Plans.

---

## 🔹 2. Compute (EC2, Lambda, Containers)

### Theory
- **EC2** → Virtual servers.
- **Auto Scaling** → Adjust EC2 count automatically.
- **ELB** → Distributes traffic (ALB, NLB, GLB).
- **Lambda** → Serverless compute, event-driven.
- **ECS/EKS/Fargate** → Containers.

### Interview Q&A
- **EC2 pricing options?** → On-demand, Reserved, Spot, Savings Plans.
- **Auto Scaling?** → Dynamically scales EC2 instances.
- **Lambda vs EC2?** → Lambda = serverless, short-lived; EC2 = long-running servers.
- **ECS vs EKS vs Fargate?** → ECS = AWS containers, EKS = Kubernetes, Fargate = serverless containers.

---

## 🔹 3. Storage (S3, EBS, EFS, Glacier)

### Theory
- **S3** → Object storage (11 9’s durability).
- **EBS** → Block storage for EC2.
- **EFS** → Shared file storage across instances.
- **Glacier** → Archival storage.

### Interview Q&A
- **S3 vs EBS?** → S3 = object, EBS = block.
- **EBS vs EFS?** → EBS = single instance, EFS = multiple instances.
- **Durability in S3?** → Replicated across AZs.
- **Bucket Policy vs IAM Policy?** → Bucket = resource-based, IAM = identity-based.

---

## 🔹 4. Databases

### Theory
- **RDS** → Managed relational DB.
- **Aurora** → High-performance AWS DB (MySQL/Postgres compatible).
- **DynamoDB** → NoSQL key-value DB.
- **Redshift** → Data warehouse.
- **ElastiCache** → In-memory cache.

### Interview Q&A
- **RDS vs DynamoDB?** → RDS = SQL, DynamoDB = NoSQL.
- **Aurora vs RDS?** → Aurora faster & scalable.
- **Multi-AZ vs Read Replica?** → Multi-AZ = HA, Read Replica = scaling.
- **ElastiCache use?** → Cache frequently accessed data.

---

## 🔹 5. Networking (VPC, Subnets, Security)

### Theory
- **VPC** → Private cloud network.
- **Subnets** → Public (IGW) vs Private (NAT).
- **Security Groups** → Instance-level firewall (stateful).
- **NACLs** → Subnet-level firewall (stateless).
- **Route53** → DNS service.
- **Load Balancers** → ALB, NLB, GLB.

### Interview Q&A
- **Public vs Private Subnet?** → Public = IGW, Private = NAT.
- **SG vs NACL?** → SG = stateful, NACL = stateless.
- **IGW vs NAT Gateway?** → IGW = inbound/outbound, NAT = outbound only.
- **Route53 policies?** → Simple, Weighted, Latency, Failover.

---

## 🔹 6. Security & IAM

### Theory
- **IAM** → Users, Groups, Roles, Policies.
- **KMS** → Key management.
- **CloudTrail** → Tracks API calls.
- **CloudWatch** → Monitoring & metrics.
- **Shared Responsibility Model** → AWS sec *of* cloud, customer sec *in* cloud.

### Interview Q&A
- **User vs Role?** → User = permanent, Role = temporary.
- **Least Privilege?** → Grant only required permissions.
- **IAM vs Bucket Policy?** → IAM = identity, Bucket = resource.
- **CloudTrail vs CloudWatch?** → Trail = audit logs, Watch = metrics/logs.
- **KMS use?** → Manage encryption keys.

---

✅ Next sections can include **DevOps Tools (CloudFormation, CodePipeline, Beanstalk)** and **Messaging (SQS, SNS, Kinesis, API Gateway)**.
