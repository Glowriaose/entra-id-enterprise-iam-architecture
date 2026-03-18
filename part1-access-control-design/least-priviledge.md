# Least Privilege Principle & Privileged Identity Management (PIM)

## Overview
The principle of least privilege ensures that users are granted only the minimum level of access required to perform their job functions.

This project adopts a **Zero Standing Access** model, where no user has permanent privileged access. Instead, access is granted temporarily when required, reducing the risk of unauthorized actions, credential misuse, and misconfigurations.

---

## Privileged Identity Management (PIM)

Privileged access is controlled using Privileged Identity Management (PIM) to enable Just-In-Time (JIT) access.

Instead of having permanent administrative permissions, users are assigned **eligible roles**, which must be activated when needed.

---

## PIM Activation Workflow

1. **Eligibility Assignment**  
   The user is assigned as *eligible* for a privileged role but does not have active permissions  

2. **Activation Request**  
   The user requests role activation and provides a valid justification (e.g., Change Request ID)  

3. **Approval Process**  
   A designated approver (e.g., **Cloud Architect**) reviews and approves the request  

4. **Time-Bound Access**  
   Access is granted for a limited duration (e.g., 1–4 hours)  

5. **Automatic Revocation**  
   Access is automatically removed after the time window expires, returning the user to a non-privileged state  

---

## Security Controls

- **Just-In-Time (JIT) Access:** Privileges are activated only when required  
- **Approval-Based Activation:** Ensures oversight before granting access  
- **Time-Limited Permissions:** Reduces prolonged exposure of privileged roles  
- **Audit Logging:** All activation and usage activities are recorded  

---

## Key Benefits

- Reduces attack surface by eliminating permanent privileged access  
- Prevents misuse of credentials and privilege abuse  
- Enforces strong access control and accountability  
- Aligns with Zero Trust security principles  
- Supports compliance in regulated environments (e.g., financial institutions)  
