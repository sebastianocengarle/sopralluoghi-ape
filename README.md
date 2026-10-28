# Sopralluoghi APE — prototipo

Web app installabile (PWA) per la raccolta dei dati di sopralluogo per gli Attestati di Prestazione Energetica. Non calcola la prestazione energetica: il PDF finale va riportato a mano nel software APE.

## Come provarla su Android

1. Apri il link dell'app con **Chrome** sul telefono (indirizzo GitHub Pages, indicato nella sezione "Pages" del repository).
2. Tocca il menu **⋮** in alto a destra.
3. Scegli **"Installa app"** oppure **"Aggiungi a schermata Home"**.
4. Avvia l'icona "Sopralluoghi" dalla schermata Home: si apre a schermo intero.

## Stato

- Versione di prova: elenco dei sopralluoghi, scheda con Generali, Involucro, Serramenti, Impianti e Firma (con foto del documento).
- Dati salvati sul telefono (localStorage), senza sincronizzazione. Le foto del documento occupano più spazio: con molti sopralluoghi conviene passare a IndexedDB.
- Da fare: planimetria con tag foto, sincronizzazione con Google Drive, esportazione PDF, campi mancanti (ACS, raffrescamento, ventilazione, superfici).

## Sviluppo locale

Nessuna dipendenza: sono file statici. Per provarli su computer basta un server statico, ad esempio `python3 -m http.server 8000`, poi apri `http://localhost:8000`.
