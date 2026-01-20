# UX / UI Design M\_\_

## 20 gennaio

3. ho aggiunto split button
   - 3.1 ho modificato la creazione di una nuova spedizione rispetto a sketch in Excalidraw: ora è un'opzione esplicita nella tenda dello split button
     - 3.1.1 nota che il titolo della dialog "aggiungi a nuova spedizione" è dinamico: contiene la var "numero di selezionati"
     - 3.1.2 "salva lista" e le altre azioni sono link sottolineati by design, e hanno hover state by design
   - 3.2 ho modificato la creazione di una nuova lista

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
