# IT Helpdesk Ticketing & Jira Support Workflow

## 1. Overview
Standard Operating Procedure (SOP) for managing, resolving, and tracking daily IT support tickets using Jira Service Management.

---

## 2. Jira Ticket Types: Incident vs Service Request

* **Incident (Something is Broken):**  
  An unplanned interruption or reduction in quality of an IT service.  
  *Examples:* Computer won't turn on, Outlook crashing, network down, printer error.  
  *Goal:* Restore normal service operation as quickly as possible.

* **Service Request (Something is Needed):**  
  A formal request from a user for something to be provided or created.  
  *Examples:* New employee onboarding setup, password reset, requesting a new laptop/mouse, software installation.  
  *Goal:* Fulfill standard user requests efficiently through standard approval paths.

---

## 3. Priority Matrix & Response Timelines

* **P1 - Critical:** System-wide outage or critical server offline affecting entire departments.  
  * *Target SLA:* Immediate (< 15 mins)
* **P2 - High:** Single user completely blocked from working (e.g., PC not booting, complete Outlook failure).  
  * *Target SLA:* < 1 hour
* **P3 - Medium:** Partial workflow impact (e.g., slow system performance, shared folder permission issue).  
  * *Target SLA:* < 4 hours
* **P4 - Low:** Non-urgent requests (e.g., password reset, software access request, peripheral inquiry).  
  * *Target SLA:* Within 24 hours

---

## 4. Daily Ticket Workflow in Jira

1. **Intake & Logging:**  
   Select the correct issue type (**Incident** or **Service Request**) and log with a clean summary:  
   `[Asset-ID/User] - [Core Issue]` (e.g., `LAP-104 - Outlook profile corruption on startup`).

2. **Triage & Diagnosis:**  
   Review error details/screenshots, set priority (P1–P4), and update ticket status to **In Progress**.

3. **Resolution & Internal Documentation:**  
   Apply the fix (e.g., DNS flush, profile recreation, permission assignment). Add an **Internal Note** in Jira detailing the fix for team visibility.

4. **User Verification & Closure:**  
   Confirm resolution with the end-user, get confirmation, and mark ticket as **Resolved / Closed**.
