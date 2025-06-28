# Custom-Nmap-Scripts

## Langflow-vuln-CVE-2025-3248.nse
GOAL: Detects and exploits CVE-2025-3248 unauthenticated remote code execution in Langflow instances (versions < 1.3.0).

The script first identifies Langflow web interface via a manual HTTP request.
When Langflow is detected, the exploitation phase will try to execute Id command on the server to confirm the vulnerability.

References for the vulnerability: 
* https://horizon3.ai/attack-research/disclosures/unsafe-at-any-speed-abusing-python-exec-for-unauth-rce-in-langflow-ai/
