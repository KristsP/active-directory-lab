# Active Directory Lab

Beginner Active Directory lab using VirtualBox, Windows Server 2022, Windows 11, Active Directory Domain Services, Group Policy, Event Viewer, and account lockout testing.

## Overview

This project documents a beginner Active Directory lab built using VirtualBox, Windows Server 2022, and Windows 11. The lab was created to practise domain controller setup, user and group management, Group Policy configuration, domain client joining, and account lockout investigation.

The project was completed as part of my practical cyber security and IT support learning. It demonstrates hands-on skills relevant to entry-level IT support, service desk, junior system administration, IT security, and beginner SOC roles.

## Lab Environment

The lab used two virtual machines connected through a VirtualBox Host-Only Adapter:

- Windows Server 2022 Evaluation domain controller
- Windows 11 client machine

Main lab details:

- Domain: `adlab.local`
- NetBIOS name: `ADLAB`
- Domain Controller: `AD-DC-01`
- Domain Controller IP: `192.168.56.10`
- Windows 11 client joined to the domain

The host-only network allowed the Windows Server and Windows 11 client to communicate with each other in an isolated lab environment.

## Tools Used

- VirtualBox
- Windows Server 2022 Evaluation
- Windows 11
- Server Manager
- Active Directory Domain Services
- DNS
- Active Directory Users and Computers
- Group Policy Management
- Group Policy Management Editor
- Event Viewer
- Windows Security Logs
- Command Prompt

## Project Parts

### Part 1: Windows Server Installation and Initial Configuration

Installed Windows Server 2022 in VirtualBox and configured the virtual machine for use in an Active Directory lab. Set up NAT and host-only networking, then assigned a static IP address to the server.

### Part 2: Active Directory Domain Controller Setup

Installed Active Directory Domain Services and DNS through Server Manager. Promoted the server to a domain controller and created the `adlab.local` domain.

### Part 3: User, Group and OU Management

Created organisational units, domain users, and a security group in Active Directory Users and Computers. Added a user account to the IT-Support-Staff group and verified membership using both the GUI and Command Prompt.

### Part 4: Group Policy Configuration

Created and applied Group Policy settings, including a login banner and account lockout policy. Used `gpresult /r` to verify that the Group Policy Objects were applied successfully.

### Part 5: Domain Client Join and Account Lockout Investigation

Joined a Windows 11 client machine to the domain. Tested domain user login, confirmed the client computer object in Active Directory, triggered an account lockout, and reviewed Windows Security events including Event ID 4625 and Event ID 4740.

## Key Skills Demonstrated

- Building an isolated virtual Active Directory lab
- Configuring NAT and host-only networking
- Setting static IP and DNS settings
- Installing Active Directory Domain Services and DNS
- Promoting a server to a domain controller
- Creating organisational units, users, and groups
- Managing Active Directory group membership
- Creating and applying Group Policy Objects
- Joining a Windows 11 client to a domain
- Testing domain user authentication
- Configuring and testing account lockout policy
- Reviewing Windows Security logs in Event Viewer
- Investigating Event ID 4625 and Event ID 4740
- Writing structured technical reports

## Reports

The full project reports are available in the `Reports` folder:

- [Final Summary Report](Reports/Active-Directory-Lab-Final-Summary-Report.pdf)
- [Part 1: Windows Server Installation and Initial Configuration](Reports/Active-Directory-Lab-Part-1-Windows-Server-Installation-and-Initial-Configuration.pdf)
- [Part 2: Domain Controller Setup](Reports/Active-Directory-Lab-Part-2-Domain-Controller-Setup.pdf)
- [Part 3: User, Group and OU Management](Reports/Active-Directory-Lab-Part-3-User-Group-and-OU-Management.pdf)
- [Part 4: Group Policy Configuration](Reports/Active-Directory-Lab-Part-4-Group-Policy-Configuration.pdf)
- [Part 5: Domain Client Join and Account Lockout Investigation](Reports/Active-Directory-Lab-Part-5-Domain-Client-Join-and-Account-Lockout-Investigation.pdf)

## Conclusion

This Active Directory Lab demonstrates a beginner workflow covering Windows Server setup, domain controller configuration, user and group management, Group Policy, domain client joining, account lockout testing, and Windows Security log review. The project helped strengthen my understanding of practical Windows domain administration, IT support, and basic security investigation workflows in a controlled lab environment.
