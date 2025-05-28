# 🛠️ osTicket – Post-Installation Configuration

This guide walks through the post-installation configuration of your osTicket environment after initial setup. You will configure roles, departments, users, SLAs, and help topics to simulate real-world help desk workflows.

---

## 🌐 Access URLs

- **Admin/Analyst Panel:**  
  `http://localhost/osTicket/scp/login.php`

- **End-User Portal:**  
  `http://localhost/osTicket`

---

## 🔑 Agent Panel vs Admin Panel

Understand the difference between the two panels:
- **Admin Panel** is used for configuration and system settings.

<img width="1047" alt="image" src="https://github.com/user-attachments/assets/fa9cbb95-cd5d-4115-b5dd-7bb603d26417" />

- **Agent Panel** is used for responding to and managing tickets.

<img width="1195" alt="image" src="https://github.com/user-attachments/assets/c836faee-ecef-4256-8e71-2ae43a2136e9" />


---

## 👥 Configure Roles

Define permission levels for agents.

**Path:**  
`Admin Panel → Agents → Roles`
![image](https://github.com/user-attachments/assets/fa1d0187-ced5-4853-9b28-31b1791fa423)

**Create a new Role:**  
- Name it Supreme Admin
- Give it all permissions

---

## 🏢 Configure Departments

Organize agents and control ticket visibility.

**Path:**  
`Admin Panel → Agents → Departments`

**Create a Department:**  
- Create a Sysadmins department and keep the Parent as *Top Level Department*  

<!-- 🖼️ Suggested Screenshot: Department creation page -->

---

## 🧩 Configure Teams

Pull agents from multiple departments into specialized teams.

**Path:**  
`Admin Panel → Agents → Teams`

**Create a Team:**  
- Online Banking

<img width="1034" alt="image" src="https://github.com/user-attachments/assets/fabe4fbd-22be-4412-80b7-c8023c0588cc" />

---

## 🔓 Allow Anyone to Create Tickets

Let unregistered users submit tickets.

**Path:**  
`Admin Panel → Settings → User Settings`  
**Action:**  
- Uncheck: `Require registration and login to create tickets`

<img width="1062" alt="image" src="https://github.com/user-attachments/assets/aabf1de8-6d00-42ad-8169-800d703e0d71" />

---

## 👩‍💼 Configure Agents (Support Staff)

Add support staff to your help desk.

**Path:**  
`Admin Panel → Agents → Add New Agent`

**Example Agents:**  
- Jane Doe
  - Configure username and password (something you will remember)
  - Set Department to *SysAdmins* and give *Supreme Admin* role
<img width="1062" alt="image" src="https://github.com/user-attachments/assets/f571fc31-be84-4914-a88f-543fcbd329e4" />


- John Doe
    - Configure username and password
    - Set Department to *Support* and give *All Access*

<img width="1062" alt="image" src="https://github.com/user-attachments/assets/2ce03aa7-53f1-4796-ae54-7308cbae28a1" />

---

## 🙋 Configure Users (Customers)

Add example customers for ticket submission.

**Path:**  
`Agent Panel → Users → Add New`

**Example Users:**  
- Karen  
- Ken
<img width="1192" alt="image" src="https://github.com/user-attachments/assets/171cc561-cd29-47f0-ac9d-5e66f08b948a" />


---

## ⏱️ Configure SLA (Service Level Agreements)

Set response time expectations for different ticket types.

**Path:**  
`Admin Panel → Manage → SLA`

**Examples:**
| SLA Level | Grace Period | Schedule   |
|-----------|--------------|------------|
| Sev-A     | 1 hour       | 24/7       |
| Sev-B     | 4 hours      | 24/7       |
| Sev-C     | 8 hours      | Business Hours |

<img width="1057" alt="image" src="https://github.com/user-attachments/assets/e754093e-c3cb-48c6-a91a-f9eff0d0078d" />


---

## 📑 Configure Help Topics

Categorize tickets for easier triage.

**Path:**  
`Admin Panel → Manage → Help Topics`

**Add new help topics:**  
- Topic name *Business Critical Outage*
  - Parent Topic *Report a Problem* 
- Topic name *Personal Computer Issues*
  - Parent Topic *Report a Problem*
- Topic name *Equipment Request*
  - Parent Topic *General Inquiry* 
- Topic name *Password Reset*
  - Parent Topic *Report a Problem*
- Topic name *Other*
  - Parent Topic *General Inquiry*
<img width="1057" alt="image" src="https://github.com/user-attachments/assets/5ec7b9f7-0db8-43db-b44c-0a1134d1bfc3" />
<img width="1057" alt="image" src="https://github.com/user-attachments/assets/eb53d623-03c4-4af5-9ba3-2c26de9d1c4d" />



> 💬 Let me know if you'd like this guide split into beginner/advanced versions or tailored for video walk-throughs.


