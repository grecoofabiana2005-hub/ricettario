# I miei ricettari — PWA v4

Versione con profili utente e sincronizzazione Supabase, mantenendo la grafica del mockup approvato.

## Novità v4

- Registrazione e accesso con email/password
- Conferma email e recupero password
- Profilo personale e logout
- Ricettari e ricette sincronizzati su più dispositivi
- Foto salvate nel bucket privato Supabase `recipe-photos`
- Row Level Security: ogni utente accede solo ai propri dati
- Trasferimento dei vecchi ricettari locali nel profilo online
- PDF della singola ricetta con layout visivo coerente con la schermata ricetta
- PDF completo del ricettario con copertina e tutte le ricette
- Condivisione PDF dal menu nativo del telefono
- Backup JSON e import nel profilo
- Cache locale di consultazione

## File da caricare su GitHub

Sostituisci nella radice del repository:
- `index.html`
- `app.js`
- `styles.css`
- `manifest.webmanifest`
- `service-worker.js`
- `icon-192.png`
- `icon-512.png`
- `README.md`

GitHub Pages ripubblicherà automaticamente il sito.

## Supabase già configurato nel progetto

L'app usa il Project URL e la Publishable key del progetto `ricettario`. La chiave segreta non è presente e non deve mai essere inserita nel frontend.

## Nota

Per la prima apertura dopo l'aggiornamento è consigliata una connessione Internet, perché vengono caricati Supabase JS, jsPDF e html2canvas.
