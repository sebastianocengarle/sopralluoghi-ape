# Sopralluoghi APE — prototipo

Web app installabile (PWA) per la raccolta dei dati di sopralluogo per gli Attestati di Prestazione Energetica. Non calcola la prestazione energetica: il PDF finale va riportato a mano nel software APE.

## Come provarla su Android

1. Apri il link dell'app con **Chrome** sul telefono (indirizzo GitHub Pages, indicato nella sezione "Pages" del repository).
2. Tocca il menu **⋮** in alto a destra.
3. Scegli **"Installa app"** oppure **"Aggiungi a schermata Home"**.
4. Avvia l'icona "Sopralluoghi" dalla schermata Home: si apre a schermo intero.

## Stato

- Versione di prova: elenco dei sopralluoghi e creazione di una bozza con indirizzo.
- Dati salvati sul telefono (localStorage), per ora senza sincronizzazione.
- Da fare: scheda (pareti, pavimento, solai, copertura, serramenti, impianti), planimetria con tag foto, firma del referente, sincronizzazione con Google Drive, esportazione PDF.

## Sviluppo locale

Nessuna dipendenza: sono file statici. Per provarli su computer basta un server statico, ad esempio `python3 -m http.server 8000`, poi apri `http://localhost:8000`.
