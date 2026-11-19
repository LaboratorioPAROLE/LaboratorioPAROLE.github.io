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
- **Loghi delle risorse** (corpora, piattaforme, strumenti): ogni scheda può avere un'immagine quadrata a sinistra. Per metterla, sostituisci `<span class="res-logo placeholder" aria-hidden="true">Logo</span>` con `<img class="res-logo" src="images/nome-file.png" alt="Nome della risorsa">`. Se la risorsa non ha un logo, elimina quella riga: il testo si allinea da solo a sinistra.
- **Filtri per categoria** (corpora, didattica, strumenti): ogni scheda ha le sue etichette scritte all'apertura, per esempio
  `<article data-lingua="italiano; latino" data-modalita="scritto" data-tipo="diacronico" …>`.
  Più valori si separano con `;`. Le tendine si riempiono da sole con tutti i valori presenti nella pagina, in ordine alfabetico: basta scrivere una lingua nuova su una scheda perché compaia nel filtro. Scrivete i valori sempre allo stesso modo ("italiano", non a volte "Italiano" o "ita"), altrimenti compaiono come voci diverse.
  Categorie per pagina: corpora → `data-lingua`, `data-modalita`, `data-tipo` (diacronico, sincronico, parallelo…) · didattica → `data-disciplina`, `data-lingua` · strumenti → `data-tipo`, `data-livello`.
  I valori attuali sulle schede segnaposto sono solo esempi da sostituire.
- **Ricerca** (corpora, didattica, strumenti): la barra filtra le schede della pagina mentre si scrive, cercando nel testo della scheda (nome, descrizione, lingua, licenza…) senza badare a maiuscole e accenti. Per far trovare una scheda anche con parole che non compaiono nel testo, aggiungile all'apertura della scheda: `<article data-keywords="italiano parlato dialetti trascrizione" style="…">`.
- **Loghi di Università e Dipartimento**: sono nella fascia bianca in cima al footer, in ogni pagina (cerca `footer-logos` nel file). Le immagini sono `images/logo_unisa.png` e `images/logo_dipsum.png`; l'altezza si cambia con `height: 44px` e `height: 34px`, il link con `href`. Per toglierli, elimina tutto il blocco `<div class="footer-logos" …> … </div>`.
- **Colore**: il rosso si cambia in una riga sola, `--accent` in cima a `style.css`.
- **Testata e footer** sono ripetuti in ogni pagina: se cambi una voce del menu o l'indirizzo, va aggiornata in tutti i file `.html` (un "trova e sostituisci" sulla cartella basta).
- **Carattere**: Avenir dove è installato (Mac, iPhone, iPad), altrimenti Nunito Sans.
- I testi tra [parentesi quadre] sono segnaposto da sostituire.

## Pubblicazione su GitHub Pages

1. Carica il contenuto di questa cartella nella radice del repository.
2. Nel repository: Settings → Pages → Source: "Deploy from a branch", branch `main`, cartella `/ (root)`.
