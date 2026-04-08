# í´ Phase 3: PIM Activation Workflow (Just-In-Time Access)

This phase demonstrates how Privileged Identity Management (PIM) enforces **Just-In-Time (JIT) access**, ensuring that privileged roles are only activated when required and automatically revoked after use.

---

## **Objective**

To validate the **Least Privilege Principle** by demonstrating how users activate privileged roles temporarily using PIM, with enforced security controls such as MFA, justification, and time-bound access.

---

## **Step 1: Role Eligibility Verification**

Before activation, I verified that the user does not have permanent administrative privileges but is instead assigned the role as **Eligible**.

* **User State:** Eligible (No active permissions)
* **Role:** Application Administrator
* **Access Level:** Zero Standing Access

> #### **[INSERT SCREENSHOT 1 HERE]**
>
> *Screenshot of **PIM > My roles > Eligible roles** showing the Application Administrator role in Eligible state.*

---

## **Step 2: Activation Request**

To perform administrative tasks, the user initiates a role activation request.

* **Action:** Clicked "Activate" on the eligible role
* **Justification Provided:** (e.g., Change Request ID or task description)
* **Scope:** Directory level

> #### **[INSERT SCREENSHOT 2 HERE]**
>
> *Screenshot of the **Activate role** panel showing justification input and activation options.*

---

## **Step 3: Security Verification (MFA Enforcement)**

As part of the Zero Trust security model, Multi-Factor Authentication (MFA) is required before activation is granted.

* **Control:** MFA challenge triggered
* **Purpose:** To verify user identity before granting elevated access

> #### **[INSERT SCREENSHOT 3 HERE]**
>
> *Screenshot showing the MFA prompt during role activation.*

---

## **Step 4: Time-Bound Role Activation**

Once approved (or auto-approved), the role becomes active for a limited duration.

* **Activation Duration:** 1â€“4 hours (as configured)
* **Access Type:** Temporary elevated privileges
* **System Behavior:** Countdown timer begins immediately

> #### **[INSERT SCREENSHOT 4 HERE]**
>
> *Screenshot of **Active roles** showing the role as Active with the remaining time (e.g., 4 hours).*

---

## **Step 5: Automatic Revocation**

After the activation window expires, access is automatically revoked.

* **Result:** User returns to non-privileged state
* **Security Benefit:** Eliminates risk of long-term privilege exposure

> #### **[INSERT SCREENSHOT 5 HERE]**
>
> *Optional: Screenshot showing role returned to Eligible state after expiration.*

---

## **Security Analysis: PIM Enforcement of Least Privilege**

This workflow enforces strong identity security controls:

1. **Just-In-Time (JIT) Access:** Privileges are only granted when explicitly requested
2. **MFA Enforcement:** Prevents unauthorized access even if credentials are compromised
3. **Time-Limited Access:** Reduces exposure window for privileged roles
4. **Audit Logging:** Every activation request is logged for compliance and monitoring

**Real-World Scenario:**
If an attacker gains access to a user account, they cannot perform administrative actions unless they successfully pass MFA and activate the role within PIM, significantly reducing the attack surface.

---

## **Tools & Services Used**

* Microsoft Entra ID (Azure AD)
* Privileged Identity Management (PIM)
* Azure Portal

---

## **Conclusion**

The implementation of PIM ensures that privileged access is tightly controlled, monitored, and time-bound. This aligns with **Zero Trust principles** and significantly enhances the security posture of the environment.

---


