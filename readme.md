# UX / UI Design M\_\_

## _todo_
- [ ] *completa scheda testata*
- [ ] *suggerimenti AI*
- [ ] *disegnare Account*
- [ ] *mobile app*
- [ ] *filtro sede giornalista*
- [ ] *nuove statistiche proposte per dashboard*

## _in progress_
- [ ] *completa scheda giornalista*
  - adeguamento a UI in https://luc4leone.github.io/mediaddress-grafica/examples/index.html
  - non ovvio: cmd/enter -> ok, esc -> cancel in editor note e in input servizio
  - finite sezioni header, note, servizi, contatti diretti
    - todos:
      - [x] valuta apri / chiudi sezioni, in particolare sezione  "note"
      - [ ] da "ok" a "aggiungi"
      - [x] fix width input, select, textarea
      - [x] sposta nome in header (togli titolo "giornalista")
      - [x] sposta ok annulla su stessa riga input
      - [x] nuovo stile sotto-sezione contatti diretti
      - [x] aggiungi split button per aggiungi lista / spedizione


## 27 gennaio 2026

- [x] **aumentato padding verticale link in nav bar**

## 24 gennaio 2026

- [x] **reso il layout più fluido**
  - ora all'allargarsi dello screen le cards per riga non si allargano più a dismisura, si allargano finchè c'è spazio per aggiungere un'altra card
- [x] **modificato nome "filtra banca dati" in nav bar**
  - modificato anche titolo e nome link per modificare la banca dati
- [x] **separati in nav bar comunicati e spedizioni**
- [x] **modificata interaction "rimuovi card" in lista**
  - x in card appare on mouse over 
- [x] **allineata grafica a landing page marketing**
  - squadrato split button
  - squadrato dropdown ordinamento cards
  - squadrato chips selezionati
  - squadrato in dashboard chips giornalisti in lista mailing list
  - sostituito h in hsl di tutta la scala di grigi
- [x] **migliorata grafica**
  - resi più scuri i testi dei valori dei campi (servizio giornalistico: mostre -> ora mostre è più scuro)
  - fixato regressione su color card note value
  - aggiunta ombreggiatura a cards
- [x] **migliorato dettaglio di interaction**
  - chevron ruota su controllo "ordina" in main, e split button in panel selezionati

## 23 gennaio 2026

- [x] **allineata grafica a landing page marketing**
  - sostituito type
  - modificato radius filtri e chips
  - modificato background color nav sidebar
  - modificato color active link nav sidebar
  - sostituito logo
  - modificato il blue dei link

## 21 gennaio 2026

- [x] **aggiunto funzionalità "condividi mailing list"**
  - ho aggiunto l'autore della mailing list, nel proto è una valore statico perché non ho sviluppato il concetto di user del programma, quindi tutte le mailing list sono create da @ugo
- [x] **aggiunto funzionalità "elimina mailing list in mailing list"**
  - così lo user può eliminare una mailing list sia dalla lista delle mailing list che dalla mailing list stessa


## 20 gennaio 2026

- [x] **aggiunto funzionalità "rimuovi selezionati da mailing list"** -> in mailing list, seleziona giornalista -> vedi riga 2 dall'alto nel panel selezionati
  - questa riga viene mostrata solo in lista, non cross viste (non per es in filtra)
- [x] **aggiunto action link "rimuovi da lista"** in card in lista
- [x] **rinominate le opzioni del menu dello split button** (potremmo chiamarlo "split link" 😉). ora sono logiche (@fabio 💪), vediamo se nei test di usabilità sono comprensibili
- [x] **tolto action link "deseleziona tutti"** da main, era ridondante e forse fuorviante (@fabio 💪)
- [x] **rinominato action link "rimuovi selezionati"** in "svuota selezione" in panel selezionati per evitare confusione con action link riga sopra "rimuovi da lista"

---

facendo riferimento al punto 3 del 19 gennaio:

- [x] aggiunto split button
  - [x] modificato la creazione di una nuova spedizione rispetto a sketch in Excalidraw: ora è un'opzione esplicita nella tenda dello split button
    - il titolo della dialog "aggiungi a nuova spedizione" è dinamico: contiene la var "numero di selezionati"
    - "salva lista" e le altre azioni sono link sottolineati by design, e hanno hover state by design
  - [x] modificato patter per la creazione di una nuova spedizione

## 19 gennaio 2026

> 1. ordinamento: preferiamo una tendina, i problemi della soluzione proposta sono:
>    •⁠ ⁠non scala su schermi piccoli
>    •⁠ ⁠⁠non scala se vogliamo aggiungere altre voci (attualmente, intendo mdddr6, l’ordinamento di default è per testata e quasi nessuno lo cambia, nello schema proposto non è neanche disponibile)
> 2. l’accoppiamento nel menù di sx di “comunicati e spedizioni” non ci convince
> 3. la soluzione per eliminare lo “split button” nel menù dei selezionati sembra poco leggibile e il pattern per creare una nuova spedizione o aggiungere a una spedizione esistente è diverso dal pattern per creare una nuova lista o aggiungere a una lista esistente

---

elenco puntato numerato fa riferimento a quello sopra:

1. ho sostituito il sort control in "filtra banca dati"

- 1.1 dato che è un prototipo lascio perdere "aggiungere criterio testata" - sarebbe "testata a-z"?
- 1.2 su mobile non metterei nemmeno il controllo

2. non convince al 100% nemmeno me; nasce dal fatto che la lista dei comunicati e la lista delle spedizioni ripetono spesso gli stessi dati (titolo, autore, data creazione); lo terrei così per ora
3. IN PROGRESS
4. modificato colore active element in nav bar

## 16 gennaio 2026

### SIDEBAR NAV

- aggiunto link "mailing list"
- eliminato "nuova spedizione"
- modificati links
  “nuovo comunicato” -> “comunicati e spedizioni”
  “nuovo progetto” -> “progetti”
  “nuovo todo” -> “todos”
- cambiato background color active element

### SIDEBAR "SELEZIONATI"

- split button diviso in 3 bottoni
- aggiunta funzione "aggiungi a lista"
- nella dialog ho una dropdown filtrabile con un termine (vengono filtrate le liste che hanno almeno una parola che inizia con il termine inserito)
- aggiunta funzione "aggiungi a spedizione" (ho sostituito "destinatari" con "spedizione)
- spostate le dialog + in alto, non sono + centrate verticalmente; inoltre rispetto alla larghezza di "salva lista" sono state allargate

### MAIN

- spostato il blocco di controlli "seleziona tutti... ordina:"
- aggiunti ordinamenti sia in modalità "giornalisti" che "testate"
- giornalisti -> aggiunti ruolo z-a, tipo di media, frequenza
- testate -> aggiunti tipo di media, frequenza
- modificato link "scegli Banca Dati" -> "banca dati"

### BUG FIX

- seleziona giornalista, vai in dashboard, torna in filtra, la sidebar "selezionati" era chiusa, DEVE ESSERE APERTA

### MISC

- uniformato copy: tolto "mailing list/s" ovunque, sostituito con "lista/e".
