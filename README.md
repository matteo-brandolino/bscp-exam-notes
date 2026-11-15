# BSCP Exam Notes

Personal cheat sheet for the **Burp Suite Certified Practitioner (BSCP)** certification.

It covers every **Practitioner**-level lab from the [PortSwigger Web Security Academy](https://portswigger.net/web-security) (Apprentice and Expert labs excluded), organized into 31 categories split across three sections that correspond to the typical phases of the exam:

- **Step 1-2** — categories typically used to gain initial access or escalate privileges (XSS, CSRF, Access control, Authentication, HTTP request smuggling, JWT, OAuth, etc.)
- **Step 2-3** — categories typically used to execute code or extract data once you've escalated to admin (SQL injection, XXE, SSRF, Command injection, SSTI, Path traversal, Insecure deserialization, File upload)
- **Other categories** — not mapped to a fixed stage (WebSockets, Information disclosure, Business logic, etc.)

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

## Disclaimer

Personal study notes, not affiliated with PortSwigger. Always refer to the [Web Security Academy](https://portswigger.net/web-security) for the complete and up-to-date material.
