# **Network Penetration Testing Project Planning & Management**

## **1. Project Proposal**
### **1.1 Project Title**
**Network Penetration Testing on Metasploitable 2**

### **1.2 Introduction**
This project focuses on conducting a **comprehensive network penetration test** on the **Metasploitable 2** virtual machine. The objective is to identify security vulnerabilities, ethically exploit them, and provide actionable remediation recommendations to enhance security.

### **1.3 Objectives**
- 🔍 Perform network scanning and enumeration to detect open ports and running services.
- 🎯 Exploit known vulnerabilities in Metasploitable 2 using ethical hacking techniques.
- 📄 Document findings and suggest effective mitigation strategies.

### **1.4 Scope**
✅ **In-Scope:**
- **Network Services:** FTP, Java RMI, SMB, RSH, SMTP, NFS, Apache,PostgreSQL
- **Attack Methods:**  Scanning, Enumeration, Exploitation
- **Tools Used:** Nmap, OpenVAS, Metasploit, Enum4Linux, Hydra

❌ **Out of Scope:**
- Testing external networks (only controlled lab environment)
- Denial-of-Service (DoS) attacks
---

## **2. Project Plan**

### **2.1 Timeline (Gantt Chart)**
| **Phase** | **Task** | **Duration** |
|----------|---------|------------|
| **Phase 1: Planning** | Define scope, methodology, tools | 📅 1 day |
| **Phase 2: Scanning & Enumeration** | OpenVAS, Nmap, Enum4Linux scans | 📅 2 days |
| **Phase 3: Exploitation** | Attacking FTP, Java RMI, SMB, RSH, SMTP, NFS, Apache,PostgreSQL | 📅 4 days |
| **Phase 4: Reporting** | Writing findings & recommendations | 📅 2 days |

### Milestones & Deliverables

- ✅ **Milestone 1:** Scanning phase completed with service enumeration  
- ✅ **Milestone 2:** Successful exploitation with proof-of-concepts  
- ✅ **Milestone 3:** Final penetration testing report delivered  

---

## **3. Task Assignment & Roles**

| **Team Member**     | **Role**               | **Responsibilities** |
|---------------------|----------------------|----------------------|
| Mohamed Sayed Maher        | Ethical Hacker        | Planning, tool selection, final report review |
| Waleed Khalid Edress    | Ethical Hacker     | Scanning & enumeration |
| Abdelrahman tarek farouk  | Ethical Hacker       | Exploitation & vulnerability testing |
| Ahmed Mohamed Ahmed Elganagy   | Ethical Hacker | Report writing & recommendations |

---
## Phase 1: Planning

### 1.1 Scope

Since we are working on Metasploitable 2, our focus is strictly on network vulnerabilities:

**Service** | **Port**
----------|---------
FTP       | 21
Rsh       | 512
NFS       | 23
Java RMI  | 1009
SMB       | 139, 445
IRC       | 6697
PostgreSQL| 5432
HTTP      | 8180

⛔ **Out of Scope:**

* Physical security attacks
* Denial-of-Service (DoS)


### 1.2 Methodology (Testing Approach)

We will follow the PTES (Penetration Testing Execution Standard) framework:

* Scanning & Enumeration – Gather system information.
* Exploitation – Attempt to gain unauthorized access.
* Post-Exploitation & Reporting – Document findings and recommend fixes.

### 1.3 Tools Selection

| Phase                     | Tool(s) Used           |
|---------------------------|------------------------|
| 🔍 Scanning & Enumeration | Nmap, OpenVAS, Enum4Linux |
| 🎯 Exploitation           | Metasploit, Hydra, SQLmap |
| 📄 Reporting              | PDF && Markdown Reports |
---
##Phase 2: Scanning & Enumeration

---
## Phase 3: Exploitation

---
### 📄  The Final Report 
[📎 The Report](https://raw.githubusercontent.com/your-username/your-repo/main/docs/report.pdf)

---
###  Setting Up the Testing Environment

* ✅ Download & Install Metasploitable 2 → SourceForge
* ✅ Use VirtualBox or VMware → Import Metasploitable 2
* ✅ Network Configuration → Set to NAT or Host-Only

---
### **👥 Team Members**

| ![John Doe](https://via.placeholder.com/100) | ![Jane Smith](https://via.placeholder.com/100) | ![Michael Brown](https://via.placeholder.com/100) | ![Emily Davis](https://via.placeholder.com/100) |
|---|---|---|---|
| **Mohamed Sayed Maher** | ** Waleed Khalid Edress** | **Abdelrahman tarek farouk** | **Ahmed Mohamed Ahmed Elganagy** |
| [LinkedIn](https://www.linkedin.com/in/mohamed-saye/) | [LinkedIn](https://www.linkedin.com/in/janesmith) | [LinkedIn](https://www.linkedin.com/in/michaelbrown) | [LinkedIn](https://www.linkedin.com/in/emilydavis) |
