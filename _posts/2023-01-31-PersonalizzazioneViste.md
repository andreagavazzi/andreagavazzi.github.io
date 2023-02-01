---
title: La personalizzazione delle viste
date: 2023-01-31 23:19:00 +0100
categories: [Generale, Sistema]
tags: [personalizzazioni]     # TAG names should always be lowercase
---

La personalizzazione delle viste permette di salvare la disposizione delle colonne e l’impostazione dei filtri in modo da richiamarli all’occorrenza.  
A titolo d'esempio concreto, pensiamo ad un utente che debba consultare quotidianamente un elenco di ordini ricambi non ancora fatturati ai clienti della sede di Leno.  
Partendo dalla vista “Tutti gli ordini clienti” potrà impostare i filtri e le colonne e memorizzarli in una vista dedicata.
Potrà creare quante viste desidera (es. una per ordini macchine, una per ordini ricambi, una per sede, ecc..).  

> Un amministratore di sistema potrà trasferire la vista creata ad altri colleghi che la troveranno disponbile nel proprio menu.
{: .prompt-tip}

![01](/assets/img/01/personalizzazione01.png){: w="700" .left}


Esempio: organizzazione colonne
Partendo dalla vista “Tutti gli ordini cliente” applico i filtri e aggiungo e/o sposto le colonne in modo da arrivare alla visualizzazione desiderata.
L’idea dell’esempio, è quella di avere un report degli ordini clienti ancora da fatturare.

In questo caso, rispetto alla vista standard, ho:
- Aggiunto e ordinato alcune colonne (Pool, Magazzino, Stato ordine, …)
- Applicato i filtri in modo da ottenere tutti gli ordini di Leno, magazzino ricambi, non pertinenti l’attività officina, in stato Aperto o Consegnato. 
- Da notare che il titolo della vista, “My view” in questo caso, ha un (*). Significa che quella vista è stata modificata e non salvata. Se uscissi, perderei quanto fatto. 
A questo punto posso salvare la mia vista in modo da richiamarla in seguito.

Esempio: salvataggio vista
Per salvare portarsi nel menu di vista e selezionare “salva con nome” (oppure “salva” se la vista è stata salvata in precedenza).
 
Attribuire un nome (1) ed una descrizione (2) alla propria vista. È possibile impostarla come predefinita (3) e salvare (4).
NB. Se imposto la vista come predefinita, ogni volta che entrerò nella lista “tutti i clienti” avrò la mia personalizzazione (comunque modificabile).
 
Le viste salvate saranno ora disponibili nel menu di vista assieme alla visualizzazione standard (che è quella classica di sistema non è sovrascrivibile né cancellabile)
 
Richiamare una vista salvata
Continuando con il nostro esempio è sufficiente entrare nella lista “Tutti gli ordini clienti” e selezionare la vista che mi interessa dal menu (1).
 
 
Funzioni aggiuntive
Nel menu di vista è presente un sotto-menu con alcune funzioni importanti
 
Aggiungi come predefinita: imposta la vista corrente come predefinita
Personalizza: 	è il classico menu di personalizzazione, ha poca rilevanza qui
Pubblica: permette di pubblicare la vista ad un gruppo di utenti (ruolo aziendale). Dato che la vista sarà disponibile a tutti gli utenti di D365 che hanno il ruolo scelto, vi consiglio di contattare il vostro Key User prima di procedere.
 
Gestisci le mie visualizzazioni: mostra un elenco delle proprie viste (riferite alla sola lista corrente). È qui possibile modificare, rinominare oppure eliminare una o più viste.

