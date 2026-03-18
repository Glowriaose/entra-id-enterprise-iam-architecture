# Access Review Process

## Overview
Over time, user permissions can accumulate as roles and responsibilities change. This process, known as "privilege creep," increases security risk.

Periodic access reviews ensure that only the appropriate users retain access to systems and resources, maintaining strong access control and security hygiene.

---

## Review Frequency

- **Privileged Roles:** Reviewed monthly by the **Security Engineer**  
- **Standard Roles:** Reviewed quarterly by **Application Owners**  

---

## Access Review Cycle

1. **Review Notification**  
   Reviewers receive automated review requests through Microsoft Entra ID  

2. **Access Analysis**  
   Reviewers evaluate user access based on activity insights and system recommendations  
   (e.g., inactive users or unusual access patterns)  

3. **Decision Making**  
   Reviewers take one of the following actions:  
   - **Approve** – Retain access  
   - **Deny** – Remove access  
   - **Not Sure** – Flag for further investigation  

4. **Automated Remediation**  
   Denied access is automatically revoked by removing the user from the assigned role or group  

---

## Security Controls

- **Automated Reviews:** Ensures consistency and reduces manual effort  
- **Activity-Based Recommendations:** Helps identify inactive or unnecessary access  
- **Role-Based Review Ownership:** Assigns accountability to appropriate stakeholders  
- **Audit Logging:** All review actions are recorded for compliance and traceability  

---

## Key Benefits

- Eliminates stale accounts and unnecessary permissions  
- Reduces risk of unauthorized access due to privilege creep  
- Strengthens identity and access governance  
- Supports audit readiness for compliance standards (e.g., SOC 2, ISO 27001)  
- Maintains a clean and secure access environment  
