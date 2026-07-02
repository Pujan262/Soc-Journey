Day12-Event logs and Active Directory

Window Registry

The Windows Registry is a centralized, hierarchical database that stores low-level settings for the Microsoft Windows operating system and the applications that run on it.

Main Hives (Categories)

HKEY_CLASSES_ROOT (HKCR): Manages file extension associations and OLE (Object Linking and Embedding) data.
HKEY_CURRENT_USER (HKCU): Stores configurations for the user currently logged into the PC (desktop settings, app preferences).
HKEY_LOCAL_MACHINE (HKLM): Contains system-wide hardware, software, and security settings for all users.
HKEY_USERS (HKU): Holds the profiles for every user account on the computer.
HKEY_CURRENT_CONFIG (HKCC): Contains hardware profile data used during the current session.

Windows Event Log

Windows automatically records everything that happens on the system in Event Logs — logins, process creation, service changes, errors.
Three main logs:
•	System — hardware and OS events
•	Application — software events
•	Security — login attempts, privilege changes, account management
•	
You already memorised these Event IDs on Day 12 — here they are again:

Event ID	   Meaning
4624	  Successful login
4625	  Failed login
4688	  New process created
4698	  Scheduled task created
4720	  New user account created
4672	  Admin privileges assigned
	
SOC use case: This is what you stare at every day in a real SOC. Every alert investigation starts with pulling relevant Event Log entries.


Active Directory

A datatbase of everything on the network or it is a serive that manages users, computers and permission across an entire organizations.

Key term

Domain
A domain is a collection of AD objects, such as users, computers, groups and Organizational Units, that are stored in a shared database

Domain Cotrollers
A Server that is responsible for maintaining this active directory databse.

Group Policy
It allows administrator define and enforce secutiy setting, configurations and software ploicies across all computer and user in an entire organizations.


LADP
LDAP (Lightweight Directory Access Protocol) is an open, vendor-neutral software protocol used to locate, manage, and verify user identities and access rights across a network
<img width="468" height="646" alt="image" src="https://github.com/user-attachments/assets/44bf3c33-e4e8-4c83-acae-5adacc761d35" />
