
How a DNS Lookup Actually Works
Example: visiting academy.networkchuck.com for the first time.
•	1. Browser checks cache — have I visited this before? If yes, use the saved IP
•	2. Ask a DNS resolver — e.g. Google's 8.8.8.8 — "what is the IP for this domain?"
•	3. Resolver checks its own cache — if someone else already looked this up recently, reuse it
•	4. Ask the Root servers — if not cached, ask the root DNS servers — these are hierarchical and handle top-level domains (.com, .in, .jp, .np)
•	5. Root points to TLD server — the root tells the resolver which server manages .com domains
•	6. TLD server points to the domain's nameserver — which finally returns the actual IP address

This entire chain usually completes in milliseconds — but every step is a real lookup happening behind the scenes.

DNS Record Types
Record	Full Name	What It Does
A	Address	Maps a hostname to an IPv4 address
AAAA	Address (IPv6)	Maps a hostname to an IPv6 address
MX	Mail Exchange	Tells where to deliver email for a domain
CNAME	Canonical Name	Points one domain to another domain
TXT	Text	Stores text info, often used to verify domain ownership

HTTP Methods
Method	Action	Real Example
GET	Retrieve data	Opening a website — browser sends a GET behind the scenes
POST	Send new data	Creating a new account and clicking submit
PUT	Update existing data	Editing your profile information
DELETE	Remove data	Deleting an account or a post

HTTP Status Codes
Code	Meaning	What It Means
200	OK	Request was successful
301	Moved Permanently	Page redirected to a new URL
403	Forbidden	You do not have permission to access this
404	Not Found	The page does not exist
500	Internal Server Error	Something broke on the server side

HTTP vs HTTPS
	HTTP	HTTPS
Encryption	None	SSL/TLS encrypted
Who can read traffic	Anyone on the network	No one — data is scrambled
SOC Concern	Sensitive data sent here is a security risk	Considered safe for sensitive data
