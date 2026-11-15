# BSCP Exam Notes

Cheat sheet personale per la certificazione **Burp Suite Certified Practitioner (BSCP)**.

Copre tutti i lab di livello **Practitioner** della [PortSwigger Web Security Academy](https://portswigger.net/web-security) (esclusi Apprentice ed Expert), organizzati in 31 categorie e divisi in tre sezioni corrispondenti alle fasi tipiche dell'esame:

- **Step 1-2** — categorie usate tipicamente per ottenere un primo accesso o scalare privilegi (XSS, CSRF, Access control, Authentication, HTTP request smuggling, JWT, OAuth, ecc.)
- **Step 2-3** — categorie usate tipicamente per eseguire codice o estrarre dati una volta scalati ad admin (SQL injection, XXE, SSRF, Command injection, SSTI, Path traversal, Insecure deserialization, File upload)
- **Altre categorie** — non mappate su uno stage fisso (WebSockets, Information disclosure, Business logic, ecc.)

Per ogni lab è indicato:
- **Segnale** — come riconoscere la vulnerabilità
- **Soluzione** — l'approccio per sfruttarla
- **Payload** — un esempio concreto
- **Link** — collegamento diretto al lab ufficiale su PortSwigger
- **Step** — a quale fase dell'esame (1, 2 o 3) il lab è più utile, basato sull'analisi dello scenario/premessa del lab (non solo sulla presenza di credenziali)

In testa al documento c'è una tabella riassuntiva categoria → stage tipico.

## File

- [`BSCP-cheatsheet-IT.md`](./BSCP-cheatsheet-IT.md) — versione italiana
- [`BSCP-cheatsheet-EN.md`](./BSCP-cheatsheet-EN.md) — versione inglese

## Disclaimer

Note di studio personali, non affiliate con PortSwigger. Per i dettagli completi e aggiornati fare sempre riferimento alla [Web Security Academy](https://portswigger.net/web-security).
