# Sopralluoghi APE — prototipo

Web app installabile (PWA) per la raccolta dei dati di sopralluogo per gli Attestati di Prestazione Energetica. Non calcola la prestazione energetica: il PDF finale va riportato a mano nel software APE.

## Come provarla su Android

1. Apri il link dell'app con **Chrome** sul telefono (indirizzo GitHub Pages, indicato nella sezione "Pages" del repository).
2. Tocca il menu **⋮** in alto a destra.
3. Scegli **"Installa app"** oppure **"Aggiungi a schermata Home"**.
4. Avvia l'icona "Sopralluoghi" dalla schermata Home: si apre a schermo intero.

## Stato

- Versione di prova: elenco dei sopralluoghi; scheda con Generali, Involucro, Serramenti, Impianti, Rinnovabili, Planimetria (tag foto e appunti a mano) e Firma (con foto del documento).
- Dati salvati sul telefono (localStorage), senza sincronizzazione. Le foto del documento occupano più spazio: con molti sopralluoghi conviene passare a IndexedDB.
- Foto e planimetrie sono salvate in IndexedDB sul telefono. Le planimetrie PDF usano pdf.js dal CDN (serve connessione alla prima apertura).
- Esportazione PDF: il pulsante "Esporta PDF" si trova nella scheda Firma, sotto il riquadro della firma. Crea il file con tutte le sezioni, le planimetrie con i tag, le foto, il documento e la firma. Il file viene salvato in Download. La libreria jsPDF è in lib/ e funziona offline.
- Scheda Informativa certificatore (come da modello D.M. 26.06.2015): compilata con i dati di Generali; esportabile da sola e inclusa in fondo al PDF del sopralluogo.
- Da fare: collegamento a Google Drive, campi mancanti (ACS, raffrescamento, ventilazione, superfici).

## Sviluppo locale

Nessuna dipendenza: sono file statici. Per provarli su computer basta un server statico, ad esempio `python3 -m http.server 8000`, poi apri `http://localhost:8000`.
