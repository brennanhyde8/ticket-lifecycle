<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This repository demonstrates how tickets move through a help desk environment using osTicket.
You’ll simulate ticket creation, property assignment, department restrictions, SLA escalation, and final resolution — just like in a real IT support team.
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

# 🎫 Help Desk Ticket Workflow Lab

**Simulating Real-World IT Support Using osTicket**

This repository outlines a hands-on lab demonstrating how support tickets move through a help desk system using **osTicket**.

The project walks through ticket creation, property configuration, SLA enforcement, department-based routing, access control restrictions, and final resolution from both the agent and administrative perspectives.

---

# 📌 Project Overview

This lab simulates real IT support operations by demonstrating:

* End-user ticket submission
* Agent review and classification
* SLA assignment (Sev-A vs Sev-B)
* Department-based permissions
* Escalation and access restrictions
* Ticket resolution and documentation

The objective is to show how structured workflows improve accountability, response times, and service quality.

---

# 🏦 Scenario 1: Online Banking System Outage

### End-User Submission

A ticket is submitted reporting that the entire mobile and online banking platform is unavailable.

### Initial Agent Review (John)

Upon viewing the ticket, default settings appear:

* Priority: Normal
* Department: Unassigned
* SLA: None
* Assigned To: Unassigned

### Ticket Configuration

Because this issue impacts customers company-wide, the ticket is updated to:

* **SLA:** Sev-A (1 hour, 24/7)
* **Department:** Online Banking

### Access Control Observation

After routing to the Online Banking department:

* Agents not assigned to that department lose visibility.
* The ticket becomes inaccessible to unauthorized agents.

This demonstrates role-based security and department segmentation.

### Resolution (Jane)

A qualified agent within the Online Banking department:

* Investigates service outage
* Coordinates with infrastructure teams
* Restores application functionality
* Documents root cause
* Closes the ticket within SLA

---

# 🧾 Scenario 2: Adobe Upgrade Issue (Accounting Department)

### End-User Submission

Accounting reports that Adobe crashes after a recent update.

### Agent Review (John)

Initial state:

* Priority: Normal
* Department: Unassigned
* SLA: None
* Assigned To: None

### Ticket Configuration

Since this issue is departmental but not company-wide:

* **SLA:** Sev-B (4 hours, 24/7)
* **Department:** Support
* **Assigned To:** John

### Resolution

John:

* Connects remotely to the user’s device
* Identifies corrupted installation
* Reinstalls approved software version
* Verifies application functionality
* Documents actions taken
* Closes the ticket
