# Intro
The hard part about being a `n00b` in this competition for me was not realizing how much I didn't know at the time before getting crushed by the comp. 
I wasn't able to grapple with good questions to evaluate where I stood in my technical knowledge compared to the knowledge required for CCDC,
albeit I don't think you can ever be fully prepared for this competition, but just better prepared and equipped for problems you will face.

This list of questions will stand as template to guide you through your learning process. 
This list will not encompass everything needed to know on the comp. It will be up to you to truly ask yourself the hard questions of fully understanding how to secure the CCDC network,
and its attack surface. **YOU WILL NEVER KNOW EVERYTHING** *but you can always learn more*. So if you aren't able to answer some of these question get learning! 

----------------------------------
# The Questions

## Networking
*networking is going to be the backbone of your technical foundation, learn how computers,hosts,and nodes talk to each other work with eachother over various protocols.*
### TCP/IP
- what is the diffrence between TCP/UDP?
- what is ICMP?
- what is an IP address?
- what is a MAC address?
- what is a defualt gateway?
- how does routing work?
- how does DHCP work?
- how does ARP work?
- how does subnetting work?
- how do I trouble shoot network connectivity
- what is a network interface?
### Application Layer Protocols
- how does DNS work?
- how does HTTP/HTTPS work?
- what is SMB? (why is this so vulnerable?)
- what is ssh,telnet,rdp,?
- what is NTP? (how do I configure an NTP server & Client)
  	- what ports do all these belong to TCP/UDP?
- what protocols does Active Directory use?
	- kerberos
   	- LDAP
  	- RPC
----------------------
## Hardening
*hardening is the process of making the host more secure by limiting attack surface*
*this is done through various ways such as uninstalling unnesscary services, minimizing open ports, ect...*
### Windows

#### Window Client
*for standalone clients we still want to make sure that the local group policy and admin accounts are locked down, while also addressing potential vulnerable services*
*if an attacker can compromise a local admin account or NTAuthority System, they may be able to dump creds of domain users using a tool such as **mimikatz***
##### Firewall
- Turning on/off correct networking ports
	- What Services am I running what protocols do they need?
##### Services 
- Disabling Services ?
- What Services do I need?
- how do I update vulnerable versions?
##### Local User / Group Permissions
- Risky Privileges
	- `SeImpersonate`
- Changing passwords?
#### Windows Server
*or `Active-Directory` One of our biggest assets on the network, learn what concurrent vulnerabilities exist.. ie (ZeroLogon)*
##### Firewall
- Turning on/off correct networking ports
	- What Services am I running what protocols do they need?
##### File Permissions
- how do I limit user from Read/Write/Excuteing files?
- what files should I restrict access to?
##### User / Service Account / Group Permissions
- AS-REP Roasting, is kerberos pre-auth not disabled?
- Kerberoasting, are any accounts SPNs?
- User Account Management, how do i disable all user accounts that are not needed?
- what service accounts should be enabled? (krbtgt)
- how do I secure the krbtgt account?
- how do I change passwords
- how do I remove risky privilges from groups? 
##### Registry Keys
*Windows Registry is a hierarchical database that stores configuration settings and options on Microsoft Windows operating systems.*
*There are some keys that we want to double check that aren't enabling risky settings*
- Disable WDigest
- Disable NetBios
##### Group Policy
- how do I disable LLMNR?
- how do I disable LM Hash
- how do I implment ldap Signing?
- strong password polcies?
- lockout polcies?
- If SMB has to be on, how do I enable SMB signing
##### ACL/ACE
  
### Linux
*not going to differ between different distros as most of them are pretty similar but be aware that some commands will be slightly different*

#### Iptables

#### File Permissions
- Risky SUID set
- Risky Capabilities Set
- Loose Privileges 
#### User Permissions
- Risky Sudo Privs


-----------
## Maneuvering Command Line 

### Windows

#### CMD

#### Powershell

### Linux

#### BASH

-----------------------

## Authentication Concepts

### Access Tokens

#### Authentication Services

##### LSASS

##### WinLogon

##### SAM

### NTLM

### Kerberos

-----------------------
