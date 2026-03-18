# Role-Based Access Control (RBAC) Design

## Overview
To enforce secure access management during cloud changes, Role-Based Access Control (RBAC) is implemented based on the Principle of Least Privilege (PoLP). 

This ensures that users are granted only the minimum permissions required to perform their job functions, reducing the risk of unauthorized access and limiting the impact of potential security incidents.

---

## Roles & Responsibilities

| Role | Responsibility |
| :--- | :--- |
| **Cloud Architect** | Reviews and approves infrastructure and architecture changes. |
| **DevOps Engineer** | Deploys applications, manages CI/CD pipelines, and executes approved changes. |
| **Security Engineer** | Monitors logs, performs risk assessments, and enforces security policies. |
| **QA Engineer** | Tests deployments in staging environments before production release. |
| **Application Owner** | Provides business-level approval and manages application configurations. |

---

## RBAC Implementation
Access is managed using **Microsoft Entra ID** through directory roles and security groups.

Permissions are assigned based on job roles, ensuring proper separation of duties.

### Recommended Directory Roles (Least Privilege)
- **Privileged Role Administrator** – Manages role assignments and privileged access.
- **Application Administrator** – Manages enterprise applications and app registrations.
- **Conditional Access Administrator** – Defines and enforces access policies (e.g., MFA).
- **Security Reader** – Provides read-only access to logs and security insights.

> **Note:** The **Global Administrator** role is restricted to emergency ("break-glass") scenarios only and is not used for routine operations.

---

## Example Access Workflow

1. A **DevOps Engineer** submits a request to deploy a new application update.
2. The **Security Engineer** reviews potential risks and validates security controls.
3. The **Cloud Architect** reviews and approves the infrastructure changes.
4. The **DevOps Engineer** executes the deployment after approval.
5. All actions are logged for audit and compliance purposes.

---

## Key Benefits

- Reduces risk of unauthorized infrastructure changes  
- Enforces separation of duties across teams  
- Improves accountability through role-based access tracking  
- Supports compliance in regulated environments (e.g., banking)  
- Scales easily using group-based access management  
