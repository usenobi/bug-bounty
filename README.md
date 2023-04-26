## Rules
The following requirements must be adhered to in order to participate in NOBI's bounty program :
- We investigate and respond to all valid reports. Due to the volume of reports we receive, though, we prioritise evaluations based on risk and other factors, and it may take some time before you receive a reply.
- We determine bounty amounts based on a variety of factors, including (but not limited to) impact, ease of exploitation, and quality of the report. Note that extremely low-risk issues may not qualify for a bounty at all.
- We seek to pay similar amounts for similar issues, but bounty amounts and qualifying issues may change with time. Past rewards do not necessarily guarantee similar results in the future.
- In the event of duplicate reports, we award a bounty to the first person to submit an issue. (Capacity determines duplicates and may not share details on the other reports.) A given bounty is only paid to one individual.
- Your participation in this program must not disrupt or compromise any data that does not belong to you. Any attacks against other users or company data without provable express consent are prohibited and will automatically disqualify you from participating in the program.
- You must not disclose the issue to the public or a third-party before it has been fixed and prior written consent from NOBI.
- You must comply with any applicable laws and regulations in connection with your participation in this program. 
- NOBI's employees and all other affiliates are not eligible for rewards.


## Scope
The following domains are in the scope of the bug bounty program:
- usenobi.com and it subdomains
- Android : https://play.google.com/store/apps/details?id=com.usenobi
- iOS : https://apps.apple.com/id/app/nobi-smart-crypto-investment/id1510269362

Any design or implementation issue that substantially affects the confidentiality or integrity of user data is likely to be within the scope of the program, this include : 
```
- Injection (SQL, NoSQL, XML, etc.)
- Reflective or stored XSS.
- Cross-Site Request Forgery (CSRF).
- Server Side Request Forgery (SSRF).
- Remote code execution
- Security misconfiguration
- File inclusions (Local & Remote).
- Server-Side Remote Code Execution (RCE).
- Leakage of sensitive informations.
- Authentication Bypasses.
- Payment Manipulation.
- Directory Traversal Issue.
- Protection Mechanism bypasses (CSRF bypass, etc.).
- Local File Disclosure (LFD) 
- Server Side Template Injection (SSTI)
- Access Control Issues (Insecure Direct Object Reference Issues, Privilege Escalation, etc).
```

## Out of Scope
Non-Qualifying Vulnerabilities:
```
- Any sort of DoS/DDoS attacks are strictly prohibited
- Brute force attack
- Tabnabbing
- Social engineering, physical attack, phishing, spamming
- Application stack traces
- Self-type Cross Site Scripting
- Cross-site Request Forgery (CSRF) with minimal security implications (Logout CSRF, etc.)
- Password complexity requirement
- SSL/TLS scan reports (this means output from sites such as SSL Labs)
- Banner grabbing issues (figuring out what web server we use, etc.)
- Comma Separated Values (CSV) injection without demonstrating a vulnerability
- Directory Traversal Issue with low impact
- Vulnerabilities related to auto-fill web forms
- Vulnerabilities in second party or third party applications or platforms
- Vulnerabilities only exploitable on out-of-date browsers or platforms
- Vulnerabilities requiring the user to be compromised or to have malicious browser extensions
- Invalid or missing SPF (Sender Policy Framework) records (incomplete or missing SPF/DKIM/DMARC)
- Clickjacking/UI redressing with minimal security impact
- Rate Limit (i.e.: Email or SMS verification)
- Email verification deficiencies, expiration of password reset links, and password complexity policies
- Theoretical vulnerabilities without actual proof of concept
- Reports from automated web vulnerability scanners (Acunetix, Burp Suite, Vega, Nessus, etc.) that have not been validated
- Open-Redirects. 99% of open redirects have low security impact. For the rare cases where the impact is higher, e.g., stealing oauth tokens, we do still want to hear about them
```

Non-Qualifying Vulnerabilities - Mobile Apps:
```
- Shared links leaked through the system clipboard
- Any URIs leaked because a malicious app has permission to view URIs opened
- Absence of certificate pinning
- Sensitive data in URLs/request bodies when protected by TLS
- User data stored unencrypted on external storage and private directory
- Lack of obfuscation is out of scope
- auth "app secret" hard-coded/recoverable in apk
- Crashes due to malformed Intents sent to exported Activity/Service/BroadcastReceive (exploiting these for sensitive data leakage is commonly in scope) and due to malformed URL Schemes
- Lack of binary protection control in android app
- Lack of Exploit mitigations i.e., PIE, ARC, or Stack Canaries
- Path disclosure in the binary
- Snapshot/Pasteboard leakage
- Runtime hacking exploits (exploits only possible in a jailbroken/rooted environment)
```
## Submission
Though we welcome reporting of non-security issues, please note that only genuine security issues are eligible for rewards. If you have found a vulnerability, we would love to work with you to resolve it:

- Please email us at security[et]usenobi.com with the subject “[Bug Bounty NOBI] - Vulnerability Name”. Please do not contact employees directly or through other channels about a report.
- Within the body of the email, please describe the nature of the bug along with any steps required to replicate it, vulnerable component (API, FQDN, Deep URL), as well as pertinent applications, programs or tools used to discover the bug and the date and time testing took place.
- Include your legal name, phone number, and IP address at time of testing with your submission.

Please feel free to reach out to us at security[et]usenobi.com with any questions regarding the bug bounty program. We receive a lot of submissions through this program, so we may not be able to reply to your email promptly, but we'll respond as soon as possible. We look forward to hearing from you.
