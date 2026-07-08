Day16- Email Phishing

1. What is a Phishing Email
A fake email designed to trick someone into clicking a malicious link, downloading malware, or giving away credentials.
Types:
•	Phishing — mass sent to many people
•	Spear phishing — targeted at a specific person
•	Whaling — targeted at a senior executive
•	Smishing — phishing via SMS text message

2. What to Check in Email Headers
Email headers contain technical information hidden from the normal view. Right click any email → View Source or Show Original to see them.

Header Field	What to Check
From	Does the display name match the actual email address?
Reply-To	Is it different from the From address? Red flag.
Received	Shows the journey the email took — check for suspicious servers
X-Originating-IP	The real IP address the email was sent from
SPF/DKIM/DMARC	Did the email pass authentication checks? Fail = suspicious

3. What Makes a URL Suspicious

Red Flag	Example
Misspelled domain	paypa1.com instead of paypal.com
Extra subdomain	paypal.com.evil.com — the real domain is evil.com
Random characters	a7f3k2.xyz
URL shorteners	bit.ly/xxxxx — hides the real destination
HTTP instead of HTTPS	No encryption on a login page
Unusual TLD	.xyz, .top, .tk instead of .com or .org

4. How to Use VirusTotal

Go to virustotal.com
•	Paste a URL, IP address, file hash, or domain
•	Click Search
•	It checks against 70+ security engines simultaneously
•	Look at the Detection tab — how many engines flagged it?
•	Even 1-2 detections is worth investigating

Practice now:
•	Search google.com — should be completely clean
•	Search a random IP from your Wireshark captures — check what comes up

5. How to Use URLScan

Go to urlscan.io
•	Paste any suspicious URL
•	Click Scan
•	It visits the site in a safe sandbox and gives you: 
o	A screenshot of the page
o	All network requests the page makes
o	Any malicious indicators found
o	Technologies used by the site

Why it matters: You can safely investigate a suspicious URL without risking your own machine visiting it.

6. Phishing Investigation Workflow
This is your checklist for every phishing alert:

Step 1 — Check sender
  → Does display name match email address?
  → Is the domain legitimate or spoofed?

Step 2 — Check email headers
  → Did it pass SPF, DKIM, DMARC?
  → What is the originating IP? Check on AbuseIPDB.

Step 3 — Check links
  → Hover over links — does URL match the display text?
  → Paste URL into URLScan — screenshot the destination safely
  → Paste URL into VirusTotal — check detections

Step 4 — Check attachments
  → Do NOT open attachments on your own machine
  → Get the file hash and check on VirusTotal
  → Upload to any.run sandbox to watch what it does

Step 5 — Verdict
  → True positive (real phishing) → block sender, alert users, escalate
  → False positive (legitimate email) → document and close
<img width="468" height="635" alt="image" src="https://github.com/user-attachments/assets/64cd9c8e-a8c9-413e-b640-aeaffbbb53b4" />
