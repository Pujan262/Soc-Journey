Day 13-Event Id Refrence

# Windows Event ID Reference Card

| Event ID | Name | What It Means | Why Attackers Trigger It |
|----------|------|---------------|------------------------|

| 4624 | Successful login | Someone logged in successfully | Normal but suspicious at 3am or from unusual location |

| 4625 | Failed login | Login attempt failed | Multiple failures = brute force attack |

| 4648 | Login with explicit credentials | Used different account credentials | Lateral movement between systems |

| 4688 | New process created | A new program started running | Malware execution shows up here |

| 4698 | Scheduled task created | A new scheduled task was added | Attackers use this to run malware automatically |

| 4720 | New user account created | New account added to the system | Could be a backdoor account created by attacker |

| 4672 | Admin privileges assigned | Someone was given admin rights | Privilege escalation by attacker |

| 7045 | New service installed | A new Windows service was added | Rootkits install as services to survive reboots |

<img width="468" height="459" alt="image" src="https://github.com/user-attachments/assets/816d8829-d9d3-4523-9c4c-a704ca46c772" />
