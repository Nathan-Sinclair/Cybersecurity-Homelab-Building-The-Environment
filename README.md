# Cybersecurity-Homelab-Building-The-Environment
## Purpose:
Built a small-scale cybersecurity lab simulating a business network to enable hands-on testing, SIEM configuration, and attack/defense simulations, serving as the foundation for follow-up projects.  

## Implementation:
- Built a cybersecurity lab with Active Directory domain controller, servers, and Windows/Linux workstations.
- Configured VMs (VirtualBox/VMware) with NAT networking and enterprise-style IPs.
- Deployed Windows Server 2025, Windows 11, Ubuntu Desktop/Server, integrating Wazuh, Security Onion, Postfix and MailHog.
- Set up the network with SIEM functionality, EDR, and vulnerability scanning.
- Documented setup with screenshots and configuration examples for reproducibility.

## Skills Demonstrated:
- **Virtualization & Lab Setup**: Configured multiple VMs in VirtualBox/VMware with NAT networking, snapshots, and cloning.  
- **OS Administration**: Installed and managed Windows Server 2025, Windows 11, and Ubuntu 22.04 LTS.  
- **Active Directory & Identity Management**: Managed users, groups, SSO, and domain-joined workstations.  
- **Network & Security Configuration**: Assigned static IPs, configured jumpboxes, and implemented SIEM/EDR with Wazuh.  
- **Containerization & Services**: Deployed Docker containers (MailHog) and used Docker Compose for repeatable setups.  
- **Email Simulation & Automation**: Set up MailHog SMTP, sent test emails via Python, and created email polling scripts.  
- **Log & Threat Monitoring**: Collected and analyzed logs from Windows and Linux endpoints for intrusion detection.  
- **Scripting & Automation**: Wrote Bash and Python scripts to automate lab tasks and monitoring.  
- **Documentation & Reproducibility**: Produced step-by-step guides with screenshots for lab replication.  
- **Problem Solving**: Troubleshot VM networking, agent deployment, container setup, and domain integration issues.  



## Architecture:
<img width="1081" height="750" alt="image" src="https://github.com/user-attachments/assets/051c2386-673c-4604-8c38-a53864dbe2cc" />

### Summary:
| Element                  | Purpose                                                                 |
|---------------------------|-------------------------------------------------------------------------|
| Hypervisor (VirtualBox)  | Runs and manages multiple virtual machines on the Windows host.          |
| Enterprise Workstation 1 | Simulates a Windows 11 employee workstation.                            |
| Enterprise Workstation 2 | Simulates a Linux workstation, e.g. developer environment.               |
| Security Workstation     | Used for monitoring and analyzing attacks with Security Onion.           |
| Security Server 1        | Provides isolated email environment with MailHog for phishing exercises.|
| Security Server 2        | Acts as central SIEM/EDR server with Wazuh for log collection/analysis. |
| Directory Services Server| Provides Active Directory, DNS, DHCP, and SSO for identity management.   |



## Prerequisites & Dependencies:
### Hardware:
- Minimum: 8 GB RAM, 50 GB storage, 2 CPU cores.
- Recommended: 16 GB RAM, 100 GB storage, 4+ CPU cores.
- Virtualisation enabled (Intel VT-x / AMD-V).

### Virtualisation Platforms:
- VirtualBox: https://www.virtualbox.org/

### Operating System ISOs:
- Windows Server 2025: https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2025
- Windows 11 Enterprise: https://www.microsoft.com/en-us/evalcenter/evaluate-windows-11-enterprise
- Ubuntu Desktop 22.04.5 LTS: https://releases.ubuntu.com/jammy/ubuntu-22.04.5-desktop-amd64.iso
- Ubuntu Server 22.04.5 LTS: https://releases.ubuntu.com/jammy/ubuntu-22.04.5-server-amd64.iso
- Security Onion: https://github.com/Security-Onion-Solutions/securityonion/releases

### Security & Monitoring Tools:
- Wazuh (SIEM): https://wazuh.com/download/
- MailHog: https://sourceforge.net/projects/mailhog.mirror/files/v1.0.0/MailHog_windows_amd64.exe/

## Documentation/Step By Step Guide:

Full step-by-step setup and configuration instructions are provided in the accompanying PDF file.  
Here is the link: (Cybersecurity-Homelab-Building-The-Environment%20Documentation.pdf)

## Credits:

- Developed by Nathan Sinclair, inspired by Grant Collins’ Build a Cybersecurity Homelab: Enterprise 101 (https://projectsecurity.teachable.com/p/build-a-cybersecurity-homelab-a-practical-guide-to-offense-defense-enterprise-101). Special thanks to Grant Collins for creating such a valuable learning resource. 

- Tools used include Wazuh, Security Onion, MailHog, Postfix, VirtualBox, VMware, and Windows/Ubuntu OSs. 

- Documentation and content suggestions assisted by ChatGPT and other large language models (LLMs), with thanks to the open-source communities behind the tools. 


