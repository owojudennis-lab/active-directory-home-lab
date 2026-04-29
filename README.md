# 🧱 Active Directory Lab Setup (Windows Server)

## 📌 Overview
This project documents the setup of a Windows Active Directory environment in a virtual lab using VirtualBox.  

The goal was to build a functional Domain Controller and prepare an environment for security monitoring and attack simulations.

---

## 🖥️ Lab Environment
- Windows Server (Domain Controller)  
- Domain: `lab.local`  
- Network: Host-Only Adapter (`192.168.56.0/24`)  

---

## ⚙️ Configuration Steps

### 1. Network Configuration
The server was configured with a static IP:
IP Address: 192.168.56.110
Subnet Mask: 255.255.255.0
Gateway: 192.168.56.1
DNS: 192.168.56.110


---
<img src = "Setting static ip.png">
---

### 2. Active Directory Installation
- Installed **Active Directory Domain Services (AD DS)**  
- Promoted server to **Domain Controller**  

Domain created:
lab.local

---
<img src = "Installing Active directory.png">
---

### 3. User Management
A test user account was created:

- Username: `testuser`  
- Location: `lab.local → Users`  



---
<img src = "Addding a user to in the Active Direectory.png">
---

## 🧠 Key Learning Points
- Importance of DNS in Active Directory environments  
- Static IP configuration for Domain Controllers  
- Domain structure and user management  

---

## ⚠️ Challenges Encountered
- Initial network misconfiguration  
- DNS setup issues  
- IP conflicts during setup  

✅ Resolutions:
- Using a Host-Only network  
- Assigning correct DNS (self-referencing)  

---

## ✅ Outcome
A fully functional Active Directory environment was successfully deployed and is ready for security testing.

---

## 🚀 Next Step
This lab was extended into a detection lab using **Wazuh SIEM**:

<a href="https://github.com/owojudennis-lab/active-directory-wazuh-monitoring" target="_blank">
  <img src="https://img.shields.io/badge/See%20Project-Active%20Directory%20Wazuh%20Monitoring-blue?style=for-the-badge" />
</a>


