# React Animali Preferiti

## Descrizione
Esercitazione per imparare a integrare React direttamente in una pagina HTML senza toolchain avanzate, concentrandosi su componenti, stato, eventi e gestione asincrona.  
L’obiettivo è creare una lista di animali dinamica con possibilità di aggiunta tramite interazione utente e API.

## Milestone 1 — Inserire un Componente React
- Montare un componente React nell’elemento con classe `.lista-animali`  
- Il componente include un `<details>` con titolo "Animali"  
- Mostrare una lista statica `<ul>` di animali generata da un array  
**Obiettivo:** visualizzare la struttura base della lista e usare `<details>` per espandere/contrarre

## Milestone 2 — Aggiungere Animali Casuali
- Trasformare l’array iniziale in uno stato tramite `useState`  
- Aggiungere bottone "Aggiungi Animale" sopra il `<details>`  
- Al click, aggiungere un animale casuale preso da array predefinito  
- Mostrare dinamicamente il nuovo animale nella lista  
**Obiettivo:** permettere all’utente di aggiungere elementi dinamicamente

## Milestone 3 — Usare una Modale per Aggiungere Animali
- Partire dal componente Modal fornito, con portal React  
- Modificare la modale per avere:
  - `content` che può contenere un componente qualsiasi
  - due bottoni: Annulla e Conferma
  - prop `onConfirm` per gestire l’azione di conferma
- Sostituire l’aggiunta casuale con una modale interattiva:
  - Aprire la modale al click del bottone "Aggiungi Animale"
  - Input testo per inserire il nome dell’animale
  - Conferma: aggiunge l’animale alla lista
  - Annulla: chiude la modale senza modifiche
**Obiettivo:** gestire input utente e modificare lo stato attraverso la modale

## Bonus — Utilizzare l’API per Creare Card
- Chiamare `/animals?search=[animalName]` con il nome inserito
- Gestire lo stato di caricamento ("Caricamento...")  
- Dal primo risultato creare un oggetto con:
  - `name`: nome dell’animale  
  - `description`: descrizione o messaggio predefinito  
  - `image`: immagine o default  
- Aggiungere alla lista e visualizzare come card:
  - Titolo, immagine, descrizione
- Gestire errori:
  - Nessun risultato → messaggio "Nessun animale trovato"  
  - Problemi di rete → messaggio "Errore durante la ricerca dell’animale"  
**Obiettivo:** imparare a fare chiamate API, gestire stati di caricamento e errori, visualizzare dati dinamici in React

## Tecnologie
- React (senza toolchain)  
- useState, useEffect  
- Eventi e gestione modale  
- Fetch API e gestione asincrona  
- React Portals

## Scopo
Apprendere l’uso di React direttamente in HTML, creando componenti interattivi, gestendo stato, input utente, modali e chiamate API.
