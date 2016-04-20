Script
=======

File aggiornati con aggiunta di un sistema di ricerca dati.

GENERALITÁ
----------

I file contengono il grafico ad istogramma riguardante la frequenza dei vari parametri dei file "tridasmeasures.csv" e "tridasclass.csv".

All'interno della cartella script si possono trovare numerosi file .html dove sono contenuti i grafici che mostrano la frequenza con cui ogni valore viene ripetuto.
Aprendo il file "home.html" si può accedere ad un menù che semplifica e aiuta la ricerca del grafico desiderato.
Nella pagina home, per esempio, selezionando la voce SourceMonitor si accederà al suo contenuto (di file .csv) e, scegliendo uno dei due, si avrà l'elenco dei vari parametri analizzati. Cliccando sul parametro desiderato si aprirà il relativo grafico.

Come detto in precedenza le varie pagine con i dati sono composte di due parti:

*Il grafico: Analizza la frequenza con cui i vari valori sono ripetuti.
*La barra di ricerca: Inserendo il valore desiderato si aprirà una finestra dove sono visualizzati tutti i nomi dei dati che hanno il valore ricercato.

RICERCA DEI VALORI
------------------

La funzione denominata finder(), presente nel primo script di codice javascript, contiene al suo interno una funzione anonima che serve per prendere i dati dal corrispondente file .csv. Dopo aver fatto ciò la funzione crea una variabile denominata "numb" che prende il valore immesso nella search bar e si crea anche un array vuoto denominato "arri" nel quale, successivamente, verranno inseriti tutti i dati ricercati (teoricamente la parte dell'array può essere saltata e fare direttamente un confronto tra il valore del csv e il valore immesso e se risulta positivo visualizzare. Per completezza abbiamo implementato l'array nel caso potesse servire in un miglioramento del codice futuro).

Una volta ottenuto il dato in input si avrà un confronto tra i valori presenti nel file.csv e il numero inserito, se questo confronto risultasse positivo, il valore viene immesso nell'array tramite .push.

Alla fine della selezione dei valori il programma mostrerà l'array che contiene il nome dei valori ricercati.

GRAFICO
-------

Il grafico, ad istogramma, mostra nell'asse delle ordinate la frequenza dei valori, mentre nell'asse delle ascisse i vari valori.
