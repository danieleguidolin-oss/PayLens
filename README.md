# PayLens

App per leggere e capire la propria busta paga. Carichi il cedolino (PDF), scegli il tuo CCNL, e un'IA risponde alle tue domande: cosa significano i codici, se ferie e ROL sono calcolati correttamente, perché lo stipendio cambia da un mese all'altro.

## Stato del progetto

Questo repo contiene per ora il **mockup grafico interattivo** (`index.html`), pensato per validare direzione visiva e flusso prima di passare allo sviluppo vero e proprio.

### Flusso mostrato nel mockup

1. **Selezione CCNL** — menu a tendina con ricerca live tra i principali contratti nazionali italiani; prima voce dell'elenco: "Non conosco il mio contratto".
2. **Caricamento cedolino** — al momento solo PDF (foto/screenshot pianificati per dopo).
3. **Decoder** — i dati estratti dal cedolino mostrati in stile "libro mastro", con un'annotazione a etichetta che traduce le voci in linguaggio semplice, e una chat con l'IA per fare domande dirette.

### Direzione grafica

Palette scura (nero + oro), font Space Grotesk / Inter / IBM Plex Mono, per un tono preciso ed elegante.

## Come vedere il mockup

Apri `index.html` in un browser — è una singola pagina statica, nessuna build richiesta.

## Installarla come app sul telefono

Il progetto è configurato come PWA (manifest + service worker + icone), quindi una volta pubblicato su GitHub Pages puoi installarlo come un'app vera:

- **Android (Chrome)**: apri il link, tocca il menu (⋮) → "Aggiungi a schermata Home" / "Installa app".
- **iPhone (Safari)**: apri il link, tocca l'icona Condividi → "Aggiungi a Home".

Resta comunque solo il mockup grafico — nessun dato reale viene caricato o elaborato.

## Prossimi passi

- Estrazione testo dai PDF (i cedolini hanno quasi sempre testo selezionabile, non serve OCR in questa fase)
- Prompt all'IA con contesto CCNL + testo estratto
- Chat funzionante collegata ai dati reali del documento caricato
