# Algebra dei Numeri Complessi

## Definizione di Numero

Il concetto di **Numero** è un concetto astratto.
Nasce dalla necessità di contare elementi dello stesso tipo, cioè dotati di almeno una caratteristica (un attributo) comune, ovvero di assegnare una valutazione non opinabile sulla quantità di elementi che costituiscono un **Insieme**.

> **Nota:**
> definiamo **Insieme** una collezione di oggetti ben definiti.
> Non siamo in grado, nella Teoria Assiomatica Moderna, di dare una definizione più rigorosa: è una nozione primitiva come quella di Punto, che non può essere ulteriormente perfezionata.
> Nel nostro caso un Insieme raggruppa tutti gli elementi dotati di una o più caratteristiche comuni.
> Ad esempio: indichiamo con: ''Insieme_degli_uomini_alti'' tutte le persone più alte di 1.80 m.

In realtà, a pensarci bene, la definizione di Numero non è una domanda di Matematica, ma di Filosofia della Matematica.
E su questo punto non esiste una risposta veramente soddisfacente.
Infatti la Matematica si occupa delle proprietà degli oggetti, piuttosto che della loro definizione.

La definizione di Numero che più si avvicina alle nostre aspettative, quella più corretta, è quella data da Von Neumann, che usa i principi della Teoria Assiomatica degli Insiemi, nel modello che riguarda la costruzione dei Numeri Naturali.

Nel modello di Von Neumann, ogni Numero Naturale è l'insieme di tutti i numeri naturali che lo precedono.
Possiamo visualizzare questa affermazione nei termini seguenti, in cui tra le parentesi graffe sono riportati appunto gli elementi che costituiscono il numero:

```text
0 = ∅
1 = {0}
2 = {0,1}
3 = {0,1,2}
```

Un elemento: 0, per il numero 1; 2 elementi: 0,1 per il numero 2; 3 elementi: 0,1,2 per il numero 3, ...

Possiamo costruire una formula generale, indicando con **n** un qualsiasi Numero Naturale:

```text
n = {0,1,2,...,n-1}
```

E fare alcune osservazioni:

* per dare consistenza al nostro modello abbiamo introdotto un nuovo tipo d'insieme: l'insieme vuoto, indicato con 0 = *∅*. L'insieme vuoto è, per definizione, un Numero Naturale.
* se vogliamo passare all'Intero successivo - che esiste sempre - che potremo indicare con **n[+1]** (il successore di n) adotteremo la definizione di **n** a cui aggiungeremo il numero, l'elemento *{n}*, cioè:

 ```text
    n[+1] = n U {n}
    n = {0,1,2,...,n-1}

    E, infatti:
    n[+1] = n U {n} = {0,1,2,...,n-1} U {n} = {0,1,2,...,n-1,n} 
```

> **Nota:**
Significato del simbolo U: il simbolo U si legge "unione".
L'unione di due insiemi è l'insieme che contiene tutti gli elementi presenti nel primo insieme, nel secondo insieme o in entrambi.
Ad esempio: {0,1,2} U {1,2,3} dà come risultato {0,1,2,3} e comprende tutti gli elementi del primo insieme che si trovano anche nel secondo, quelli del primo insieme che non si trovano nel secondo e quelli del secondo che non si trovano nel primo.

* nella definizione di Numero Naturale vale sempre questa relazione:
  
 ```text
0 ⊂ 1 ⊂ 2 ⊂ 3 ⊂ ... ⊂ n-1 ⊂ n
```

che ci dice che ogni numero 'contiene' i suoi predecessori, cioè se **n** è il numero che stiamo osservando, n conterrà n[-1], n[-2], ... n[-(n-1)], n[-n].

> **Nota:**
Significato del simbolo ⊂ : il simbolo ⊂ si legge "è contenuto in".
Ad esempio: {1,2} ⊂ {1,2,3}, perché tutti gli elementi del primo insieme si trovano anche nel secondo.

Per arrivare alla seguente conclusione:

* Ogni Numero Naturale coincide con il suo simbolo (3, ad esempio, è indicato dal simbolo "3") e esattamente allo stesso modo con l'Insieme che lo individua: 3 = {0,1,2}.
In particolare, Numero e Cardinalità dell'insieme coincidono.

> **Nota:**
Cardinalità di un insieme: la cardinalità di un insieme è il numero dei suoi elementi. Se A è l'insieme, la sua cardinalità si indica con: |A| e rappresenta quanti elementi siano contenuti nell'insieme.

Pensare che Numero ed Insieme possano essere visti come facce diverse della stessa medaglia, permette di applicare le operazioni della Teoria degli Insiemi ad ogni Numero Naturale - Somma, Sottrazione, ... - operando così in modo giustificato su di essi.
E' osservazione molto potente, perché mostra come sia possibile costruire l'aritmetica partendo esclusivamente dagli insiemi.

Con questa ipotesi possiamo dire che nella Teoria degli Insiemi sia possibile definire Interi per induzione [cioè ragionando per ricorrenza], costruendo esplicitamente una sequenza di insiemi dall'Insieme vuoto.

Possiamo esplicitare quanto detto nel modo seguente:

```text
0 = ∅
1 = {0} = {∅}
2 = {0,1} = {0, {∅}} = {∅, {∅}}
3 = {0,1,2} = {∅, {∅}, {∅, {∅}} } 
```

mettendo in luce il concetto di ricorrenza.Il numero naturale non serve solo a contare gli elementi di un insieme: nella costruzione di Von Neumann esso è l'insieme stesso.
