# BSCP Exam Notes

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/matteo-brandolino/bscp-exam-notes)](https://github.com/matteo-brandolino/bscp-exam-notes/commits/main)

[🇬🇧 English](./README.md) · 🇮🇹 Italiano

**Cheat sheet per superare più in fretta l'esame Burp Suite Certified Practitioner (BSCP): segnale → payload → stage d'esame.**

Appunti per la certificazione **Burp Suite Certified Practitioner (BSCP)** di [PortSwigger](https://portswigger.net/). Coprono tutti i lab di livello **Practitioner** della [PortSwigger Web Security Academy](https://portswigger.net/web-security) (esclusi Apprentice ed Expert), con payload pronti all'uso, organizzati per stage d'esame.

👉 **Leggi la cheat sheet:** [Italiano](./BSCP-cheatsheet-IT.md) · [English](./BSCP-cheatsheet-EN.md)

## Anteprima

La tabella di triage "Funzionalità → vulnerabilità" collega ciò che vedi nell'applicazione a ciò che conviene provare, con lo stage d'esame:

| Vedi… | Stage | Prova |
| --- | --- | --- |
| Barra di ricerca / termine riflesso nei risultati | 1-2 | XSS reflected/stored · SQLi |
| Cookie JWT (3 parti base64url) | 2 | JWT |
| Cookie `TrackingId` (query lato server) | 2 | Blind SQLi |
| "Check stock" (body XML) | 3 | XXE · bypass filtro SQLi · SSRF |
| Caricamento immagine prodotto (parametro `filename`) | 3 | Path traversal / LFI |

## Contenuto

31 categorie divise in quattro sezioni, ordinate secondo la struttura Foothold → Privilege Escalation → Data Exfiltration di [botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study](https://github.com/botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study):

- **Stage 1 (Foothold)** — categorie tipicamente usate per ottenere l'accesso iniziale contro una vittima anonima/generica, senza bisogno di un tuo account (Information disclosure, vulnerabilità DOM-based, XSS, Web cache poisoning, attacchi all'header Host, HTTP request smuggling, Authentication)
- **Stage 2 (Privilege escalation)** — categorie in cui il lab ti fornisce già credenziali valide a basso privilegio e l'exploit colpisce una vittima specifica già autenticata (spesso admin) per rubarne la sessione o forzare un'azione. I lab CSRF sono inclusi: ogni lab CSRF parte con il tuo account, quindi non è mai Stage 1 (CSRF, SQL injection, JWT, Prototype pollution, API testing, Access control, GraphQL, CORS, Business logic, Race conditions, NoSQL injection, Web cache deception, Web LLM attacks)
- **Stage 3 (Data exfiltration)** — categorie tipicamente usate per eseguire codice o estrarre dati una volta diventati admin (XXE, SSRF, SSTI, Path traversal, File upload, Insecure deserialization, OS command injection)
- **Altre categorie** — non coperte dalla suddivisione di botesjuan, quindi non associate a uno stage fisso (Clickjacking, OAuth, WebSockets, Essential skills)

Per ogni lab trovi:
- **Signal** — come riconoscere la vulnerabilità
- **Solution** — l'approccio per sfruttarla
- **Payload** — un esempio concreto
- **Link** — link diretto al lab ufficiale su PortSwigger
- **Step** — a quale stage d'esame (1, 2 o 3) il lab si adatta meglio, in base all'analisi dello scenario del lab (non solo alla presenza di credenziali)

All'inizio del documento c'è una tabella riassuntiva che associa ogni categoria al suo stage tipico.

## File

- [`BSCP-cheatsheet-IT.md`](./BSCP-cheatsheet-IT.md) — versione italiana
- [`BSCP-cheatsheet-EN.md`](./BSCP-cheatsheet-EN.md) — versione inglese
- [`README.md`](./README.md) — README in inglese

## Contribuire

Hai trovato un errore, un link a un lab rotto o un payload migliore? [Apri una issue](https://github.com/matteo-brandolino/bscp-exam-notes/issues) o manda una pull request. Mantieni il formato **Signal / Solution / Payload / Link / Step** e, se puoi, tieni allineate le versioni EN e IT.

## Crediti

- La mappatura degli stage (Stage 1 / 2 / 3) usata nella tabella riassuntiva è stata verificata rispetto alla suddivisione di [botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study](https://github.com/botesjuan/Burp-Suite-Certified-Practitioner-Exam-Study), che fornisce anche la wordlist per i lab PortSwigger citata negli appunti.
- La tabella di triage "Funzionalità → vulnerabilità" è ispirata a [D4mianWayne/BSCP](https://github.com/D4mianWayne/BSCP) (a sua volta basata su [DingyShark/BurpSuiteCertifiedPractitioner](https://github.com/DingyShark/BurpSuiteCertifiedPractitioner)).
- [bscp.guide](https://bscp.guide/) (Hacking-Notes) — checklist interattiva per l'esame citata nelle note di strategia.

Grazie ai rispettivi autori.

## Disclaimer

Appunti di studio personali, non affiliati a PortSwigger. Fai sempre riferimento alla [Web Security Academy](https://portswigger.net/web-security) per il materiale completo e aggiornato. Questo repository contiene solo appunti sui lab pubblici dell'Academy, non contenuti reali dell'esame.

## Licenza

[MIT](./LICENSE)
