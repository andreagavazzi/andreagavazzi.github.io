---
title: L'inventario
date: 2023-02-01 16:27:00 +0100
categories: [Tutte le aree, Ricambi]
tags: [ricambi, inventario, rettifiche]     # TAG names should always be lowercase
pin: true
---

## Introduzione
L’inventario è gestito in sistema tramite un giornale di registrazione che, in automatico, raccoglie tuti gli articoli che rispecchiano le condizioni scelte dall’utente.
Gli articoli nel giornale verranno quindi conteggiati, con supporto cartaceo o tramite scanner. Le differenze rilevate saranno automaticamente trasferite in una rettifica inventariale.

> Un articolo inserito nel giornale di conteggio e già contato non sarà disponibile per altre registrazioni (acquisto, vendita, trasferimento, …). È buona normale pertanto avere tanti piccoli giornali con un minimo numero di righe.
{: .prompt-warning}

# Creazione del giornale
Entrare in Gestione articoli / Scritture contabili / Conteggio articoli / Conteggio

![02](/assets/img/02/01.png)

Creare un nuovo giornale premendo “Nuovo” (1)  
Verificare la correttezza di sito e magazzino (2)  
Abilitare magazzino e ubicazione (3)  
Nel caso si volessero utilizzare gli scanner abilitare la voce “Rilascio su mobile” (5). È comunque possibile abilitare questa funzione anche successivamente.  
Inserire la persona che sta facendo il conteggio (4)  

 
# Inserimento delle righe
Scegliere dal menu “Crea righe” la voce “Disponibilità”
 

In questa schermata è necessario selezionare la combinazione di parametri e di filtri che porteranno alla creazione delle righe articoli nel giornale.
1.	Parametri
 

Data di conteggio: la data in cui si esegue il conteggio.
Non contati da: l’elenco includerà tutti gli articoli che, a partire dalla data inserita, non sono mai stati contati (il sistema controlla la Data di conteggio).
Includere articoli senza disponibilità: deve essere attivo in quanto è necessario contare anche quegli articoli per i quali non ho disponibilità in sistema. Potrei infatti avere disponibilità fisica
Ho poi un gruppo di parametri che vanno abilitati e indicano al sistema come produrre la lista: Configurazione, Magazzino, Stato inventario, Ubicazione.

2.	Record da includere (filtro)
Accedere al filtro per definire ulteriormente l’elenco degli articoli proposti dal sistema
  
# Inserimento dei filtri
 
Es. Con questa selezione sto chiedendo al sistema di elencarmi tutti gli articoli del magazzino ricambi di Leno che hanno a che fare con gli scaffali 20001A, 20001B, 20001C, 20001D, 20001E.
N.B. In appendice è presente un elenco sulla sintassi nei filtri.

Definire anche l’ordinamento in modo da avere una lista più facilmente consultabile.
 
Prestare attenzione alle tabelle scelte. Nell’esempio qui sopra il sistema ordinerà in modo crescente per Ubicazione e, all’interno di una stessa ubicazione, per numero articolo.
Premere “OK” e, verificati i parametri, ancora “OK”
 
Dopo qualche secondo il sistema mi inserirà tutte gli articoli che rientrano nei parametri impostati
 

Come in tutte le liste di D365 è possibile inserire ulteriori colonne come di consueto. Ubicazione e Prezzo di costo sono senza dubbio importanti.

> La colonna “Ubicazione”, come tutte le colonne relative alle dimensioni, deve essere aggiunta in questo modo:
{: .prompt-warning} 

Nel caso fosse stato commesso un errore durante la scelta dei parametri o dei filtri è possibile eliminare tutte le righe tramite il menu Funzioni / Elimina righe giornale di registrazione
 
È inoltre possibile inserire manualmente nuove righe nel giornale stesso. Utile per apportare piccole correzioni.

Conteggio con supporto cartaceo
Tramite la funzione “Stampa / Elenco di conteggio” verranno prodotte le stampe che accompagneranno l’utente tra gli scaffali.
 

Lasciare disabilitata l’opzione “Stampa disponibilità” e premere OK
 

N.B.: La stampa ottenuta è attualmente in corso di revisione
 
 
Quanto contato su carta deve essere trasferito in D365 utilizzando il campo “Contato” (1)
Il sistema avviserà (2) qualora il costo di un articolo sul quale è necessaria una rettifica non fosse presente. Tale costo (3) deve essere inserito manualmente prima di registrare il giornale.
 

# Conteggio con scanner
La preparazione del giornale (da pag.1 a pag.5) non cambia. Riferirsi pertanto a questa sezione.
Una volta creato il giornale con l’elenco degli articoli da contare, verificare che l’opzione “Rilascia su Mobile” sia attiva. Solo in questo caso il giornale sarà visualizzato sullo scanner.
 
 
Sullo scanner seleziona la voce “Count”. Verranno mostrati tutti i giornali di conteggio aperti (uno solo in questo caso). Toccare quello che si intende processare per portarsi al suo interno. 
Al fine di non condizionare l’utente che esegue il conteggio, sullo scanner non saranno mostrate le quantità attualmente disponibili in sistema. La colonna delle quantità indica invece il valore del conteggio.

![14](/assets/img/02/14.png){: .left w="250"}  
![15](/assets/img/02/15.png){: .left w="250"}  
![16](/assets/img/02/16.png){: .left}  
<br>

È possibile (ma non obbligatorio) ridurre la lista mostrata filtrando sull’ubicazione desiderata: Scansionare il QR code dell’ubicazione per applicare il filtro.
Per passare ad un’altra ubicazione sarà sufficiente scansionare il nuovo QR code, il filtro si modificherà di conseguenza
Per eliminare il filtro e visualizzare nuovamente l’intero giornale, toccare la “x”
 

Scansionare il codice articolo da contare, confermare l’ubicazione attuale (non è possibile un trasferimento di ubicazione durante il conteggio inventariale). Inserire la quantità contata e confermare.
         

È ora possibile continuare il conteggio scansionando un altro articolo o l’ubicazione successiva. 

# Conteggio ripetuto e gestione errori
Quando si inserisce la quantità di un articolo, fare attenzione a quanto indicato sullo schermo: se è presente la barra verde allora l’articolo è già stato contato (viene mostrato anche il valore).
Un nuovo input si somma a quello già presente. Il che in alcuni casi potrebbe essere utile per modificare, ma solo in aumento, un conteggio precedente.
     

Per modificare un conteggio tenere premuto sulla riga interessata e dal menu scegliere “Registrations”. Verranno visualizzati tutte le registrazioni effettuate sulla la riga selezionata.
Toccando brevemente una registrazione sarà possibile modificarne la quantità, mentre tenendo premuto sarà possibile accedere al menu contestuale ed eliminare la registrazione stessa (Delete line). È ora possibile tornare alla pagina principale.
         

# Invio a D365
Per trasferire a sistema il conteggio finora effettuato selezionare dal menu     la funzione “Post”. Dopo qualche secondo un messaggio avviserà del completamento dell’operazione. Quanto sullo scanner verrà trasferito in D365.
         
 
In D365, le righe contate tramite scanner saranno evidenziate dal segno di spunta
 
A: articoli contati con lo scanner
B: articoli contati manualmente

# Registrazione rettifiche
Terminato l’inserimento e le opportune verifiche del caso, è possibile convalidare e registrare il giornale.
Tutte le righe devono essere state contate, cioè deve esserci un valore nella colonna “Contato”
 

Il sistema procederà a rettificare quegli articoli che hanno una differenza positiva o negativa tra disponibile e contato. L’operazione si concluderà dopo qualche secondo. 
Tramite la funzione “Visualizza registrazioni” è possibile verificare le registrazioni effettuate ed il giustificativo prodotto
