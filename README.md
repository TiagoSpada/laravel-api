## giorno 1 consegna:

Ciao ragazzi,
creiamo con Laravel il nostro sistema di gestione del nostro Portfolio di progetti.
Oggi iniziamo un nuovo progetto che si arricchirà nel corso delle prossime lezioni: man mano aggiungeremo funzionalità e vedremo la nostra applicazione crescere ed evolvere.
Nel pomeriggio, rifate ciò che abbiamo visto insieme stamattina stilando tutto a vostro piacere utilizzando SASS.
Descrizione:
Ripercorriamo gli steps fatti a lezione ed iniziamo un nuovo progetto usando laravel breeze per utilizzare il sistema di autenticazione.
Trovate sulla mia repo github il progetto con tutte le indicazioni per creare un vostro template, partendo da un progetto laravel 10 pulito:
Seguite le istruzioni del README:
https://github.com/taniot/laravel-auth-classe126
Iniziamo con il definire il layout, modello, migrazione, controller e rotte necessarie per il sistema portfolio:

1. Autenticazione: si parte con l'autenticazione e la creazione di un layout per back-office
2. Creazione del modello Project con relativa migrazione, seeder, controller e rotte
   _Bonus_
   Per la parte di back-office creiamo un resource controller Admin\ProjectController per gestire tutte le operazioni CRUD dei progetti
   Implementiamo la validazione dei dati dei Progetti nelle operazioni CRUD che lo richiedono usando due form requests.

## giorno 2 consegna:

Ciao ragazzi,
continuate con l'esercitazione cominciata ieri - stessa repository e portate a conclusione le CRUD per la gestione dei progetti.
nome repo: laravel-auth
Bonus:
provate a modificare il comportamento di default di laravel creando un campo SLUG per ogni progetto e riferendovi a quello per le operazioni di EDIT, SHOW, CREATE, DELETE;
create una versione pubblica dei vostri progetti creando un controller Guest\ProjectController
Buon lavoro e buon weekend!

## giorno 3 consegna (relazione one-to-many):

Ciao ragazzi,
Esercizio di oggi: Laravel Boolfolio - Project Typology
nome repo: laravel-one-to-many
Continuiamo a lavorare sul codice dei giorni scorsi, ma in una nuova repo e aggiungiamo una nuova entità Type. Questa entità rappresenta la tipologia di progetto ed è in relazione one to many con i progetti.
I task da svolgere sono diversi, ma alcuni di essi sono un ripasso di ciò che abbiamo fatto nelle lezioni dei giorni scorsi:

-   [x] creare la migration per la tabella types
-   [x] creare il model Type
-   [x] creare la migration di modifica per la tabella projects per aggiungere la chiave esterna
-   [x] aggiungere ai model Type e Project i metodi per definire la relazione one to many
-   [x] visualizzare nella pagina di dettaglio di un progetto la tipologia associata, se presente
-   [x] permettere all’utente di associare una tipologia nella pagina di creazione e modifica di un progetto
-   [x] gestire il salvataggio dell’associazione progetto-tipologia con opportune regole di validazione
-   Bonus 1:
-   -   [] creare il seeder per il model Type.
-   Bonus 2:
-   -   [] aggiungere le operazioni CRUD per il model Type, in modo da gestire le tipologie di progetto direttamente dal pannello di amministrazione.
-   -   [] Buon lavoro e buon divertimento!

## relazione many to many (giorno 1)

Ciao ragazzi,
Esercizio di oggi: Laravel Boolfolio - Project Technology
nome repo: laravel-many-to-many
Continuiamo a lavorare sul codice dei giorni scorsi, ma in una nuova repo e aggiungiamo una nuova entità Technology.
Questa entità rappresenta le tecnologie utilizzate ed è in relazione many to many con i progetti.
I task da svolgere sono diversi, ma alcuni di essi sono un ripasso di ciò che abbiamo fatto nelle lezioni dei giorni scorsi:

-   [x] creare la migration per la tabella technologies
-   [x] creare il model Technology
-   [x] creare la migration per la tabella pivot project_technology
-   [x] aggiungere ai model Technology e Project i metodi per definire la relazione many to many
-   [x] visualizzare nella pagina di dettaglio di un progetto le tecnologie utilizzate, se presenti
-   Bonus 1:
-   -   [x] creare il seeder per il model Technology.
-   Bonus 2:
-   -   [] aggiungere le operazioni CRUD per il model Technology, in modo da gestire le tecnologie utilizzate nei progetti direttamente dal pannello di amministrazione.
-   -   [] Buon lavoro e buon divertimento!

## relazione many to many (giorno 2)

Ciao ragazzi,
Esercizio di oggi: Laravel Boolfolio - Project Technology
nome repo: laravel-many-to-many
Continuiamo a lavorare sul codice di ieri, stessa repo.
I task sono:

-   [x] permettere all’utente di associare le tecnologie nella pagina di creazione e modifica di un progetto
-   [x] gestire il salvataggio dell’associazione progetto-tecnologie con opportune regole di validazione
-   [x] eliminare opportunamente le relazioni alla cancellazione del progetto/technology

Buon lavoro e buon divertimento!
A lunedì!

# INIZIO LAVORO Laravel Boolfolio - API

## Giorno 1

Ciao ragazzi,
continuiamo a lavorare sul codice dei giorni scorsi, ma in una nuova repo.
L’esercizio di oggi è suddiviso in milestone ed è importante che ne seguiate l’ordine.

### Milestone 1

-   [x] nome repo 1: laravel-api
-   [x] Aggiungiamo al nostro progetto Laravel una nuovo Api/ProjectController. Questo controller risponderà a delle richieste via API e si occuperà di restituire la lista dei progetti presenti nel database in formato json.

### Milestone 2

-   [x] Testiamo la chiamata API tramite Postman e assicuriamoci di ricevere i dati correttamente.

### Milestone 3

-   [x] nome repo 2: vite-boolfolio
-   [x] Iniziamo ad occuparci della parte front-office della nostra applicazione: creiamo un nuovo progetto Vue 3 con Vite e installiamo axios.
-   [x] Colleghiamo questo progetto ad una repo separata.

### Milestone 4

-   [x] Nel componente principale della nostra Vue App facciamo una chiamata API all’endpoint costruito nel progetto Laravel (milestone 1) e recuperiamo tutti i progetti dal nostro back-end.
-   [x] Stampiamo in console i risultati e verifichiamo di ricevere i dati correttamente.

### Milestone 5

-   Creiamo un nuovo componente ProjectCard, che corrisponde ad una card per visualizzare un progetto. Utilizziamo questo componente per visualizzare tutti i progetti ricevuti tramite API.

### Bonus:

-   Gestire la paginazione dei risultati
    Buon lavoro e buon divertimento!

## giorno 2

Ciao ragazzi,
continuate l'esercitazione iniziata ieri stesse repo.
frontend: vite-boolfolio
backend: laravel-api
:avviso: Se non l'avete ancora fatto, aprite le repo oggi stesso.

### Ecco i task da completare:

-   aggiungere una pagina di dettaglio di progetto (frontend)
-   aggiungere sistema di paginazione (frontend)
    La pagina di dettaglio dovrà avere tutte le informazioni del progetto e le informazioni relazionate.

### Vi lascio inoltre qualche bonus:

-   Aggiungere campi e sistema di filtro sul backend (in draft, in evidenza)
-   Aggiungere sistema di filtro sul frontend (in evidenza), mostrando i relativi progetti in homepage
-   Aggiungere un campo di ricerca per titolo (frontend / backend)
-   Creazione di un nuovo progetto da frontend (base)
-   Creazione di un nuovo progetto da frontend con caricamento immagine.
    Ci rivediamo il 26 agosto!
    Buone vacanze!
