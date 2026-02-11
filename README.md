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


---

# Scenario 1: Online Banking System Outage

### End-User Submission

<p>
<img width="853" height="497" alt="Screenshot RD40" src="https://github.com/user-attachments/assets/2781a0a1-1b69-4be8-a79a-e54ac30345f1" />
</p>

A ticket is submitted reporting that the entire mobile and online banking platform is unavailable.

### Initial Agent Review (John)

<p>
<img width="853" height="497" alt="Screenshot RD41" src="https://github.com/user-attachments/assets/cdd23d7f-1880-4b03-b1cd-977d56eb4aca" />
</p>

Upon viewing the ticket, default settings appear:

- Priority: Normal
- Department: Unassigned
- SLA: None
- Assigned To: Unassigned

### Ticket Configuration

<p>
<img width="853" height="497" alt="Screenshot RD42" src="https://github.com/user-attachments/assets/944c0598-4290-4ae4-aa8d-383dd6b94a47" />
</p>

Because this issue impacts customers company-wide, the ticket is updated to:

- "SLA:" Sev-A (1 hour, 24/7)
- "Department:" Online Banking

### Access Control Observation

After routing to the Online Banking department:

- Agents not assigned to that department lose visibility.
- The ticket becomes inaccessible to unauthorized agents.

This demonstrates role-based security and department segmentation.

### Resolution (Jane)

<p>
<img width="853" height="497" alt="Screenshot RD43" src="https://github.com/user-attachments/assets/7690ceb5-aafa-43eb-bf93-2b26d310a545" />
</p>

<p>
<img width="853" height="497" alt="Screenshot RD44" src="https://github.com/user-attachments/assets/dbedc3d2-7264-4286-9472-6bbe12c73d53" />
</p>

<p>
<img width="853" height="497" alt="Screenshot RD45" src="https://github.com/user-attachments/assets/083b0bcf-4a91-4b10-9c03-13565f84c290" />
</p>

A qualified agent within the Online Banking department (Jane):

- Investigates service outage
- Coordinates with infrastructure teams
- Restores application functionality
- Documents root cause
- Closes the ticket within SLA

---

# Scenario 2: Adobe Upgrade Issue (Accounting Department)

### End-User Submission

<p>
<img width="853" height="497" alt="Screenshot RD46" src="https://github.com/user-attachments/assets/0a9d2526-6590-46bf-bbe3-ea215bab4393" />
</p>

Accounting reports that Adobe crashes after a recent update.

### Agent Review (John)

<p>
<img width="853" height="497" alt="Screenshot RD47" src="https://github.com/user-attachments/assets/2382fd7e-4992-43dd-8448-10a0ad284f7e" />
</p>

Initial state:

- Priority: Normal
- Department: Unassigned
- SLA: None
- Assigned To: None

### Ticket Configuration

<p>
<img width="853" height="497" alt="Screenshot RD48" src="https://github.com/user-attachments/assets/60978612-565d-4c8e-822c-10a076c96a9d" />
</p>

Since this issue is departmental but not company-wide:

- "SLA:" Sev-B (4 hours, 24/7)
- "Department:" Support
- "Assigned To:" John

### Resolution

<p>
<img width="853" height="497" alt="Screenshot RD49" src="https://github.com/user-attachments/assets/f24e62b7-d05e-4fba-9208-b62f2ba697d7" />
</p>

<p>
<img width="853" height="497" alt="Screenshot RD50" src="https://github.com/user-attachments/assets/dbe02965-57c3-409d-870d-1d3554b09ff7" />
</p>

John:

- Connects remotely to the user’s device
- Identifies corrupted installation
- Reinstalls approved software version
- Verifies application functionality
- Documents actions taken
- Closes the ticket
