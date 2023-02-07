---
title: L'inventario
date: 2023-02-01 16:27:00 +0100
categories: [Tutte le aree, Ricambi]
tags: [ricambi, inventario, rettifiche]     # TAG names should always be lowercase
pin: false
---

## Introduzione
L’inventario è gestito in sistema tramite un giornale di registrazione che, in automatico, raccoglie tuti gli articoli che rispecchiano le condizioni scelte dall’utente.
Gli articoli nel giornale verranno quindi conteggiati, con supporto cartaceo o tramite scanner. Le differenze rilevate saranno automaticamente trasferite in una rettifica inventariale.

> Un articolo inserito nel giornale di conteggio e già contato non sarà disponibile per altre registrazioni (acquisto, vendita, trasferimento, …). È buona normale pertanto avere tanti piccoli giornali con un minimo numero di righe.
{: .prompt-warning}

# Creazione del giornale
Entrare in Gestione articoli/Scritture contabili/Conteggio articoli/Conteggio (Inventory management/Journal entries/Item counting/Counting)

![01](/assets/img/02/01.png)
<br>

Creare un nuovo giornale premendo “Nuovo” (1)  
Verificare la correttezza di sito e magazzino (2)  
Abilitare magazzino e ubicazione (3)  
Inserire la persona che sta facendo il conteggio (4)  
Nel caso si volessero utilizzare gli scanner abilitare la voce “Rilascio su mobile” (5), ma è possibile abilitare questa funzione anche successivamente.  

# Inserimento delle righe
Scegliere dal menu “Crea righe” la voce “Disponibilità”

![01a](/assets/img/02/01a.png)
<br>

In questa schermata è necessario selezionare la combinazione di parametri e di filtri che porteranno alla creazione delle righe articoli nel giornale.  

**Parametri**
![02](/assets/img/02/02.png)
<br>

Data di conteggio: la data in cui si esegue il conteggio.  
Non contati da: l’elenco includerà tutti gli articoli che, a partire dalla data inserita, non sono mai stati contati (il sistema controlla la Data di conteggio presente in anagrafica articolo / Gestione articoli / Articoli di Magazzino).  

Includere articoli senza disponibilità: deve essere attivo in quanto è necessario contare anche quegli articoli per i quali non ho disponibilità in sistema. Potrei infatti avere una loro disponibilità fisica.  
Ho poi un gruppo di parametri che vanno abilitati e indicano al sistema come produrre la lista: Configurazione, Magazzino, Stato inventario, Ubicazione.  

**Record da includere (filtro)**
Accedere al filtro per definire ulteriormente l’elenco degli articoli proposti dal sistema
![03](/assets/img/02/03.png)
<br>

# Inserimento dei filtri
![04](/assets/img/02/04.png)
<br>

Es. Con questa selezione sto chiedendo al sistema di elencarmi tutti gli articoli del magazzino ricambi di Leno che hanno a che fare con gli scaffali 20001A, 20001B, 20001C, 20001D, 20001E.
N.B. In appendice è presente un elenco sulla sintassi nei filtri.

Definire anche l’ordinamento in modo da avere una lista più facilmente consultabile.

![05](/assets/img/02/05.png)
<br>

Prestare attenzione alle tabelle scelte. Nell’esempio qui sopra il sistema ordinerà in modo crescente per Ubicazione e, all’interno di una stessa ubicazione, per numero articolo.
Premere “OK” e, verificati i parametri, ancora “OK”
 
Dopo qualche secondo il sistema mi inserirà tutte gli articoli che rientrano nei parametri impostati  

![06](/assets/img/02/06.png)
<br>

Come in tutte le liste di D365 è possibile inserire ulteriori colonne come di consueto. Ubicazione e Prezzo di costo sono senza dubbio importanti.

> La colonna “Ubicazione”, come tutte le colonne relative alle dimensioni inventariali (sito, magazzino, ubicazione,...), deve essere aggiunta tramite l'apposita funzione "visualizza dimensioni":
{: .prompt-warning} 

![07](/assets/img/02/07.png)
<br>

Nel caso fosse stato commesso un errore durante la scelta dei parametri o dei filtri è possibile eliminare tutte le righe tramite il menu Funzioni / Elimina righe giornale di registrazione

![08](/assets/img/02/08.png)
<br>

È inoltre possibile inserire manualmente nuove righe nel giornale stesso. Utile per apportare piccole correzioni.

# Conteggio con supporto cartaceo
Tramite la funzione “Stampa / Elenco di conteggio” verranno prodotte le stampe che accompagneranno l’utente tra gli scaffali.  

![09](/assets/img/02/09.png)
<br>

Lasciare disabilitata l’opzione “Stampa disponibilità” e premere OK  

![10](/assets/img/02/10.png)
<br>

N.B.: La stampa ottenuta è attualmente in corso di revisione  

![11](/assets/img/02/11.png)
<br>
 
Quanto contato tramite supporto cartaceo deve essere copiato in D365 nel campo “Contato” (1)
Il sistema avviserà (2) qualora il costo di un articolo sul quale è necessaria una rettifica non fosse presente. Tale costo (3) deve essere inserito manualmente prima di registrare il giornale.     

![12](/assets/img/02/12.png)
<br>

Salvare quanto fatto e procedere con la <A href="#registrazione">Registrazione</A>.

# Conteggio con scanner
La preparazione del giornale non cambia. Riferirsi pertanto a questa sezione.
Una volta creato il giornale contenente l’elenco degli articoli da contare, verificare che l’opzione “Rilascia su Mobile” sia attiva. Solo in questo caso il giornale sarà visualizzato sullo scanner.  

![13](/assets/img/02/13.png)
<br>

1. Nel menu principale dello scanner seleziona la voce “Count”
2. Verranno mostrati tutti i giornali di conteggio aperti (uno in questo caso). Toccare quello che si intende processare per portarsi al suo interno.
3. Sullo scanner non saranno mostrate le quantità attualmente disponibili in sistema, ma il solo valore conteggiato.  

|                             |                             |                             |
|:----------------------------|:----------------------------|:----------------------------|
| ![14](/assets/img/02/14.png){: w="250"} | ![15](/assets/img/02/15.png){: w="250"} | ![16](/assets/img/02/16.png){: w="250"} |

<br>


> Per semplificare la lista mostrata è possibile scansionare il QR code di un'ubicazione che verrà applicato come un normale filtro alla lista.
Per passare ad un’altra ubicazione sarà sufficiente scansionare il QR code dell'ubicazione successiva, il filtro si modificherà di conseguenza.
Per eliminare il filtro e visualizzare nuovamente l’intero giornale, toccare la “x”
{: .prompt-tip}

![17](/assets/img/02/17.png){: w="250"}  <br>

Scansionare il codice articolo da contare, confermare l’ubicazione attuale (non è possibile effettuare un trasferimento di ubicazione durante il conteggio inventariale). Inserire la quantità contata e confermare.  

|                             |                             |                             |
|:----------------------------|:----------------------------|:----------------------------|
| ![18](/assets/img/02/18.png){: w="250"} | ![19](/assets/img/02/19.png){: w="250"} | ![20](/assets/img/02/20.png){: w="250"} |

<br>


È ora possibile continuare il conteggio scansionando un altro articolo o l’ubicazione successiva. 

# Gestione errori
Quando si inserisce la quantità di un articolo, fare attenzione a quanto indicato sullo schermo: se è presente la barra verde allora l’articolo è già stato contato (viene mostrato anche il valore).
Un nuovo input si somma a quello già presente. Il che in alcuni casi potrebbe essere voluto per modificare, ma solo in aumento, un conteggio precedente.  

|                             |                             |
|:----------------------------|:----------------------------|
| ![21](/assets/img/02/21.png){: w="250"} | ![22](/assets/img/02/22.png){: w="250"} |

<br>   

Per modificare un conteggio tenere premuto sulla riga interessata e dal menu scegliere “Registrations”. Verranno visualizzati tutte le registrazioni effettuate sulla la riga selezionata.
Toccando brevemente una registrazione sarà possibile modificarne la quantità, mentre tenendo premuto sarà possibile accedere al menu contestuale ed eliminare la registrazione stessa (Delete line). È ora possibile tornare alla pagina principale.  

|                             |                             |                             |
|:----------------------------|:----------------------------|:----------------------------|
| ![23](/assets/img/02/23.png){: w="250"} | ![24](/assets/img/02/24.png){: w="250"} | ![25](/assets/img/02/25.png){: w="250"} |

<br>

# Invio a D365
Per trasferire a sistema il conteggio finora effettuato selezionare dal menu la funzione “Post”. Dopo qualche secondo un messaggio avviserà del completamento dell’operazione. Quanto sullo scanner verrà trasferito in D365.  

|                             |                             |                             |
|:----------------------------|:----------------------------|:----------------------------|
| ![26](/assets/img/02/26.png){: w="250"} | ![27](/assets/img/02/27.png){: w="250"} | ![28](/assets/img/02/28.png){: w="250"} |

<br>
       
In D365, le righe contate tramite scanner saranno evidenziate dal segno di spunta

![29](/assets/img/02/29.png)
<br>

A: articoli contati con lo scanner
B: articoli contati manualmente

# Registrazione #
Terminato l’inserimento e le opportune verifiche del caso, è possibile convalidare e registrare il giornale.
Tutte le righe devono essere state contate, cioè deve esserci un valore nella colonna “Contato”  

![30](/assets/img/02/30.png)
<br>

Il sistema procederà a rettificare quegli articoli che hanno una differenza (positiva o negativa) tra disponibile e contato. L’operazione si concluderà dopo qualche secondo. 
Tramite la funzione “Visualizza registrazioni” è possibile verificare le registrazioni effettuate ed il giustificativo prodotto  

![31](/assets/img/02/31.png)
<br>

![32](/assets/img/02/32.png)
<br>

# Sintassi nei filtri


|     Descrizione                                |     Sintassi                |
|------------------------------------------------|-----------------------------|
|     Uguale a 20001A                            |     20001A                  |
|     Diverso da 20001A                          |     !20001A                 |
|     Uguale a 20001A,   20002A, 20003A          |     20001A,20002A,20003A    |
|     Contiene 20001                             |     *20001*                 |
|     Non contiene 20001                         |     !*20001*                |
|     Inizia con 2                               |     2*                      |
|     Superiore a 20001C                         |     >20001C                 |
|     Superiore o   uguale a 20001C              |     20001C..                |
|     Inferiore a 20001C                         |     <20001C                 |
|     Inferiore o   uguale a 20001C              |     ..20001C                |
|     Tra 20001A e 20001C   (estremi inclusi)    |     20001A..20001C          |

<br>

# Barcode e QR

|                             |                             |
|:----------------------------|:----------------------------|
| ![33](/assets/img/02/33.png){: w="250"} | ![34](/assets/img/02/34.png){: w="250"} |
| ![35](/assets/img/02/35.png){: w="250"} | ![36](/assets/img/02/36.png){: w="250"} |

<br>  



