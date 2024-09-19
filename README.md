# Intro
The hard part about being a n00b in this competition for me was not understanding how much I didn't know at the time before getting crushed by the completion. 
I wasn't able to grapple with good questions to evaluate where I stood in my technical knowledge compared to the knowledge required for CCDC,
albeit I don't think you can ever be fully prepared for this competition, but just better prepared and equipped for problems you will face.

This list of questions will stand as template to guide you through your learning process. 
This list will not encompass everything needed to know on the comp. It will be up to you to truly ask yourself the hard questions of fully understanding how to secure the CCDC network,
and its attack surface. **YOU WILL NEVER KNOW EVERYTHING** *but you can always learn more*. So if you aren't able to answer some of these question get learning! 

----------------------------------
# The Questions

## Networking

----------------------
## Hardening

### Windows

##### Window Client

###### Firewall
- Turning on/off correct networking ports
	- What Services am I running what protocols do they need?
###### Services 
- Disabling Services?
###### Local User / Group Permissions
- Risky Privileges
	- `SeImpersonate`
- Changing passwords?
##### Windows Server
###### Firewall
###### File Permissions
###### User / Service Account / Group Permissions
- AS-REP Roasting
- Kerberoasting
- User Account Management
###### Registry Keys
### Linux
*not going to differ between different distros as most of them are pretty similar but be aware that some commands will be slightly different*

#### Iptables

#### File Permissions
- Risky SUID set
- Risky Capabilities Set
- Loose Privileges 
##### User Permissions
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
