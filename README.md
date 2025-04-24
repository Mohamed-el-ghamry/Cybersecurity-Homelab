# Cybersecurity-Homelab

## Objective

The Cybersecurity Home Lab project aimed to build a comprehensive and isolated environment for simulating and detecting cyber attacks. The focus was to establish a secure domain infrastructure, deploy various security tools, and create a vulnerable environment for conducting offensive and defensive exercises. This project provides hands-on experience in network security, system administration, attack simulation, and incident detection using industry-standard tools.

### Skills Learned

- Proficiency in setting up and configuring a domain controller using Microsoft Active Directory.
- Experience with configuring and managing multiple operating systems (Windows, Ubuntu, Kali Linux).
- Hands-on skills in using Wazuh and Security Onion for intrusion detection and log analysis.
- Ability to simulate and execute penetration testing using tools like Hydra, Evil-WinRM, and Kali Linux.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
#### Defense & Enterprise Infrastructure
- VirtualBox – Type 2 hypervisor used as the local virtualization platform for VM orchestration.
- Microsoft Active Directory – Identity, user, and group management for the domain.
- Wazuh – Log analysis, intrusion detection, and SIEM functionality.
- Security Onion – Network traffic monitoring and forensic analysis.
- Postfix – Linux-based SMTP relay/email server.

#### Offensive & Penetration Testing Tools
- Hydra – Password brute-force tool for various protocols.
- Evil-WinRM – Post-exploitation tool for remote command execution.
- NetExec – Lateral movement & remote command execution over SMB, WMI, etc.
- XFreeRDP – RDP client for remote desktop control and reconnaissance.
- SecLists – Wordlists for username, password, and directory brute-forcing.
- Kali Linux Tools – Full suite for enumeration, scanning, and exploitation.
  
## Steps Overview

**1. Virtualization Setup**   

Provisioned all VMs in VirtualBox with allocated resources. Ensured internal NAT for lab isolation.

**3. Domain Services Deployment**   

Installed Windows Server 2019 and configured AD DS, DNS, and DHCP. Created users, groups, and GPOs.

**4. Client Environment Configuration**

Set up Windows 11 Enterprise and Ubuntu Desktop clients to join the domain, mimicking business and dev endpoints.

**5. Security Monitoring Infrastructure**

Deployed Security Onion and Wazuh for host and network intrusion detection. Configured agent-based logging and alerts.

**6. Email Server Setup**

Deployed Ubuntu Server 22.04 with Postfix as an internal email relay and tested SMTP configurations.

**7. Attack Simulation**

Used Kali Linux, Hydra, Evil-WinRM, and NetExec to simulate password attacks, remote shell access, and lateral movement.

**8. Log Analysis and Detection**

Analyzed logs in Wazuh and Security Onion for brute-force attempts, unauthorized logins, and suspicious traffic patterns.
