registrazione: nome, cognome, *ruolo*, stipendio

ruolo: {operatore, responsabile}



responsabile: creare e gestire anagrafica dei prodotti presenti, UI\_RESP, monitora l'andamento del magazzino (operazioni totali \[intervallo temporale])



prodotto: ID\_PROD, nome, descrizione, categoria, \[DISP\_MINIMA] -> opzionale, posizione del prodotto (scaffale/area)



operatore: deve essere autenticato, ha la sua UI\_OPERATORE





sistema: ricerca prodotti {codice, nome, categoria, posizione}, visualizzazione al dettaglio del prodotto {anagrafica, quantità, transazioni associate}, accesso personale garantito





autenticazione: 

UI\_OPERATORE: elenco prodotti presenti; registrare i movimenti (operazioni di carico, scarico), sezione per il suo storico operativo

movimento: prodotto coinvolto, tipo, quantità, data, ID\_OPERATORE





ad ogni movimento il sistema aggiorna automaticamente la quantità disponibile di prodotti

ERRORI: non posso permettere lo scarico di prodotti superiore a quelli fisicamente presenti



UI\_RESP: storico dei movimenti per ogni prodotto (filtri temporali/movimento), visualizza la vista aggiornata del magazzino (elenco, quantità, indicazioni prodotti sotto scorta), area warning per visualizzare eventuali prodotti che necessitano di essere riforniti





quantità: se scende sotto la soglia minima -> segnalazione automatica "sotto scorta" -> area "warning" del gestore







supposizioni: ogni operazione riguarda un solo prodotto per volta (posso intendere come una singola istanza per volta?)







accessibile via web e app, UI RESPONSIVE, notifiche di avviso al responsabile per "prodotti sotto soglia"

