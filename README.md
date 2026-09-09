# I miei ricettari — PWA

Versione 3.0 con interfaccia ridisegnata per riprendere il mockup approvato: sfondo crema, ricettari a copertina pastello, barra di navigazione inferiore, elenco ricette a card, form puliti e scheda ricetta con foto a tutta larghezza.

## Funzioni

- Ricettari illimitati con nome e colore personalizzati
- Copertine stile quaderno/ricettario
- Ricette con nome, ingredienti, procedimento opzionale, foto opzionale e cottura opzionale
- Foto da fotocamera o galleria
- Template uniforme per tutte le ricette
- Ricerca per nome e ingredienti
- Preferiti
- Modifica ed eliminazione di ricettari e ricette
- PDF della singola ricetta
- PDF completo del ricettario
- Condivisione PDF tramite menu nativo del telefono quando supportato
- Backup JSON e ripristino
- Salvataggio locale tramite IndexedDB
- PWA installabile e utilizzabile offline per le risorse già caricate

## Aggiornare il progetto su GitHub Pages

Nel repository GitHub sostituisci i file con quelli presenti in questa cartella e conferma il commit. Mantieni gli stessi nomi dei file e lasciali nella radice del repository.

File da caricare:

- `index.html`
- `app.js`
- `styles.css`
- `manifest.webmanifest`
- `service-worker.js`
- `icon-192.png`
- `icon-512.png`
- `README.md`

GitHub Pages ripubblicherà automaticamente il sito. La nuova versione del service worker usa una strategia più adatta agli aggiornamenti frequenti, quindi le modifiche ai file vengono recuperate dalla rete quando disponibile e restano disponibili offline in cache.

## Dati

L'aggiornamento dei file non cancella normalmente i ricettari già salvati nello stesso browser, perché il database locale mantiene lo stesso nome. È comunque consigliato esportare un backup prima di aggiornamenti importanti.
