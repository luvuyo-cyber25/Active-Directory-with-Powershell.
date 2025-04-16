# Active Directory Management System - PowerShell & Windows Server

## Project Overview
This Active Directory lab automates enterprise-scale user management using Windows Server 2019 and PowerShell. The system deploys a functional domain controller, configures DHCP/DNS, and automates the creation of 1,000+ user accounts. Designed to replace manual AD administration, it demonstrates scalable infrastructure management and security policy implementation.

I built this project to solve two critical problems in enterprise IT: (1) the inefficiency of manual user provisioning, and (2) inconsistent security configurations. By implementing PowerShell automation and proper Group Policy settings, the system achieved 96% faster user creation (15 minutes vs 8 hours manually) and ensured 100% client connectivity in testing. This project showcases core Windows Server administration skills applicable to help desk and junior sysadmin roles.

## Features
- **Bulk User Creation**: Automated generation of 1,000+ AD accounts via PowerShell
- **Domain Configuration**: Deployed forest (mydomain.com) with OUs and security groups
- **Network Services**: Configured DHCP scopes (172.16.0.0/24) and DNS for client connectivity
- **Virtual Lab**: Built dual-network environment in VirtualBox (NAT + Internal)
- **Client Integration**: Successfully joined Windows 10 clients to the domain

## Technologies & Skills Gained

### Technical Skills
- **PowerShell Scripting**: Automated user creation (`New-ADUser`)
- **Active Directory Management**: OU structure, Group Policy basics
- **DHCP/DNS Configuration**: Scope management (172.16.0.0/24)
- **Virtual Networking**: VirtualBox adapter configuration
- **Windows Server Administration**: Role installation (AD DS, Routing)
- **Troubleshooting**: Resolved client-domain join issues

### Soft Skills Developed
- Process Automation
- Technical Documentation

## Screenshots
1. **VirtualBox Network Configuration**  
   ![Network Setup](screenshots/vbox_network.png)  
   *Dual adapter configuration (NAT + Internal)*

2. **AD DS Role Installation**  
   ![AD Installation](screenshots/ad_install.png)  
   *Installing Active Directory Domain Services*

3. **PowerShell Automation**  
   ![PS Script](screenshots/powershell_script.png)  
   *Bulk user creation script output*

4. **DHCP Scope Configuration**  
   ![DHCP Setup](screenshots/dhcp_scope.png)  
   *172.16.0.100/24 scope with gateway*

5. **Client Domain Join**  
   ![Joined Client](screenshots/client_join.png)  
   *CLIENT1 successfully joined to domain*

6. **User Login Test**  
   ![Login Test](screenshots/user_login.png)  
   *Domain user authentication*

7. **AD Users & Computers**  
   ![ADUC View](screenshots/ad_users.png)  
   *1,000+ users in OU structure*

## Installation
1. **Requirements**:
   - Oracle VirtualBox
   - Windows Server 2019 ISO
   - Windows 10 VM
