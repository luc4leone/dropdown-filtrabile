# Dropdown Filtrabile

## Descrizione dettagliata Interactions

### Apertura e Chiusura

- **Click sull'input**: Apre/chiude la tendina discesa
- **Click fuori dalla componente**: Chiude automaticamente la tendina se aperta
- **Tasto Escape**: Chiude la tendina se aperta
- **Frecce Su/Giù**: Se la tendina è chiusa, la apre automaticamente

### Filtraggio

- **Digitazione nell'input**: Filtra le opzioni in tempo reale mostrando solo quelle che contengono il testo digitato
- **Filtro case-insensitive**: La ricerca non distingue tra maiuscole e minuscole
- **Ricerca parziale**: Trova le opzioni che contengono il termine digitato in qualsiasi posizione
- **Nessun risultato**: Mostra il messaggio "Nessun risultato trovato" se il filtro non produce risultati

### Selezione con Mouse

- **Click su elemento**: Seleziona l'elemento cliccato e chiude la tendina
- **Hover**: Evidenzia visivamente l'elemento su cui si passa il mouse
- **Elemento selezionato**: Mostra un background diverso per l'elemento attualmente selezionato

### Navigazione con Tastiera

- **Freccia Giù**: Sposta l'evidenziazione verso il basso nella lista
- **Freccia Su**: Sposta l'evidenziazione verso l'alto nella lista
- **Enter**: Seleziona l'elemento attualmente evidenziato
- **Navigazione ciclica**: Non è ciclica - si ferma al primo/ultimo elemento

### Comportamento dell'Input

- **Valore preselezionato**: Quando si clicca sull'input con un valore già selezionato, tutto il testo viene selezionato
- **Sostituzione rapida**: Dopo aver selezionato tutto il testo, iniziare a digitare sostituisce completamente il valore
- **Placeholder**: Mostra "Cerca o seleziona un elemento..." quando l'input è vuoto

### Gestione della Lista

- **Posizionamento automatico**: Quando si riapre la tendina, si posiziona automaticamente sull'elemento precedentemente selezionato
- **Scroll automatico**: L'elemento evidenziato viene automaticamente reso visibile nella lista
- **Reset del filtro**: Dopo aver selezionato un elemento, alla prossima apertura vengono mostrate tutte le opzioni disponibili

### Feedback Visivo

- **Freccia**: Ruota quando la tendina è aperta
- **Bordi**: L'input cambia aspetto quando la tendina è aperta (bordi arrotondati solo in alto)
- **Evidenziazione**: L'elemento navigato con la tastiera viene evidenziato visivamente
- **Elemento selezionato**: L'elemento attualmente selezionato ha un background distintivo

### Comportamento di Ricerca

- **Ricerca incrementale**: Il filtro si applica ad ogni carattere digitato
- **Apertura automatica**: La tendina si apre automaticamente quando si inizia a digitare
- **Mantenimento selezione**: L'elemento selezionato rimane evidenziato anche quando il filtro è attivo

### Stato della Componente

- **Selezione persistente**: Il valore selezionato rimane nell'input anche dopo la chiusura
- **Stato iniziale**: All'apertura iniziale non c'è alcun elemento selezionato
- **Recovery**: Dopo una selezione, la componente "ricorda" l'elemento scelto per le interazioni successive
