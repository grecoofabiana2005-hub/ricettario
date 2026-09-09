# I miei ricettari — PWA

Versione 2.0 pronta per l'uso e per GitHub Pages.

## Funzioni incluse
- Ricettari illimitati con nome e colore personalizzati
- Copertine stile quaderno/ricettario
- Ricette con nome, ingredienti, procedimento opzionale, foto opzionale e cottura opzionale
- Foto da fotocamera o galleria
- Template grafico uniforme per tutte le ricette
- Ricerca dentro un ricettario e ricerca globale per nome/ingredienti
- Preferiti
- Modifica ed eliminazione di ricettari e ricette
- PDF della singola ricetta
- PDF completo del ricettario
- Condivisione PDF con il menu nativo del telefono quando supportato
- Backup JSON e ripristino
- Salvataggio locale tramite IndexedDB (fallback localStorage)
- Installazione come PWA
- Service Worker per funzionamento offline dopo il primo caricamento

## Pubblicazione gratuita su GitHub Pages
1. Crea un repository pubblico su GitHub.
2. Carica **il contenuto** di questa cartella nella radice del repository.
3. Vai in Settings → Pages.
4. In Build and deployment scegli “Deploy from a branch”.
5. Seleziona `main` e cartella `/ (root)`.
6. Apri l'indirizzo HTTPS generato da GitHub Pages.
7. Dal telefono scegli “Installa app” / “Aggiungi a schermata Home”.

## Nota PDF
La libreria jsPDF viene caricata da jsDelivr al primo accesso. Dopo il primo caricamento il Service Worker prova a conservarla nella cache per l'uso offline. Se si apre l'app per la primissima volta completamente offline, le funzioni PDF non possono ancora essere caricate.

## Dati e privacy
Non è presente un server: ricettari, ricette e foto rimangono nel browser/dispositivo. È consigliato esportare periodicamente un backup dalle Impostazioni.
