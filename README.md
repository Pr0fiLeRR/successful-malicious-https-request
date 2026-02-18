## Detection as Code - Successful Malicious HTTPS requests

### Reason for Implementation

- I have seen incidents containing malicious HTTPS requests from many different IP addresses, this script gives us some information by correlating the IP address with the type of attack attempted from the IP (e.g., SQLi, XSS, Illegal Resource Access), with the time stamp and the attack count.

<img align="left" alt="MITRE ATT&CK Logo" width="120px" src="https://attack.mitre.org/theme/images/mitre_attack_logo.png"/>
<br/>

- [T1071.001 - Application Layer Protocol: Web Protocols](https://attack.mitre.org/techniques/T1071/001/)

### Query Instructions

- Line 23
    - You may want to remove IncapRules from this query if you want to see the requests that were hit by these rules which were most likely created by the SOC team right in the platform.
- Line 25
    - You may not see results, which can be a good sign, but if you need results for reference on what the query displays on the screen, edit from == to != to see blocked HTTP requests.

<br/>
<img align="left" alt="Detections.ai logo" width="120px" src="https://detections.ai/detections-logo-navbar.svg"/>
<br/>

- [Link to this contribution](https://detections.ai/rules/019c6e45-2654-7072-a368-f3c7f153f9ca)
