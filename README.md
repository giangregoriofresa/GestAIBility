# Coordinamento AIB — Pannello Applicazioni

Sito statico (HTML puro, nessuna build) con tre applicazioni collegate allo stesso
foglio Google Sheets condiviso, tramite un backend Google Apps Script.

## File

| File | Descrizione |
|---|---|
| `index.html` | Pannello di accesso alle tre app |
| `reperibilita_aib.html` | Registro reperibilità — inserimento/modifica turni |
| `matrice_turni.html` | Vista matrice (sola lettura) |
| `activity.html` | Creazione squadre operative |

## Pubblicazione su GitHub Pages

1. Carica tutti i file di questa cartella nella **root** del repository (stesso livello, nessuna sottocartella).
2. Vai su **Settings → Pages**.
3. In **Source** seleziona il branch `main` e la cartella `/root`, poi **Save**.
4. Dopo 1-2 minuti il sito sarà online su:
   `https://<nome-utente>.github.io/<nome-repo>/`

## Nota sul backend

Ogni pagina si collega allo stesso Web App di Google Apps Script (variabile
`SCRIPT_URL` nel `<script>` di ciascun file). Se cambi il deploy dello script,
aggiorna l'URL in tutti e tre i file (`reperibilita_aib.html`, `matrice_turni.html`,
`activity.html`).
