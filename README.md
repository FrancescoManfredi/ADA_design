# APPUNTI
Qui dentro raccogliamo alcuni dettagli di design solo per quanto
riguarda il comportamento di ADA di fronte al pubblico. Per i requisiti
che riguardano il deployment, la configurazione e la gestione di
contenuti di ADA sarà necessario preparare documenti separati.  

A partire dagli use case in UseCases.csv generiamo dei
test case.  
  
Ad ogni use case associamo un certo numero di test case.

Ogni test case deve essere formato da:
- riferimento allo use case (magari proprio il campo UseCase
da UseCases.csv);  
- una piccola porzione della Knowledge Base estratta dal database;  
- una query utente che sia inerente al contenuto della KB fornita
per i test di casi positivi o NON inerente per testare le risposte
"di ripiego";  
  
Avere i test case in questa forma ci permette di eseguirli automaticamente
via API verso ADA e serializzare i risultati.  
La valutazione dei risultati serializzati può essere fatta valutare
automaticamente ad un LLM fornendo la query utente, il comportamento atteso,
la knowledge base e la risposta ottenuta da ADA.

