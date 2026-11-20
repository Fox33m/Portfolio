# Marco Sansilvestri — Portfolio

Portfolio personale statico, responsive e pubblicabile su GitHub Pages. I contenuti provengono dal portfolio PowerPoint; video e fotografie sono conservati in `assets/`.

## Struttura del progetto

```text
index.html       Struttura e testi della pagina
style.css        Impaginazione, grafica e media query (tablet / mobile)
script.js        Menu mobile e anno del footer
assets/          Fotografie con nomi descrittivi, Logo_Marco.svg e video MP4
.nojekyll        Permette la pubblicazione statica con GitHub Pages
```

I nomi delle fotografie identificano **prodotto e contesto** (es. `lexgo_miro_lungomare.webp`). Le immagini sono in WebP per ridurre il peso; le dimensioni sono gestite con percentuali, `aspect-ratio`, `object-fit` e limiti quando opportuno.

## Pubblicazione su GitHub Pages

1. Crea un repository pubblico su GitHub, ad esempio `portfolio`.
2. Carica **il contenuto** di questa cartella nella radice del repository, non la cartella contenitore. Assicurati che `index.html` sia nella radice.
3. Apri **Settings → Pages** nel repository.
4. In *Build and deployment* scegli **Deploy from a branch**, branch `main`, cartella `/(root)` e salva.
5. Il sito sarà raggiungibile all'indirizzo `https://TUO-USERNAME.github.io/portfolio/`.

## Anteprima locale e manutenzione

Apri `index.html` con Chrome/Edge oppure, per un ambiente più vicino a GitHub Pages, esegui `python -m http.server 8000` dalla cartella del progetto e visita `http://localhost:8000`.

- Modifica testi, contenuti e percorsi delle immagini in `index.html`.
- Modifica colori e layout in `style.css`; le regole responsive sono raggruppate in fondo al file.
- Il JavaScript si limita all'apertura/chiusura del menu mobile e all'anno del footer.
- Mantieni insieme la cartella `assets` e i file principali.
- `assets/lexgo-facility.mp4` è un video HTML5 di circa 21 MB; non eliminarlo.

Il layout carica i font Google quando è disponibile internet, con fallback di sistema.
