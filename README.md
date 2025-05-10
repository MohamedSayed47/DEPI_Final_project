![DEPI](https://media.licdn.com/dms/image/v2/D4D0BAQFNQpCaHl_CPw/company-logo_200_200/company-logo_200_200/0/1702455160827/digital_egypt_pioneers_initiative_depi_logo?e=2147483647&v=beta&t=O2rai_g0FzHFaE4ynebZgFGwPjWmsEpkUC1QrA0wTOg)
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
- **Network Services:** FTP, Java RMI, SMB, UnrealIRCd, VNC, Telnet, Apache Tomcat, SMTP
- **Attack Methods:** Scanning, Enumeration, Exploitation
- **Tools Used:** Nmap, Nessus, Metasploit, Enum4Linux

❌ **Out of Scope:**
- Testing external networks (only controlled lab environment)
- Denial-of-Service (DoS) attacks

---

## **2. Project Plan**

### **2.1 Timeline (Gantt Chart)**

| **Phase**              | **Task**                                     | **Duration** |
|------------------------|----------------------------------------------|--------------|
| **Phase 1: Planning**  | Define scope, methodology, tools              | 📅 1 day     |
| **Phase 2: Scanning & Enumeration** | Run Nmap, Nessus, Enum4Linux          | 📅 2 days    |
| **Phase 3: Exploitation**           | Exploit services like FTP, SMB, RMI    | 📅 4 days    |
| **Phase 4: Maintaining Access**           | Foothold in the target system  | 📅 2 days    |
| **Phase 5: Reporting** | Write findings & remediation report           | 📅 2 days    |

### Milestones & Deliverables
- ✅ **Milestone 1:** Initial scan and enumeration complete  
- ✅ **Milestone 2:** Exploitation phase with PoC  
- ✅ **Milestone 3:** Final report with detailed vulnerabilities and recommendations  

---

## **3. Task Assignment & Roles**

| **Team Member**                 | **Role**           | **Responsibilities**                           |
|--------------------------------|--------------------|------------------------------------------------|
| Mohamed Sayed Maher             | Ethical Hacker     | FTP , Java RMI |
| Waleed Khalid Edress           | Ethical Hacker     | SMB , UnrealIRCd        |
| Abdelrahman Tarek Farouk       | Ethical Hacker     | SMTP , VNC          |
| Ahmed Mohamed Ahmed Elganagy   | Ethical Hacker     | Telnet , Apache Tomcat               |

---

## **Phase 1: Planning**

### 1.1 Scope of Testing

| **Port** | **Service**        |
|----------|--------------------|
| 21       | FTP                |
| 25       | SMTP               |
| 1099     | Java RMI           |
| 445      | SMB (Samba)        |
| 6667     | UnrealIRCd         |
| 5900     | VNC                |
| 23       | Telnet             |
| 8180     | Apache Tomcat      |

⛔ **Out of Scope:**
- Physical security
- DoS attacks

### 1.2 Methodology

Following **PTES (Penetration Testing Execution Standard)**:

1. **Scanning & Enumeration** – Identify open ports/services
2. **Exploitation** – Gain unauthorized access where possible
3. **Maintaining Access** – Establishing a persistent foothold in the target system

### 1.3 Tools Used

| **Phase**              | **Tools**                          |
|------------------------|------------------------------------|
| Scanning & Enumeration | Nmap, Nessus, Enum4Linux,smbmap          |
| Exploitation           | Metasploit, Manual Scripts  |
| Reporting              | PDF                      |

---

## **Phase 2: Scanning & Enumeration**

All major ports and services were scanned. Vulnerabilities discovered are listed below.

| **Port** | **Service**        | **Vulnerability**            | **Description**                                                                 | **CVE**            | **Exploitability** |
|----------|--------------------|------------------------------|---------------------------------------------------------------------------------|--------------------|---------------------|
| 21       | FTP (vsftpd)       | Backdoor RCE                 | Hidden backdoor in vsftpd 2.3.4 allows remote command execution                 | CVE-2011-2523      | High                |
| 25       | SMTP (Postfix)     | Misconfiguration             | Allows unauthorized relaying or user enumeration                                | -                  | Medium              |
| 1099     | Java RMI           | Deserialization RCE          | Remote code execution via unsafe Java object deserialization                    | CVE-2011-3556      | High                |
| 445      | SMB (Samba)        | Usermap Script RCE           | Command injection through the Samba “username map script”                       | CVE-2007-2447      | High                |
| 6667     | UnrealIRCd         | Backdoor RCE                 | Backdoor allows execution of commands sent via IRC                              | CVE-2010-2075      | High                |
| 5900     | VNC                | Weak Credentials             | Access possible using default/weak passwords                                    | -                  | Medium              |
| 23       | Telnet             | Default Credentials          | Accepts login using default system credentials                                  | -                  | Medium              |
| 8180     | Apache Tomcat      | Weak Credentials + Upload    | Default credentials allow panel access for web shell deployment                 | CVE-2009-3548      | High                |

---

## **Phase 3: Exploitation**

Ethical exploitation was conducted on high-risk services. Successful attacks include:

- FTP backdoor shell access
- Java RMI code execution
- Samba RCE
- Tomcat WAR file deployment
- IRC remote commands
- Telnet access via default creds

---

## **Phase 4: Reporting**
### 📄  The Final Report : [📎 The Report](https://raw.githubusercontent.com/your-username/your-repo/main/docs/report.pdf)
---

## **💻 Setting Up the Lab**

- ✅ Download & install Metasploitable 2 from : [📎 SourceForge](https://sourceforge.net/projects/metasploitable/files/Metasploitable2/).
- ✅ Import into VirtualBox or VMware  
- ✅ Set network to NAT or Host-Only for isolation  

---

## **👥 Team Members**

| **Mohamed Sayed Maher** | **Waleed Khalid Edress** | **Abdelrahman Tarek Farouk** | **Ahmed Mohamed Ahmed Elganagy** |
|-------------------------|--------------------------|-------------------------------|----------------------------------|
| [LinkedIn](https://www.linkedin.com/in/mohamed-saye/) | [LinkedIn](https://www.linkedin.com/in/waleed-aboglail-09a6b226b/) | [LinkedIn](https://www.linkedin.com/in/abdelrahman-tarek-26a196264/) | [LinkedIn](https://www.linkedin.com/in/ahmedelganagy/) |
