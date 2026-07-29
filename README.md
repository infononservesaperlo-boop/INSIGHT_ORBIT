# Insight Reel — Report

Archivio locale di report generati leggendo dati social (Instagram/Facebook via Composio, sola lettura). Apri `index.html` nel browser per l'elenco.

## Struttura

```
index.html          hub — elenco di tutti i report
reports/             un report per sottocartella, ognuna con il proprio index.html autonomo
  YYYY-MM-DD-nome-report/
    index.html
data/                dati grezzi (JSON) dietro ogni report, per rigenerarlo o aggiornarlo in futuro
  YYYY-MM-DD-nome-report.json
assets/               riservata per CSS/immagini condivise tra report, se in futuro servirà
```

Ogni report in `reports/` è un singolo file HTML autonomo (nessuna dipendenza esterna): funziona aprendolo direttamente da file system o pubblicandolo così com'è su GitHub Pages.

## Aggiungere un nuovo report

1. Crea `reports/YYYY-MM-DD-nome-report/index.html`.
2. Salva i dati grezzi corrispondenti in `data/YYYY-MM-DD-nome-report.json`.
3. Aggiungi una card in `index.html` (sezione `.report-list`) con link, data e breve descrizione.
