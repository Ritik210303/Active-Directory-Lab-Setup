# Active-Directory-Lab-Setup

This project demonstrates the design and implementation of a complete **Active Directory (AD) environment** within a virtualized lab using Windows Server, Windows 10, and Ubuntu systems.

The objective of this project was to simulate a **real-world enterprise infrastructure**, where centralized identity management, authentication, and cross-platform integration are critical components of daily operations.

The lab was built using **Oracle VirtualBox** and configured to replicate how organizations manage users, devices, and access control through a domain-based architecture.

---

## 🏗️ Lab Architecture

The environment consists of the following systems:

- **Windows Server 2022** – Configured as Domain Controller  
- **Windows 10 Client** – Domain-joined workstation  
- **Ubuntu Client** – Integrated with Active Directory using realmd and SSSD  
- **Virtual Network** – NAT-based internal network for communication  

**Domain Name:** `RIT.local`

---

## ⚙️ Key Implementations

### 🔹 Active Directory Domain Services (AD DS)
- Installed and configured AD DS role  
- Promoted Windows Server to Domain Controller  
- Created and configured domain: `RIT.local`  

---

### 🔹 DNS Configuration
- Configured DNS for domain name resolution  
- Ensured proper communication between domain-joined systems  

---

### 🔹 Client Integration

#### Windows 10:
- Successfully joined to the domain  
- Verified domain-based authentication  

#### Ubuntu:
- Integrated using:
  - `realmd`
  - `sssd`
  - `adcli`  
- Enabled domain user login from Linux system  

---

### 🔹 System Validation
- Verified domain connectivity and authentication  
- Used tools such as:
  - `dcdiag` for domain controller diagnostics  
  - `nslookup` for DNS validation  
- Tested cross-platform authentication scenarios  

---

## 🧪 Challenges & Troubleshooting

During the setup, several real-world issues were encountered and resolved:

- DNS misconfiguration affecting domain discovery  
- Linux authentication failures with Active Directory users  
- Domain resolution inconsistencies  
- Troubleshooting SSSD and realm configuration  

These challenges provided practical experience in debugging enterprise identity systems.

---

## 📚 Learning Outcomes

This project provided hands-on experience with:

- Enterprise identity and access management  
- Centralized authentication using Active Directory  
- Cross-platform domain integration (Windows + Linux)  
- DNS and its role in domain environments  
- Real-world troubleshooting and system diagnostics  

---

## 🌍 Real-World Relevance

Active Directory is widely used in enterprise environments for:

- User authentication and access control  
- Device management within a domain  
- Policy enforcement using Group Policy Objects (GPO)  

This lab simulates a real organizational setup where multiple systems rely on a centralized identity provider, closely aligning with real-world IT and SOC environments.

---

## 🚀 Future Improvements

- Implement Group Policy Objects (GPO)  
- Integrate SIEM solution (Wazuh) for monitoring  
- Simulate attack scenarios (brute-force, lateral movement)  
- Enhance security controls and auditing  

---

## 👨‍💻 Author

**Ritik Patel**  
SOC – Threat Research Intern  
