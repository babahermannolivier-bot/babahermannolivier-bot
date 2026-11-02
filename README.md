#[PROPOSED]  Multi-Cloud Zero-Trust Secure Deployment of Docker Containers in Azure and AWS Using Prisma Cloud Compute and SASE — CNAPP and ZTNA Implementation

> **Statuts:** Proposed MSc Final Project-Awaiting Lecturer Approval
> **Programme: MSc Applied Cybersecurity(Palo Alto) & Cloud Technology — London Metropolitan University

### 🎯 Objective
Securely deploy containerized workloads across AWS and Azure using Zero-Trust principles, enforced by Palo Alto Prisma Cloud Compute (CNAPP) and Prisma SASE with ZTNA.

### 🏗️ Architecture
**Multi-Cloud:** AWS EKS + Azure AKS
**Zero-Trust Model:** Never Trust, Always Verify
**Core Security Stack:**
- **Palo Alto Prisma Cloud Compute** (CNAPP) - Image Scanning, Runtime Defense, Compliance
- **Palo Alto Prisma SASE / ZTNA** - Secure remote access, identity-aware access
- **Docker** - Containerized microservices
- **Terraform** - IaC for secure provisioning
- **IAM** - Least privilege, federated identities
- **CI/CD Security** - Twistlock / Prisma scanning in pipeline

### 🔐 Key Implementations
1.  **CNAPP - Cloud Native Application Protection**
    - Container image vulnerability scanning before deployment
    - Runtime protection & compliance checks for EKS/AKS
    - Cloud Security Posture Management (CSPM)

2.  **ZTNA - Zero Trust Network Access (via Prisma SASE)**
    - Identity-based access, no VPN
    - Micro-segmentation between workloads
    - Conditional access policies

3.  **Secure IaC**
    - Terraform hardened with S3 backend encryption, IAM roles
    - No hardcoded secrets, using Azure Key Vault & AWS Secrets Manager

4.  **Threat Prevention**
    - Palo Alto Next-Gen Firewall policies
    - East-West traffic inspection in Kubernetes
    - 
### 📌 Project Status
- [x] Draft Architecture & Research
- [x] Initial IaC Scaffold (AWS EKS, Azure AKS)
- [x] Docker Hardening Baseline
- [x] Prisma Cloud CNAPP Policy Draft
- [ ] Awaiting Formal Approval from Supervisor
- [ ] Full Implementation & Testing (Post-Approval)

> Note: This repository currently contains the proposal scaffold and security baselines. Full deployment will commence upon approval.
