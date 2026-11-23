# BSCP Exam Notes

Personal cheat sheet for the **Burp Suite Certified Practitioner (BSCP)** certification.

It covers every **Practitioner**-level lab from the [PortSwigger Web Security Academy](https://portswigger.net/web-security) (Apprentice and Expert labs excluded), organized into 31 categories split across four sections, ordered to follow the Foothold → Privilege Escalation → Data Exfiltration structure of [botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study](https://github.com/botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study):

- **Stage 1 (Foothold)** — categories typically used to gain initial access against an anonymous/generic victim, with no account of your own needed (Information disclosure, DOM-based vulnerabilities, XSS, Web cache poisoning, Host header attacks, HTTP request smuggling, Authentication)
- **Stage 2 (Privilege escalation)** — categories where the lab already hands you valid low-privilege credentials, and the exploit targets a specific, already-authenticated victim (often admin) to steal their session or force an action — CSRF labs included: every CSRF lab starts with your own account, so it is never Stage 1 (CSRF, SQL injection, JWT, Prototype pollution, API testing, Access control, GraphQL, CORS, Business logic, Race conditions, NoSQL injection, Web cache deception, Web LLM attacks)
- **Stage 3 (Data exfiltration)** — categories typically used to execute code or extract data once escalated to admin (XXE, SSRF, SSTI, Path traversal, File upload, Insecure deserialization, OS command injection)
- **Other categories** — not covered by botesjuan's breakdown, so not mapped to a single fixed stage (Clickjacking, OAuth, WebSockets, Essential skills)

For each lab you'll find:
- **Signal** — how to recognize the vulnerability
- **Solution** — the approach to exploit it
- **Payload** — a concrete example
- **Link** — direct link to the official lab on PortSwigger
- **Step** — which exam stage (1, 2 or 3) the lab best fits, based on an analysis of the lab's scenario/premise (not merely whether credentials are provided)

At the top of the document there's a summary table mapping each category to its typical stage.

## Files

- [`BSCP-cheatsheet-IT.md`](./BSCP-cheatsheet-IT.md) — Italian version
- [`BSCP-cheatsheet-EN.md`](./BSCP-cheatsheet-EN.md) — English version

## Credits

The exam-stage mapping (Stage 1 / Stage 2 / Stage 3) used in the summary table was cross-checked against the stage breakdown from [botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study](https://github.com/botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study), used here as a reference with thanks to the author.

## Disclaimer

Personal study notes, not affiliated with PortSwigger. Always refer to the [Web Security Academy](https://portswigger.net/web-security) for the complete and up-to-date material.
