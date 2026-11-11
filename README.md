# Sito del workshop IN-DEPTH 2027

Il sito è pubblicato su https://indepth2027.eu tramite GitHub Pages. Ogni modifica salvata in questo repository va online da sola in circa un minuto.

Tutto il sito sta in `index.html`. Le immagini e i PDF stanno nella cartella `assets`.

## Modificare date, scadenze, email e link del modulo

1. Apri `index.html` su GitHub e clicca sulla matita in alto a destra.
2. Cerca il blocco che inizia con `const CONFIG = {`. Si trova verso la fine del file e si fa prima con Cmd+F.
3. Cambia solo il testo tra virgolette. Per esempio `dates: "15–17 April 2027"` oppure `deadline: "15 January 2027"`. Il link del modulo Google va in `applyUrl`.
4. Clicca su "Commit changes" e conferma.

## Caricare la locandina

1. Nella cartella `assets` clicca su "Add file", poi "Upload files". Trascina il PDF e, se vuoi un'anteprima, anche un'immagine JPG della locandina. Poi clicca "Commit changes".
2. Nel blocco `CONFIG` di `index.html` scrivi il percorso dei file, per esempio:
   `posterPdf: "assets/Poster_IN-DEPTH_2027.pdf",`
   `posterImage: "assets/Poster_IN-DEPTH_2027.jpg",`
3. Salva con "Commit changes". La sezione "Workshop poster" compare da sola nella home.

## Inserire il programma giorno per giorno

Sotto `CONFIG` c'è `const PROGRAMME = [];`. Sopra trovi un esempio commentato da copiare. I tipi disponibili sono `session`, `handson`, `break`, `social` e `other`.

## Se qualcosa non va

Su GitHub, nella scheda "Actions", ogni pubblicazione ha un segno verde o una croce rossa. Se il sito si rompe dopo una modifica, apri la cronologia del file (pulsante "History") e torna alla versione precedente. Spesso il problema è una virgola o una virgoletta mancante nel blocco `CONFIG`.
