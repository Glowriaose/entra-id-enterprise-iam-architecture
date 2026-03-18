# Auditability and Logging

## Overview
Auditability and logging provide visibility into all identity-related activities within the cloud environment.

This ensures that every action can be traced, monitored, and reviewed, supporting security operations, incident response, and compliance requirements.

---

## Logging Architecture

The system captures three primary log streams using Microsoft Entra ID:

1. **Sign-in Logs**  
   Capture authentication activity, including user identity, location, device, and accessed applications  

2. **Audit Logs**  
   Record configuration changes such as group membership updates, role assignments, and policy modifications  

3. **Provisioning Logs**  
   Track lifecycle events including user creation, updates, and deletions within the directory  

---

## Critical Events Monitored

The **Security Engineer** actively monitors high-risk events, including:

- Changes to Conditional Access policies  
- Assignment of privileged roles or addition to sensitive security groups  
- Successful sign-ins from unfamiliar locations or unusual patterns  
- Multiple failed Multi-Factor Authentication (MFA) attempts  
- Unusual spikes in login or administrative activity  

---

## Log Management & Retention

- **Centralized Storage:** Logs are exported to a Log Analytics Workspace for long-term retention and analysis  
- **Retention Policy:** Logs are retained based on organizational and compliance requirements  
- **Access Control:** Only authorized roles (e.g., Security Reader) can view logs  

---

## Traceability & Accountability

All logged activities provide visibility into:

- **Who** performed an action  
- **What** action was performed  
- **When** the action occurred  
- **Where** the action originated  

This enables effective incident investigation, accountability, and audit readiness.

---

## Key Benefits

- Enhances visibility across identity and access activities  
- Supports rapid detection of suspicious behavior  
- Enables efficient incident response and forensic analysis  
- Strengthens compliance and audit readiness  
- Improves overall security monitoring capabilities  
