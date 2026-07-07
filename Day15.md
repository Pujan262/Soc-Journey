Day15-Kill chain and Mitre attack framework

1.Cyber Kill Chain — 7 Stages

Created by Lockheed Martin. Describes the 7 steps an attacker follows to successfully compromise a target. Understanding this helps SOC analysts identify which stage an attack is at and stop it early.

Stage	Name	What the attacker does
1	Reconnaissance	Gathering information about the target — emails, IP addresses, technologies used
2	Weaponisation	Creating the attack tool — building malware, crafting a phishing email
3	Delivery	Sending the attack to the target — phishing email, USB drop, malicious website
4	Exploitation	The vulnerability is triggered — victim opens the file, malware executes
5	Installation	Malware installs itself on the system — creates persistence
6	Command & Control	Attacker establishes communication with the compromised machine
7	Actions on Objectives	Attacker does what they came to do — steal data, encrypt files, move laterally

SOC use case: The earlier you detect an attack in the kill chain, the less damage is done. Catching it at Stage 3 (Delivery) is far better than catching it at Stage 7 (Actions on Objectives).


2. MITRE ATT&CK Framework

A free, publicly available knowledge base of real attacker tactics and techniques based on real-world observations. Used by every serious SOC team in the world.

Structure:
Level	What it is	Example
Tactic	  The goal the attacker wants to achieve	 Persistence
Technique	  How they achieve that goal	 T1053 Scheduled Task
Sub-technique	  A specific variation of the technique	 T1053.005 Scheduled Task/Job



		
The 14 Tactics (attacker goals):
•	Reconnaissance
•	Resource Development
•	Initial Access
•	Execution
•	Persistence
•	Privilege Escalation
•	Defense Evasion
•	Credential Access
•	Discovery
•	Lateral Movement
•	Collection
•	Command and Control
•	Exfiltration
•	Impact

MITRE ATT&CK is a framework that lists attacker 
tactics (goals) and techniques (how they achieve 
those goals). It is used by SOC analysts to 
categorise and understand attacks.

Example: Attacker uses PowerShell to download 
malware = Tactic: Execution, Technique: T1059.001
