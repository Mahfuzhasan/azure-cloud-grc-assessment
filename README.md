# Azure Cloud Governance, Risk, and Compliance (GRC) Project

## Overview

This project demonstrates how cybersecurity **Governance, Risk, and Compliance (GRC)** practices can be implemented in a **Microsoft Azure cloud environment**. The environment simulates a **small law firm infrastructure** responsible for storing and protecting sensitive legal documents and confidential client information.

The project focuses on implementing cloud governance controls, identity security, network protection, secure storage, and policy enforcement while aligning the architecture with major cybersecurity compliance frameworks.

The goal of the project is to show how organizations can design and manage a secure cloud environment while reducing risk and supporting regulatory compliance requirements.

---

# Project Objectives

The primary objectives of this project were to:

- Design a secure **Azure cloud architecture** using cybersecurity best practices  
- Implement **Identity and Access Management (IAM)** using Microsoft Entra ID  
- Configure **Role-Based Access Control (RBAC)** and Multi-Factor Authentication (MFA)  
- Deploy a segmented **Virtual Network** to isolate application components  
- Protect sensitive data using **Azure Blob Storage encryption**  
- Enforce governance using **Azure Policy**  
- Perform a **risk assessment and threat analysis**  
- Map security controls to major **cybersecurity and compliance frameworks**

---

# Azure Architecture

The cloud environment simulates a secure infrastructure for a law firm handling confidential legal data.

Core components include:

- **Azure Resource Group** – Governance boundary for deployed resources
- **Azure Virtual Network (VNet)** – Provides secure network segmentation
- **Subnets**
  - Web Subnet (10.0.1.0/24)
  - Application Subnet (10.0.2.0/24)
- **Linux Virtual Machine** – Hosts a lightweight Nginx web server
- **Azure Blob Storage** – Stores sensitive legal documents securely
- **Network Security Group (NSG)** – Controls inbound network traffic
- **Azure Policy** – Enforces governance and security configurations

The environment demonstrates a **defense-in-depth cloud security architecture**.

---

# Identity and Access Management (IAM)

Identity governance was implemented using **Microsoft Entra ID**.

Security controls include:

- User identities representing organizational roles
- Security groups for permission management
- **Role-Based Access Control (RBAC)** assignments
- **Multi-Factor Authentication (MFA)**
- Conditional Access policies

These controls enforce the **principle of least privilege** and prevent unauthorized access to sensitive cloud resources.

---

# Network Security

Network security is implemented using Azure networking components:

- **Azure Virtual Network segmentation**
- **Network Security Groups (NSG)** acting as virtual firewalls
- Restricted inbound rules allowing only:
  - **Port 22** – SSH access
  - **Port 80** – Web application access

All other inbound traffic is denied by default.

This configuration reduces the attack surface and limits unauthorized access attempts.

---

# Secure Data Storage

Sensitive legal documents are stored using **Azure Blob Storage**.

Security protections include:

- Private storage container access
- Encryption of data **at rest**
- **HTTPS secure transfer enforcement**
- **Soft delete protection**

These controls help protect confidential data from unauthorized access or accidental loss.

---

# Governance and Policy Enforcement

Cloud governance is enforced using **Azure Policy**.

Policies implemented in the environment include:

- Mandatory **resource tagging** for ownership tracking
- **Disable public access** to storage accounts
- **Region restriction policy** to enforce data residency
- **Secure transfer enforcement** for encrypted communication

These policies act as **preventive controls**, blocking insecure configurations before deployment.

---

# Risk Assessment

A risk assessment was conducted to identify potential security threats affecting the cloud environment.

Key risks evaluated included:

- Unauthorized access to cloud resources
- Public exposure of sensitive storage data
- Misconfigured cloud infrastructure
- Network intrusion attempts
- Data interception during transmission
- Deployment of resources outside approved regions

A **risk register and heat map** were developed to evaluate risk likelihood and impact.

Security controls implemented within the environment significantly reduce the overall risk level.

---

# Compliance Framework Mapping

The implemented security controls align with major cybersecurity and regulatory frameworks:

- **NIST SP 800-53**
- **ISO/IEC 27001**
- **SOC 2**
- **PCI DSS**
- **PIPEDA**

Mapping cloud security controls to these frameworks demonstrates how organizations can maintain **regulatory compliance while securing cloud infrastructure**.

---

# Key Security Features

- Cloud governance using **Azure Resource Groups and tagging**
- Identity protection with **Microsoft Entra ID**
- **RBAC and MFA** access control
- Secure **network segmentation**
- **Firewall protection with NSG**
- **Encrypted storage for sensitive data**
- **Automated governance enforcement using Azure Policy**
- **Risk assessment and threat analysis**

---

# Technologies Used

- Microsoft Azure
- Microsoft Entra ID
- Azure Virtual Network
- Azure Virtual Machines
- Azure Blob Storage
- Azure Policy
- Network Security Groups
- Ubuntu Linux
- Nginx Web Server

---

# Conclusion

This project demonstrates how organizations can implement **cloud Governance, Risk, and Compliance (GRC) practices** within a Microsoft Azure environment. By combining governance policies, identity security, network protection, encrypted storage, and automated policy enforcement, the architecture establishes a strong **defense-in-depth cloud security model**.

The project illustrates how secure cloud environments can be designed to protect sensitive data while aligning with major cybersecurity and regulatory compliance standards.

---
