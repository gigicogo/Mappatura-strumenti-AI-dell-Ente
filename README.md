# 🔍 Shadow AI · La mappa dell'ufficio

> **Esercitazione interattiva per il percorso formativo "L'intelligenza artificiale nella Pubblica Amministrazione".**
> Un'unica web-app in tre fasi per mappare (senza giudicare) gli strumenti di IA già in uso negli uffici pubblici: autorizzati o spontanei, con quali account, per quali attività.

---
<img width="1120" height="628" alt="Screenshot 2026-10-24 alle 23 13 15" src="https://github.com/user-attachments/assets/b405261f-d66d-4a4d-92c2-20af37b0b946" />


🔗 **Demo online:** https://gigicogo.github.io/Mappatura-strumenti-AI-dell-Ente/

---

## 📋 Cos'è

Un singolo file HTML, senza backend né installazioni, pensato per l'esercitazione di gruppo che chiude il Modulo 1 (*"Lo scenario: come e perché l'IA è già entrata negli uffici pubblici"*). L'app accompagna i partecipanti in tre fasi progressive, per un totale di circa 30 minuti:

| Fase | Tempo | Cosa succede |
| --- | --- | --- |
| **1 · Detective** | ≈ 8′ | Quiz "caccia alla Shadow AI": 8 scenari d'ufficio da classificare (uso governato / Shadow AI / Shadow AI ad alto rischio), con feedback didattico e mappa dei "punti ciechi" più comuni |
| **2 · Censimento** | ≈ 15′ | Form guidato per censire gli strumenti di IA già in uso nel proprio ufficio: canale, tipo di account, attività, dati coinvolti, frequenza |
| **3 · Termografia** | ≈ 7′ | Matrice interattiva account × sensibilità dei dati: le schede del censimento si posizionano automaticamente, celle cliccabili per l'uso in plenaria |

## 🚀 Come si usa

### In aula (nessuna connessione richiesta)

1. Scarica il file `index.html` dal repo (o copialo da una chiavetta).
2. Aprilo con un doppio clic in qualunque browser moderno: Chrome, Edge, Firefox, Safari.
3. Proiettalo per la plenaria, oppure invialo ai piccoli gruppi perché lo usino sul proprio PC.

### Online

Il file è completamente statico e autocontenuto: può essere pubblicato gratuitamente su **GitHub Pages**, **Netlify** o qualunque hosting statico (vedi sotto), oppure semplicemente condiviso via canale interno dell'ente.

## 🔒 Privacy e protezione dei dati

L'app è progettata per l'uso in un ente pubblico, quindi:

- **Nessun dato lascia il dispositivo.** Nessuna richiesta di rete, nessun cookie, nessun servizio esterno.
- **Anonimato per costruzione.** Non viene mai chiesto il nome delle persone, al massimo l'ufficio/area.
- **I dati restano in locale** (localStorage del browser) finché l'utente non li cancella con "Svuota".
- **Export CSV** per la restituzione in plenaria: separatore `;` e codifica UTF-8 con BOM, pronti per Excel/Fogli.

## 🛠️ Struttura del repository

```text
├── index.html    # l'app completa (HTML + CSS + JS inline, zero dipendenze)
├── README.md     # questo file
└── LICENSE       # licenza (da scegliere)
```

Non serve build, npm, né alcuno strumento: solo un browser.

## 🌐 Pubblicazione gratuita (GitHub Pages)

1. Fai il fork o crea il repository e carica `index.html`.
2. Vai su **Settings → Pages**.
3. Sotto *Build and deployment*, seleziona il branch (`main`) e la cartella (`/root`), poi **Save**.
4. Dopo qualche minuto l'app sarà online su `https://<tuo-username>.github.io/<repo>/`.

Netlify (free) è un'alternativa valida: trascina il file e ottieni un link immediato.

## 📐 Come è costruita l'esercitazione

L'app segue i contenuti del Modulo 1 del percorso:

- la definizione di **Shadow AI** e i suoi canali (account personali, estensioni/plugin, funzioni IA integrate nelle suite, app mobile);
- il quadro **GDPR** (pseudonimizzazione ≠ anonimizzazione, art. 32) e il principio antropocentrico della **Legge 132/2025**;
- la distinzione tra **IA generalista** e **IA governata dalla PA** (RAG, fonti interne validate, account istituzionali).

La matrice finale serve da ponte verso la Giornata 3 (sicurezza e privacy) e la Giornata 5 (policy interna e tabella "ammesso / non ammesso").

## ✏️ Personalizzazione

Tutto il contenuto è in chiaro dentro `index.html`:

- **scenari del quiz**: array `CASI` (testi, risposte corrette, feedback);
- **attività e canali del censimento**: markup delle sezioni corrispondenti;
- **colori e testi**: CSS inline e stringhe leggibili nel blocco `<script>`.

Se adatti l'app al tuo ente, ricorda la regola d'ingaggio del corso: tutto ciò che produce l'IA (e anche questo esercizio, nel caso lo usi per raccogliere dati) resta materiale di lavoro — la valutazione e le decisioni restano sempre alle persone.

## 📄 Licenza

Da definire: si suggerisce una licenza aperta (es. MIT o CC BY 4.0) per favorire il riuso da parte di altri enti. Sostituisci questo paragrafo con il testo della licenza scelta e il file `LICENSE` del repo.

## 👤 Autore e contesto

**Gianluigi Cogo** — consulente e docente sui temi dell'IA generativa nella Pubblica Amministrazione.

L'app nasce come esercitazione della **Giornata 1** del percorso operativo *"L'IA nella Pubblica Amministrazione — Percorso operativo per l'uso consapevole, sicuro e governato dell'IA generativa"* (20 ore: percorso base per funzionari ed esecutori + modulo governance per direttori e dirigenti).

- 📮 Newsletter: [gigicogo.substack.com](https://gigicogo.substack.com)
- 📝 Blog: [medium.com/webeconoscenza](https://medium.com/webeconoscenza)
- ▶️ YouTube: [youtube.com/@gigicogo](https://www.youtube.com/@gigicogo)
- 💼 LinkedIn: [linkedin.com/in/gigicogo](https://it.linkedin.com/in/gigicogo)
