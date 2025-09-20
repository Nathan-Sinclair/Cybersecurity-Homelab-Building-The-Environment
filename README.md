# Cybersecurity-Homelab-Building-The-Environment
## Purpose:
Built a small-scale cybersecurity lab simulating a business network to enable hands-on testing, SIEM configuration, and attack/defense simulations, serving as the foundation for follow-up projects.  

## Implementation:
- Built a cybersecurity lab with Active Directory domain controllers, servers, and Windows/Linux workstations.
- Configured VMs (VirtualBox/VMware) with NAT networking and enterprise-style IPs.
- Deployed Windows Server 2025, Windows 11, Ubuntu Desktop/Server, integrating Wazuh, Security Onion, Postfix and MailHog.
- Set up the network with SIEM functionality, EDR, and vulnerability scanning.
- Documented setup with screenshots and configuration examples for reproducibility.

## Architecture:
<img width="1081" height="750" alt="image" src="https://github.com/user-attachments/assets/051c2386-673c-4604-8c38-a53864dbe2cc" />

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
Here is the link: [Insert PDF Link Here] 

## Credits:

- Developed by Nathan Sinclair, inspired by Grant Collins’ Build a Cybersecurity Homelab: Enterprise 101 (https://projectsecurity.teachable.com/p/build-a-cybersecurity-homelab-a-practical-guide-to-offense-defense-enterprise-101)

- Tools used include Wazuh, Security Onion, MailHog, Postfix, VirtualBox, VMware, and Windows/Ubuntu OSs. 

- Documentation and content suggestions assisted by ChatGPT and other large language models (LLMs), with thanks to the open-source communities behind the tools. 


