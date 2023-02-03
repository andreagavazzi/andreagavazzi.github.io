---
title: Il primo accesso al sistema
date: 2023-01-31 23:29:00 +0100
categories: [Generale, Sistema]
tags: [personalizzazioni]     # TAG names should always be lowercase
pin: true
---


> Le schermate qui proposte si riferiscono ad un ambiente standard Microsoft e, pur mantenendo le stesse funzionalità, differiscono per impatto visivo.
{: .prompt-info }


## Login

L’accesso a Dynamics 365 avviene tramite browser da qualsiasi dispositivo e senza necessità di una connessione VPN utilizzando le proprie credenziali (indifferentemente l’indirizzo mail oppure lo username). È raccomandato l’utilizzo di Edge.

![01](/assets/img/03/01.png)
<br>
 
Ogni utente ha uno o più ruolo assegnato in base alle funzioni anziendali che svolge, quindi, ad esempio, chi si occupa di ricambi avrà delle funzioni che chi si occupa di macchine non troverà.

## Homepage
La prima schermata, che può essere altamente personalizzata raccoglie più elementi

![02](/assets/img/03/02.png)
<br>

Ci sono due elementi fondamentali in sistema: le **aree di lavoro** e i **moduli**
L'area di lavoro è un cruscotto che visualizza degli indicatori, mostra report, racchiude link per accedere ai moduli.  
I moduli sono le zone in cui vengono svolte le normali operazioni di sistema.  

1.	Aree: presenta l’accesso alle aree di lavoro che raccolgono le funzioni raggruppate per ruolo utente. Ogni riquadro permette l’accesso ad un’area specifica.
2.	Bottone hamburger: qui troviamo il menu con i diversi moduli di sistema
3.	Barra menu
4.	Eventuali azioni assegnate all’utente
 
## Opzioni utente
Le opzioni utente sono accessibili dal bottone ingranaggio e racchiudono diverse scelte che permettono di impostare gli elementi principali del sistema.

![03](/assets/img/03/03.png)
<br>

**Visivo** 
L’area permette di selezionare il colore dell’interfaccia e la relativa dimensione  

![04](/assets/img/03/04.png)
<br>

> Si raccomanda di lasciare il colore predefinito e di selezionare la dimensione più compatta
{: .prompt-warning }

**Preferenze** 
In questo blocco troviamo le impostazioni di lingua e paese che permettono, tra le altre cose, di cambiare il formato data.  

![05](/assets/img/03/05.png)
<br>


## La navigazione
Ci sono due modi principali per accedere ai moduli, il campo di ricerca e il menu "hamburger".
Il campo di ricerca (lente di ingrandimento) permette di trovare aree di sistema in base al loro nome (es. tutti i clienti) mentre il menu "hamburger" elenca tutte le aree e tutti i moduli disponibili.  

![06](/assets/img/03/06.png)
<br>

## Le aree di lavoro
Come detto, un'area di lavoro racchiude diversi elementi e permette un rapido accesso alle informazioni più ricorrenti. Benchè personalizzate per ruolo e personalizzabili per utente, le aree di lavoro sono simili tra loro per impostazione.  

![07](/assets/img/03/07.png)
<br>

1.	Nella parte di sinistra troviamo i riquadri, con indicatori, che danno immediato accesso alle liste.
2.	Nella parte centrale troviamo le liste stesse
3.	Nella parte destra ci sono i collegamenti ai moduli

## I moduli
I moduli si presentano all'utente come liste di dati. Ogni riga è un dato (es. un cliente, una macchina, un ordine fornitore, ...). I moduli rappresentano il fultro dell'attività in sistema.  

![08](/assets/img/03/08.png)
<br>

1.	Ogni colonna ha il suo filtro
2.	Qui troviamo la possibilità di definire i parametri di ricerca
3.	Nel campo di inserimento del testo è possibile utilizzare il carattere jolly *

Il campo di ricerca che troviamo sopra alla lista è utilizzabile come filtro, ma racchiude solo pochi campi predefiniti.  
 
![09](/assets/img/03/09.png)
<br>

Sulla sinistra, il bottone con il simbolo dell'imbuto, dà accesso ad un riepilogo dei filtri applicati e offre la possibilità di applicarne ulteriori raffinando la ricerca.  

![10](/assets/img/03/10.png)
<br> 


Informazioni correlate
Sulla destra delle liste solitamente troviamo il menu che mostra alcune informazioni relative alla riga selezionata.
 

Rientro a menu principale
Lo spostamento tra i moduli è possibile da diversi punti
 
1.	Direttamente dal menu moduli
2.	Chiudendo le viste aperte
3.	Cercando il modulo desiderato per passare direttamente alla funzione scelta

Salvataggio
Il salvataggio di ogni modifica avviene in modo automatico uscendo dal campo stesso oppure tramite la pressione del bottone di salvataggio
 


 
Personalizzazione Liste
Nelle viste troviamo normalmente 3 parti principali
 
1.	Tab dei menu
2.	Funzioni
3.	Lista
È possibile personalizzare le liste, salvando inoltre i filtri inseriti sulle colonne come link nella propria area di lavoro
Inserimento colonne
Sebbene esistano diversi modi, quello suggerito da Microsoft è il seguente:
 

1.	Tab Opzioni
2.	Personalizza modulo: comparirà la barra di personalizzazione
3.	Inserisci campo
4.	Click sulla lista (il sistema si aspetta che gli diciamo dove inserire il campo)
Selezionare le colonne da aggiungere alla lista
 

N.B. sebbene siano presenti nella lista delle colonne da poter aggiungere, i campi relativi alle dimensioni devono essere inseriti dall’apposito menu.
Es. da Gestione delle macchine>Macchine>Tutte le macchine
 
Selezionare “Salva impostazione” per memorizzare l’inserimento delle colonne selezionate.
Spostamento colonne
Anche lo spostamento della colonna viene fatto dalla barra di personalizzazione
 

1.	Selezionare il simbolo di spostamento
2.	Evidenziare la colonna da spostare
3.	Tramite i tasti freccia (da tastiera) collocare la colonna nella posizione desiderata
4.	Premere il tasto invio
La modifica delle liste richiederà spesso la ricarica del modulo (tasto F5)

 
Salvataggio della personalizzazione
Il salvataggio della personalizzazione è fatto automaticamente dal sistema per il proprio utente.

Esportazione e importazione della personalizzazione
È possibile esportare il layout su un file .xml, passarlo ad un altro utente che lo importerà.
Anche l’esportazione del layout viene fatto dalla barra di personalizzazione
 
1.	Esporta: equivale a salvare un file da internet. La cartella predefinita di Google Chrome sarà quella Download.
2.	Importa: selezionare il file layout sostituendolo all’attuale
 
3.	Cancella: riporta la lista alla visualizzazione originale senza cancellare il file layout precedentemente generato

 
Aggiungere in Area di Lavoro
È possibile salvare la lista personalizzata (anche avendo inserito alcuni filtri) tramite il menu “Aggiungi ad area di lavoro”
 
1.	Scegliere l’area di lavoro a cui aggiungere la lista
2.	Selezionare il tipo di presentazione
1.	Riquadro: è il quadrato sulla sinistra con il riepilogo del nr.linee presenti
2.	Elenco: è un’anteprima della lista. Solo 8 colonne possono essere visualizzate
3.	Collega: è il semplice link qui a sinistra
 

Funzioni utili
Aggiornare le viste
Premere la freccia circolare (1) per aggiornare una vista ricaricandone il contenuto. Premere la freccia circolare sulla barra del browser (2) per ricaricare l’intera pagina.
 

Esportare in Excel
Premendo il tasto destro sul titolo di colonna è possibile esportare tutte le righe o solo quelle selezionate
 

 
Aprire in nuova finestra
Premendo con il tasto destro del mouse sul tab del browser e selezionando duplica, si aprirà un secondo tab copia esatta del primo
 
Premendo l’icona disancora (2) la vista attuale verrà sganciata dal browser che verrà riportato in homepage
