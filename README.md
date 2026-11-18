# Sito del Laboratorio P.A.R.O.L.E.

Sito statico: nessuna installazione, si pubblica così com'è con GitHub Pages.

## Struttura

| File | Pagina |
|---|---|
| `index.html` | Home |
| `persone.html` | Persone |
| `progetti.html` | Progetti |
| `risorse.html` | Risorse (pagina generale) |
| `corpora.html` · `didattica.html` · `strumenti.html` | Sottopagine di Risorse |
| `attivita.html` | Attività del Laboratorio (pagina generale) |
| `tesi.html` · `eventi.html` · `terza-missione.html` | Sottopagine di Attività |
| `contatti.html` | Contatti |
| `style.css` | Stile comune (colori, testata, menu) |
| `images/` | Immagini: il logo va salvato come `images/logo.png` |

## Note

- **Logo**: testata e home cercano `images/logo.png`. Se il file ha un altro nome, sostituisci `images/logo.png` nelle pagine.
- **Colore**: il rosso si cambia in una riga sola, `--accent` in cima a `style.css`.
- **Testata e footer** sono ripetuti in ogni pagina: se cambi una voce del menu o l'indirizzo, va aggiornata in tutti i file `.html` (un "trova e sostituisci" sulla cartella basta).
- **Carattere**: Avenir dove è installato (Mac, iPhone, iPad), altrimenti Nunito Sans.
- I testi tra [parentesi quadre] sono segnaposto da sostituire.

## Pubblicazione su GitHub Pages

1. Carica il contenuto di questa cartella nella radice del repository.
2. Nel repository: Settings → Pages → Source: "Deploy from a branch", branch `main`, cartella `/ (root)`.
