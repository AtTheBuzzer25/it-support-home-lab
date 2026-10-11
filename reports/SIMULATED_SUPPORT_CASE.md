# Simulated support case: Windows device cannot access a website

**Work type:** Fictional training scenario authored for this portfolio setup.
**Execution status:** Not performed. No diagnostic outputs or successful resolution are claimed.

## Ticket
A user reports that a business website will not load on one Windows computer. Other users appear unaffected. Exact error, scope, and start time are unknown.

## Initial response
I understand this is preventing you from working. Please send the website address, the exact error or a screenshot, and when it started. Can you open other websites, and does the same site load on another device? I will use those details to narrow down the issue and keep you updated.

## Investigation plan
1. Confirm business impact and whether other devices or sites are affected.
2. Record the exact browser error; check the URL and system time.
3. Inspect `ipconfig /all` for adapter, address, gateway, and DNS configuration. Keep unredacted output private.
4. Run `Resolve-DnsName <hostname>` using the actual affected hostname; record whether resolution succeeds and which server answers.
5. Run `Test-NetConnection <hostname> -Port 443` for an HTTPS site. A successful TCP connection alone does not establish that the website works.
6. Compare with a working device and check relevant proxy, VPN, browser, and service-status information.
7. Make the smallest justified change, then retest the original task. Record all outcomes; escalate with evidence if the cause remains unclear.

## Closure criteria
The affected user can complete the original task; the action and verification are documented. Root cause and resolution remain undetermined until the investigation is actually performed.
