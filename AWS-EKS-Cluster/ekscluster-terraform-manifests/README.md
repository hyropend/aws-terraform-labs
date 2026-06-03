# AWS EKS Cluster using Terraform ☸️

This project extends the previous AWS networking and Bastion Host infrastructure by deploying an Amazon EKS (Elastic Kubernetes Service) cluster using Terraform.

The goal of this lab is to better understand Kubernetes infrastructure on AWS and practice Infrastructure as Code (IaC) concepts in a real cloud environment.

---

# Technologies

* AWS
* Terraform
* Amazon EKS
* Kubernetes
* EC2
* IAM
* VPC
* Bastion Host
* Security Groups
* Linux / Bash

---

# Project Features

* Custom AWS VPC deployment
* Bastion Host configuration
* Amazon EKS Cluster deployment
* IAM Roles and permissions
* Security Group configuration
* Terraform variables and outputs
* Modular Terraform structure
* Infrastructure provisioning using Terraform

---

# Why EKS?

Amazon EKS is a managed Kubernetes service provided by AWS.

Instead of manually installing and managing Kubernetes control plane components, AWS manages the Kubernetes control plane automatically, including:

* API Server
* etcd
* High Availability
* Cluster health management
* Automatic scaling and maintenance

This allows engineers to focus more on workloads and infrastructure design rather than maintaining the Kubernetes control plane manually.

---

# Why IAM Roles?

IAM Roles are required because many AWS services and Kubernetes components need secure access to AWS resources.

Examples include:

* Worker nodes accessing AWS services
* Kubernetes components communicating with AWS APIs
* EBS CSI Driver managing storage
* Pods accessing AWS resources securely

IAM Roles provide temporary and secure permissions without exposing AWS credentials directly.

---

# EKS Networking Architecture

In this project, the EKS cluster is deployed inside the AWS VPC infrastructure created with Terraform.

The architecture includes:

* Custom VPC
* Public networking configuration
* Bastion Host access
* EKS Cluster resources
* Security Groups
* IAM-based access management

The Kubernetes cluster itself operates inside AWS-managed networking components while still integrating with the custom VPC environment.

---

# Learning Objectives

Through this project I practiced:

* Kubernetes fundamentals
* Amazon EKS architecture
* Terraform Infrastructure as Code workflows
* AWS IAM concepts
* Bastion Host architecture
* AWS networking fundamentals
* Secure infrastructure deployment

---

# Future Improvements

Planned future additions:

* Private Subnets
* Node Groups
* IRSA (IAM Roles for Service Accounts)
* EBS CSI Driver
* Helm deployments
* ArgoCD
* Monitoring & Logging
* CI/CD pipelines
* Production-style EKS architecture

---

03.06.2026
