---
title: Work Breakdown Structure (WBS)
layout: default
parent: Allegati
nav_order: 7
---

# Work Breakdown Structure (WBS)
{: .no_toc}

## Versioni
{: .no_toc}

- TOC
{:toc}

## Ultima Versione
{: .no_toc}

[![Work Breakdown Structure](/pm/resources/diagrams/wbs.jpg)](https://miro.com/app/board/uXjVM7oEJbI=/?share_link_id=912979534867)
> _**NOTA**_: cliccare sull'immagine per visualizzare il diagramma su _Miro_.

---

## 01-02-2023

[Back to Top](#top) |
[Back to Planning](/pm/2-planning#work-breakdown-structure-wbs)

### Attività
{: .no_toc}

[Download Excel](/pm/resources/tables/tasks-2023-02-01.xlsx){: .btn .btn-green }

### Gerarchia delle Attività
{: .no_toc}

Di seguito, si riporta l'RBS a cui sono state aggiunte le attività (in verde) necessarie a soddisfare i requisiti di 
progetto (in nero).

**Goal**: realizzare un'applicazione web per giocare a scacchi online.

1. `M` **Game Management**: permettere a due giocatori dell'applicazione di
   giocare insieme;
    1. `M` **Game Configuration**: permettere a un giocatore di creare e configurare
       una nuova partita di scacchi;

       {: .text-green-200}
        - **Create Configuration Page**: creare la schermata del _Frontend_ relativa alla
          configurazione di una partita di scacchi, che mostri le opzioni di configurazione di una
          partita e permetta di crearne una nuova;
            - **Mockup Configuration Page**: progettare la schermata del _Frontend_ relativa alla
              configurazione di una partita di scacchi;
            - **Implement Configuration Page**: implementare la schermata del _Frontend_ relativa
              alla configurazione di una partita di scacchi;
            - **Integrate Configuration Page**: integrare la schermata del _Frontend_ relativa alla
              configurazione di una partita di scacchi con l'intero _Frontend_ e _Backend_.
        - **Handle Game Creation**: gestire la creazione di una partita di scacchi nel _Backend_,
          data la sua configurazione;
            - **Model Game Configuration**: nel _Game Service_, modellare il concetto di configurazione di una partita;
            - **Initialize Game**: nel _Game Service_, gestire l'inizializzazione di una partita di scacchi;
            - **Handle Host Connection**: gestire la connessione dell'utente che ha creato la partita
              al _Game Service_.

        1. `M` **Public Game**: permettere a un giocatore di creare una partita pubblica
           di scacchi, a cui chiunque può partecipare;

           {: .text-green-200}
            - **Add Public Game option to Frontend**: aggiungere l'opzione nella Configuration Page;
            - **Add Public Game option to Backend**: aggiungere l'opzione nel _Game Service_.
        2. `S` **Private Game**: permettere a un giocatore di creare una partita privata
           di scacchi, a cui può partecipare solo chi conosce l'identificatore segreto;

           {: .text-green-200}
            - **Add Private Game option to Frontend**: aggiungere l'opzione nella Configuration Page;
            - **Add Private Game option to Backend**: aggiungere l'opzione nel _Game Service_.
        3. `C` **Friend Game**: permettere a un giocatore autenticato di creare una partita
           privata di scacchi invitando un suo specifico amico nell'applicazione a parteciparci;

           {: .text-green-200}
            - **Add Friend Game option to Frontend**: aggiungere l'opzione nella Configuration Page;
            - **Handle Friend Invitation**: nel _Game Service_, gestire l'invio agli amici dell'invito a partecipare a 
              una partita attraverso il _Notification Service_.
        4. `M` **Time Constraint**: permette di configurare i vincoli di tempo della partita;
            1. `M` **No Limit**: nessun vincolo di tempo;

               {: .text-green-200}
                - **Add No Limit option to Frontend**: aggiungere l'opzione nella Configuration Page;
                - **Add No Limit option to Backend**: aggiungere l'opzione nel _Game Service_.

            2. `C` **Turn Limit**: vincolo di tempo sul turno di ciascun giocatore (es.: ogni
               giocatore ha 3 minuti ogni turno per fare la propria mossa);

               {: .text-green-200}
                - **Add Turn Limit option to Frontend**: aggiungere l'opzione nella Configuration Page;
                - **Add Turn Limit option to Backend**: aggiungere l'opzione nel _Game Service_.

            3. `C` **Player Limit**: vincolo di tempo sul controllo della scacchiera di ciascun
               giocatore (es.: ogni giocatore ha 10 minuti in totale per fare le sue mosse
               durante un'intera partita);

               {: .text-green-200}
                - **Add Player Limit option to Frontend**: aggiungere l'opzione nella Configuration Page;
                - **Add Player Limit option to Backend**: aggiungere l'opzione nel _Game Service_.

    2. `M` **Game Participation**: permettere a un giocatore di partecipare a una partita
       di scacchi, già configurata;

       {: .text-green-200}
        - **Create Game Participation Page**: creare la schermata del _Frontend_ relativa alla
          partecipazione a una partita di scacchi, che mostri le diverse modalità per partecipare a
          una partita di scacchi;
            - **Mockup Game Participation Page**: progettare la schermata del _Frontend_ relativa alla
              partecipazione a una partita di scacchi;
            - **Implement Game Participation Page**: implementare la schermata del _Frontend_ relativa
              alla partecipazione a una partita di scacchi;
            - **Integrate Game Participation Page**: integrare la schermata del _Frontend_ relativa alla
              partecipazione a una partita di scacchi con l'intero _Frontend_ e _Backend_.

        1. `M` **Public Game Participation**: permettere a un giocatore di partecipare a una
           partita pubblica qualsiasi;

           {: .text-green-200}
            - **Add Join Public Game to Frontend**: aggiungere l'opzione nella Participation Page;
            - **Handle Public Game Participation**: gestire la connessione di un utente al _Game Service_
              per partecipare a una partita pubblica casuale.
        2. `S` **Private Game Participation**: permettere a un giocatore di partecipare a una
           partita privata di cui conosce l'identificatore segreto;

           {: .text-green-200}
            - **Add Join Private Game to Frontend**: aggiungere l'opzione nella Participation Page;
            - **Handle Private Game Participation**: gestire la connessione di un utente al _Game Service_
              per partecipare a una partita privata di cui ha specificato l'identificatore segreto.
        3. `C` **Friend Game Participation**: permettere a un giocatore autenticato di partecipare
           a una partita privata a cui è stato invitato;

           {: .text-green-200}
            - **Show Friend Game Invitation**: mostrare al giocatore gli inviti alle partite inviati dai suoi amici;
            - **Handle Friend Game Participation**: gestire la connessione di un utente al _Game Service_
              per partecipare a una partita privata a cui è stato invitato.
    3. `M` **Game Execution**: gestione dello svolgimento di una partita tra due giocatori;

       {: .text-green-200}
        - **Create Game Page**: creare la schermata del _Frontend_ relativa allo svolgimento di una
          partita di scacchi, che mostri lo stato della partita in svolgimento e permetta l'interazione
          dell'utente con essa;
            - **Mockup Game Page**: progettare la schermata del _Frontend_ relativa allo svolgimento di
              una partita di scacchi;
            - **Implement Game Page**: implementare la schermata del _Frontend_ relativa
              allo svolgimento di una partita di scacchi;
            - **Integrate Game Page**: integrare la schermata del _Frontend_ relativa allo svolgimento di
              una partita di scacchi con l'intero _Frontend_ e _Backend_.
        - **Reuse previous chess application**: riutilizzare le funzionalità dell'applicazione
          già realizzata dal committente (es.: esecuzione di una partita di scacchi nelle diverse
          configurazioni sui limiti di tempo...);
            - **Analyze previous chess application**: analizzare l'applicazione già realizzata
              dal committente, identificando quali componenti possono essere facilmente riutilizzati;
            - **Integrate previous chess application**: integrare tali componenti con il _Game Service_,
              esponendo le loro funzionalità agli utenti dell'applicazione.
        - **Handle Game Termination**: gestire la terminazione delle partite eseguite dal _Game Service_,
          memorizzando i risultati di ciascun giocatore nello _Statistics Service_;

        1. `M` **Turn Execution**: gestione di un turno della partita;
            1. `M` **Turn Control**: durante il turno di un giocatore, tale giocatore
               deve essere l'unico ad avere il controllo sulla scacchiera;
            2. `M` **Turn Termination**: all'esecuzione di una mossa, il turno termina e
               il controllo è ceduto al giocatore avversario.
        2. `M` **Chessboard Creation**: creazione della scacchiera negli scacchi;
            1. `M` **Rank Creation**: la scacchiera è definita da 8 righe numerate da 1 a
               8, chiamate Rank;
            2. `M` **File Creation**: la scacchiera è definita da 8 colonne identificate
               con le lettere da A a H, chiamate File.
        3. `M` **Piece Creation**: creazione dei pezzi della scacchiera;
            1. `M` **Pawn Creation**: creazione del pedone;
            2. `M` **Knight Creation**: creazione del cavallo;
            3. `M` **Bishop Creation**: creazione dell'alfiere;
            4. `M` **Rook Creation**: creazione della torre;
            5. `M` **Queen Creation**: creazione della regina;
            6. `M` **King Creation**: creazione del re.
        4. `M` **Piece Movement**: movimento dei pezzi sulla scacchiera;
            1. `M` **Movement Constraints**: gestione dei vincoli di movimento;
                1. `M` **Border Constraint**: nessun pezzo può muoversi al di fuori della
                   scacchiera;
                2. `M` **Block Constraint**: nessun pezzo, ad eccezione del cavallo, può
                   muoversi scavalcando gli altri pezzi sulla scacchiera;
                3. `M` **Check Constraint**: nessun pezzo può muoversi se tale mossa pone
                   il giocatore corrente in scacco.
            2. `M` **Pawn Movement**: movimento del pedone sulla scacchiera;
                1. `M` **One Forward**: movimento di una casella in avanti;
                2. `M` **Double Forward**: movimento di due caselle in avanti. Possibile
                   solo alla prima mossa del pedone.
            3. `M` **Knight Movement**: movimento del cavallo sulla scacchiera. Il cavallo
               può effettuare movimenti seguendo una traiettoria ad L;
            4. `M` **Bishop Movement**: movimento dell'alfiere sulla scacchiera. L'alfiere
               può effettuare movimenti in diagonale;
            5. `M` **Rook Movement**: movimento della torre sulla scacchiera. La torre può
               effettuare movimenti in verticale o in orizzontale;
            6. `M` **Queen Movement**: movimento della regina sulla scacchiera. La regina
               può effettuare movimenti in verticale, in orizzontale e in diagonale;
            7. `M` **King Movement**: movimento del re sulla scacchiera;
                1. `M` **One Around**: movimento di una casella in qualsiasi direzione;
                2. `M` **Castling**: movimento di due caselle a sinistra o a destra, verso
                   una delle due torri del giocatore. Quando effettuato, la torre verso
                   cui si è mosso il re si muove fino a scavalcare il re.
                   Effettuabile solo se il re e la torre non hanno eseguito movimenti
                   in precedenza e se non ci sono altri pezzi tra loro due.
        5. `M` **Piece Capture**: gestione della cattura dei pezzi sulla scacchiera;
            1. `M` **Standard Capture**: tutti i pezzi, ad eccezione del pedone, possono
               catturare un pezzo avversario effettuando un movimento su tale pezzo;
            2. `M` **Pawn Capture**: gestione della cattura da parte del pedone;
                1. `M` **Diagonal Capture**: il pedone può catturare un pezzo
                   solo muovendosi di una posizione in avanti in diagonale;
                2. `M` **En Passant**: il pedone può catturare un pedone avversario che,
                   nel turno precedente, gli si è mosso accanto effettuando una mossa
                   doppia. Tale cattura avviene muovendosi dietro il pedone avversario.
        6. `M` **Chessboard Analysis**: riconoscimento dei possibili stati della scacchiera;
            1. `M` **Check**: situazione in cui il re del giocatore corrente può essere
               catturato dal suo avversario nel turno successivo;
            2. `M` **Stale**: situazione in cui il giocatore corrente non ha mosse
               disponibili;
            3. `M` **Checkmate**: situazione in cui il giocatore corrente è sia in scacco
               che in stallo;
            4. `M` **Promotion**: situazione in cui il giocatore corrente ha portato un
               pedone sul lato opposto della scacchiera e può sostituirlo con un
               cavallo, un alfiere, una torre o una regina.
2. `S` **Tournament Management**: permettere di organizzare dei tornei che includono
   più partite tra diversi giocatori autenticati;
    1. `S` **Tournament Configuration**: permettere a un amministratore di creare e
       configurare dei tornei di scacchi (es.: massimo numero di partecipanti,
       numero di round...);

       {: .text-green-200}
        - **Create Tournament Configuration Page**: creare la schermata del _Frontend_ relativa
          alla configurazione di un torneo di scacchi, che mostri le opzioni di configurazione di un
          torneo e permetta di crearne uno nuovo;
            - **Mockup Tournament Configuration Page**: progettare la schermata del _Frontend_ relativa
              alla configurazione di un torneo di scacchi;
            - **Implement Tournament Configuration Page**: implementare la schermata del _Frontend_ relativa
              alla configurazione di un torneo di scacchi;
            - **Integrate Tournament Configuration Page**: integrare la schermata del _Frontend_ relativa
              alla configurazione di un torneo di scacchi con l'intero _Frontend_ e _Backend_.
        - **Handle Tournament Creation**: gestire la creazione di un torneo di scacchi nel _Backend_,
          data la sua configurazione;
            - **Model Tournament Configuration**: nel _Tournament Service_, modellare il concetto di configurazione di
              un torneo;
            - **Initialize Tournament**: nel _Tournament Service_, gestire l'inizializzazione di un torneo di scacchi.
    2. `S` **Tournament Participation**: permettere a un giocatore autenticato di partecipare a un torneo;

       {: .text-green-200}
        - **Create Tournament Participation Page**: creare la schermata del _Frontend_ relativa alla
          partecipazione a un torneo di scacchi, che mostri i tornei a cui il giocatore può partecipare;
            - **Mockup Tournament Participation Page**: progettare la schermata del _Frontend_ relativa alla
              partecipazione a un torneo di scacchi;
            - **Implement Tournament Participation Page**: implementare la schermata del _Frontend_ relativa
              alla partecipazione a un torneo di scacchi;
            - **Integrate Tournament Participation Page**: integrare la schermata del _Frontend_ relativa alla
              partecipazione a un torneo di scacchi con l'intero _Frontend_ e _Backend_.
    3. `S` **Tournament Execution**: gestione dell'esecuzione di un torneo, basandosi
       sul sistema svizzero;

       {: .text-green-200}
        - **Create Tournament Page**: creare la schermata del _Frontend_ relativa all'esecuzione
          di un torneo di scacchi, che mostri lo stato del torneo in svolgimento e permetta l'interazione
          dell'utente con essa;
            - **Mockup Tournament Page**: progettare la schermata del _Frontend_ relativa all'esecuzione
              di un torneo di scacchi;
            - **Implement Tournament Page**: implementare la schermata del _Frontend_ relativa all'esecuzione
              di un torneo di scacchi;
            - **Integrate Tournament Page**: integrare la schermata del _Frontend_ relativa all'esecuzione
              di un torneo di scacchi con l'intero _Frontend_ e _Backend_.

        1. `S` **Round Execution**: gestione di un round del sistema svizzero;
            1. `S` **Participant Pairing**: gestione della formazione delle coppie di
               giocatori autenticati che devono affrontarsi, sulla base dei risultati
               di ciascun giocatore autenticato;

               {: .text-green-200}
                - **Implement Pairing Algorithm**: implementare la funzionalità del _Tournament Service_
                  che, dati i partecipanti al torneo, restituisce le coppie di partecipanti che dovranno
                  sfidarsi, sulla base dei loro risultati nei match precedenti.
            2. `S` **Match Execution**: gestione dell'esecuzione dei match tra le coppie
               di giocatori autenticati che devono affrontarsi;

               {: .text-green-200}
                - **Create Match**: gestire la creazione dei match individuati dal _Tournament Service_
                  attraverso il _Game Service_, che li eseguirà.
            3. `S` **Result Aggregation**: gestione dell'aggregazione dei risultati dei
               match eseguiti nel round corrente;

               {: .text-green-200}
                - **Notify Match Termination**: gestire la terminazione dei match eseguiti dal _Game Service_,
                  notificandone i risultati al _Tournament Service_, che li aggregherà per mostrarli ai partecipanti.

    4. `S` **Tournament Awards**: gestione della premiazione del torneo;

       {: .text-green-200}
        - **Handle Tournament Termination**: gestire la terminazione dei tornei eseguiti dal _Tournament Service_,
          memorizzando i risultati di ciascun giocatore nello _Statistics Service_.
    5. `S` **Tournament Storage**: gestione della memorizzazione dei dati relativi
       ai tornei (es.: numero di partecipanti massimi e correnti...);

       {: .text-green-200}
        - **Install Tournament Database**: installare un database in cui memorizzare i dati relativi ai tornei;
        - **Design Tournament Database**: progettare la struttura dei dati da memorizzare relativi ai tornei;
        - **Implement Tournament Database Queries**: implementare le query per il reperimento o l'aggiornamento
          dei dati relativi ai tornei.
3. `M` **Authentication Management**: permettere a un giocatore ospite di autenticarsi
   all'interno dell'applicazione;
    1. `M` **Sign In**: permettere a un giocatore ospite di registrarsi all'applicazione;
        1. `M` **Registration Form**: gestione dell'inserimento dei dati del giocatore ospite.
           In particolare, sono richiesti la sua email, il suo username e la sua password;

           {: .text-green-200}
            - **Create Registration Page**: creare la schermata del _Frontend_ relativa alla registrazione
              di un giocatore ospite all'applicazione;
                - **Mockup Registration Page**: progettare la schermata del _Frontend_ relativa alla registrazione
                  di un giocatore ospite all'applicazione;
                - **Implement Registration Page**: implementare la schermata del _Frontend_ relativa
                  alla registrazione di un giocatore ospite all'applicazione;
                - **Integrate Registration Page**: integrare la schermata del _Frontend_ relativa alla registrazione
                  di un giocatore ospite all'applicazione con l'intero _Frontend_ e _Backend_.
            - **Handle Registration**: nell'_Authentication Service_, gestire la registrazione di un nuovo utente
              all'applicazione.
        2. `W` **Confirmation Email**: gestione dell'email per ultimare la registrazione del
           giocatore ospite, verificando che l'email da lui specificata sia effettivamente
           di suo possesso;

           {: .text-green-200}
            - **Send Confirmation Email**: nell'_Authentication Service_, inviare una email per ultimare la
              registrazione del giocatore ospite;
            - **Handle Email Verification**: nell'_Authentication Service_, gestire il metodo di verifica dell'email del
              giocatore ospite.
    2. `M` **Log In**: permettere a un giocatore ospite di accedere all'applicazione,
       conoscendo le proprie credenziali;

       {: .text-green-200}
        - **Create Login Page**: creare la schermata del _Frontend_ relativa all'accesso
          di un giocatore ospite all'applicazione;
            - **Mockup Login Page**: progettare la schermata del _Frontend_ relativa all'accesso
              di un giocatore ospite all'applicazione;
            - **Implement Login Page**: implementare la schermata del _Frontend_ relativa
              all'accesso di un giocatore ospite all'applicazione;
            - **Integrate Login Page**: integrare la schermata del _Frontend_ relativa all'accesso
              di un giocatore ospite all'applicazione con l'intero _Frontend_ e _Backend_.

        1. `M` **Token Creation**: creazione di un token utente riferito a una sessione
           attiva di un giocatore autenticato, richiesto per accedere alle operazioni
           sensibili dell'applicazione (es.: cambio della password...);

           {: .text-green-200}
            - **Handle Token Creation**: nell'_Authentication Service_, gestire la creazione di un nuovo token utente.
        2. `M` **Token Expiration**: gestire la scadenza dei token utente, per limitare
           la validità di uno specifico accesso nel tempo;

           {: .text-green-200}
            - **Handle Token Expiration**: nell'_Authentication Service_, gestire la scadenza di un nuovo token utente.
        3. `M` **Authorization Management**: gestire i permessi dell'utente in base al
           suo ruolo nell'applicazione (es.: dipendente dell'azienda, giocatore...);

           {: .text-green-200}
            - **Handle User Permissions**: nell'_Authentication Service_, gestire i permessi dell'utente in base al
              ruolo.

    3. `M` **Log out**: permettere a un giocatore autenticato di disconnettersi
       dall'applicazione;
        
       {: .text-green-200}
        - **Add Logout option to Frontend**: aggiungere l'opzione nella barra di navigazione delle pagine del
          _Frontend_;
    
        1. `M` **Token Revocation**: gestione della revoca ed eliminazione del token
           utente riferito alla sessione attiva del giocatore autenticato appena
           disconnesso;

           {: .text-green-200}
            - **Handle Token Revocation**: nell'_Authentication Service_, gestire la revoca ed eliminazione di un token
              utente.
    4. `M` **Sensitive Data Storage**: gestione dei dati sensibili dei giocatori registrati
       all'applicazione;
        1. `M` **Secure Storage**: gestione della memorizzazione dei dati sensibili su
           una piattaforma sicura. Tra i dati sensibili, sono inclusi l'email del
           giocatore, la sua password e i token utente delle sessioni attive;

           {: .text-green-200}
            - **Install Authentication Database**: installare un database in cui memorizzare i dati sensibili degli
              utenti;
            - **Design Authentication Database**: progettare la struttura dei dati sensibili degli utenti da
              memorizzare;
            - **Implement Authentication Database Queries**: implementare le query per il reperimento o l'aggiornamento
              dei dati sensibili degli utenti.
        2. `M` **Cryptography**: gestione dell'oscuramento dei dati sensibili (es.:
           password degli utenti dell'applicazione...);

           {: .text-green-200}
            - **Encrypt Sensitive Data**: nell'_Authentication Service_, criptare i dati sensibili degli utenti durante
              l'inserimento dei dati nel database.
4. `M` **Profile Management**: permettere a un giocatore autenticato di gestire il proprio
   profilo utente;

    {: .text-green-200}
    - **Create Profile Page**: creare la schermata del _Frontend_ relativa al profilo
      di un giocatore autenticato all'applicazione, che permetta di visualizzare e aggiornare
      le informazioni relative al suo account;
        - **Mockup Profile Page**: progettare la schermata del _Frontend_ relativa al profilo
          di un giocatore autenticato all'applicazione;
        - **Implement Profile Page**: implementare la schermata del _Frontend_ relativa al profilo
          di un giocatore autenticato all'applicazione;
        - **Integrate Profile Page**: integrare la schermata del _Frontend_ relativa al profilo
          di un giocatore autenticato all'applicazione con l'intero _Frontend_ e _Backend_.

    1. `M` **Profile Visualization**: permettere a un giocatore autenticato di visualizzare
       il proprio profilo utente, ovvero le informazioni relative al proprio account
       (es.: email, username...);

       {: .text-green-200}
        - **Get User Profile Information**: nell'_Authentication Service_, gestire il reperimento delle informazioni
          relative a un giocatore autenticato.
    2. `M` **Profile Update**: permettere a un giocatore autenticato di aggiornare le
       informazioni relative al proprio account (es.: email, password...);

       {: .text-green-200}
        - **Update User Profile Information**: nell'_Authentication Service_, gestire l'aggiornamento delle informazioni
          relative a un giocatore autenticato.
5. `C` **Socialization Management**: permettere ai giocatori di interagire e socializzare tra di loro;
    1. `C` **Friend Management**: gestione delle amicizie all'interno dell'applicazione;

       {: .text-green-200}
        - **Create Friend Page**: creare la schermata del _Frontend_ relativa agli amici
          di un giocatore autenticato all'applicazione, che permetta di visualizzare i suoi amici, inviare
          o accettare richieste di amicizia e di rimuovere degli amici;
            - **Mockup Friend Page**: progettare la schermata del _Frontend_ relativa agli amici
              di un giocatore autenticato all'applicazione;
            - **Implement Friend Page**: implementare la schermata del _Frontend_ relativa agli amici
              di un giocatore autenticato all'applicazione;
            - **Integrate Friend Page**: integrare la schermata del _Frontend_ relativa agli amici
              di un giocatore autenticato all'applicazione con l'intero _Frontend_ e _Backend_. 

        1. `C` **Friend Request**: permettere a due giocatori autenticati di stringere amicizia;

           {: .text-green-200}
            - **Handle Friend Request Forwarding**: nel _Friend Service_, gestire l'inoltro di una richiesta di amicizia
              verso un giocatore registrato all'applicazione;

            1. `C` **Send Request**: permettere a un giocatore autenticato di inviare una richiesta
               di amicizia a un altro giocatore registrato all'applicazione;
                1. `W` **In-Game Request**: permettere a un giocatore autenticato di inviare una richiesta
                   di amicizia al giocatore autenticato avversario durante una partita;

                   {: .text-green-200}
                    - **Add In-Game Friend Request option to Frontend**: aggiungere l'opzione nella
                      Game Page.
                2. `C` **Request By Username**: permettere a un giocatore autenticato di inviare una richiesta
                   di amicizia a un altro giocatore registrato all'applicazione, conoscendone lo username;

                   {: .text-green-200}
                    - **Add Friend Request By Username option to Frontend**: aggiungere l'opzione nella Friend Page.
            2. `C` **Receive Request**: permettere a un giocatore autenticato di accettare o rifiutare una
               richiesta di amicizia ricevuta da un altro giocatore registrato all'applicazione;
                1. `C` **Request Visualization**: permettere a un giocatore autenticato di visualizzare
                   le richieste di amicizia ricevute dagli altri giocatori registrati all'applicazione;

                   {: .text-green-200}
                    - **Get Friend Requests**: nel _Friend Service_, gestire il reperimento delle richieste di amicizia
                      ricevute da un giocatore autenticato.
                2. `W` **Request Notification**: gestione della notifica a un giocatore autenticato della
                   ricezione di una nuova richiesta di amicizia;

                   {: .text-green-200}
                    - **Handle Friend Request Notification**: nel _Friend Service_, gestire la notifica a un giocatore
                      autenticato della ricezione di una nuova richiesta di amicizia tramite il _Notification Service_.
                3. `C` **Accept Request**: permettere a un giocatore autenticato di accettare una richiesta di
                   amicizia inviata da un altro giocatore;

                   {: .text-green-200}
                    - **Handle Accept Friend Request**: nel _Friend Service_, gestire l'accettazione di una richiesta di
                      amicizia tra due giocatori registrati all'applicazione.
                4. `C` **Reject Request**: permettere a un giocatore autenticato di rifiutare una richiesta di
                   amicizia inviata da un altro giocatore;

                   {: .text-green-200}
                    - **Handle Reject Friend Request**: nel _Friend Service_, gestire il rifiuto di una richiesta di
                      amicizia tra due giocatori registrati all'applicazione.

        2. `C` **Friend Visualization**: permettere a un giocatore autenticato di visualizzare se i propri
           amici sono offline, online o all'interno di una partita;

           {: .text-green-200}
            - **Get Friends**: nel _Friend Service_, gestire il reperimento delle amicizie di un giocatore
              autenticato.
        3. `C` **Friend Removal**: permettere a un giocatore autenticato di rimuovere un altro giocatore dalla
           lista dei suoi amici;

           {: .text-green-200}
            - **Handle Friend Removal**: nel _Friend Service_, gestire la rimozione di un'amicizia dalla
              lista degli amici di un giocatore autenticato.
        4. `C` **Friend Storage**: gestione della memorizzazione degli amici dei giocatori
           e del loro stato;

           {: .text-green-200}
            - **Install Friend Database**: installare un database in cui memorizzare i dati relativi alle amicizie
              dei giocatori autenticati all'applicazione;
            - **Design Friend Database**: progettare la struttura dei dati da memorizzare relativi alle amicizie
              dei giocatori autenticati all'applicazione;
            - **Implement Friend Database Queries**: implementare le query per il reperimento o l'aggiornamento
              dei dati relativi alle amicizie dei giocatori autenticati all'applicazione.
    2. `C` **Communication Management**: permettere ai giocatori di comunicare tra di loro;
        1. `C` **Chat**: permettere ai giocatori di scambiarsi dei messaggi testuali tra di loro;
            1. `W` **In-Game Chat**: permettere a un giocatore di scambiare dei messaggi testuali con il
               proprio avversario durante una partita;
                1. `W` **Send Message**: permettere a un giocatore di inviare messaggi testuali al proprio
                   avversario durante una partita;

                   {: .text-green-200}
                    - **Handle In-Game Message Sending**: nel _Game Service_, gestire l'invio di messaggi non
                      persistenti
                      durante una partita di scacchi.
                2. `W` **Receive Message**: permettere a un giocatore di ricevere messaggi testuali provenienti
                   dal proprio avversario durante una partita;

                   {: .text-green-200}
                    - **Handle In-Game Message Receiving**: nel _Game Service_, gestire la ricezione di messaggi
                      non persistenti durante una partita di scacchi.
                3. `W` **Message Visualization**: permettere a un giocatore di visualizzare i messaggi testuali
                   scambiati con il proprio avversario durante una partita;

                   {: .text-green-200}
                    - **Get In-Game Messages**: nel _Game Service_, gestire il reperimento dei messaggi testuali
                      non persistenti scambiati tra i giocatori durante la partita;
                    - **Show In-Game Messages**: nella Game Page, mostrare i messaggi testuali non persistenti scambiati
                      tra i giocatori durante la partita;
                4. `W` **Message Notification**: gestione della notifica a un giocatore della ricezione di un
                   messaggio dell'avversario durante una partita;

                   {: .text-green-200}
                    - **Handle In-Game Message Notification**: nel _Game Service_, gestire la notifica a un giocatore
                      della ricezione di un nuovo messaggio non persistente durante la partita tramite il
                      _Notification Service_.
            2. `C` **Friend Chat**: permettere a un giocatore autenticato di scambiare dei messaggi testuali con
               un suo amico;

               {: .text-green-200}
                - **Show Friend Chats**: nella barra di navigazione delle pagine del _Frontend_, permettere a un
                  giocatore autenticato di accedere alle conversazioni svolte con i suoi amici;

                1. `C` **Send Message**: permettere a un giocatore autenticato di inviare messaggi testuali a un
                   suo amico;

                   {: .text-green-200}
                    - **Handle Message Sending**: nel _Message Service_, gestire l'invio di messaggi persistenti agli
                      amici di un giocatore.
                2. `C` **Receive Message**: permettere a un giocatore registrato di ricevere messaggi testuali
                   provenienti da un suo amico;

                   {: .text-green-200}
                    - **Handle Message Receiving**: nel _Message Service_, gestire la ricezione di messaggi persistenti
                      dei propri amici.
                3. `C` **Message Visualization**: permettere a un giocatore autenticato di visualizzare i messaggi
                   testuali scambiati con un suo amico;

                   {: .text-green-200}
                    - **Get Messages**: nel _Message Service_, gestire il reperimento dei messaggi persistenti scambiati
                      tra due giocatori registrati all'applicazione;
                    - **Show Messages**: nelle pagine del _Frontend_, quando un giocatore autenticato accede a una
                      conversazione svolta con uno dei suoi amici, mostrare i messaggi persistenti scambiati tra di loro
                      in quella conversazione.
                4. `C` **Message Forwarding**: gestione dell'inoltro di un messaggio da un giocatore autenticato
                   a un suo amico;

                   {: .text-green-200}
                    - **Handle Message Forwarding**: nel _Message Service_, gestire l'inoltro di un messaggio
                      persistente da un giocatore autenticato a un suo amico, verificando prima la loro effettiva
                      amicizia tramite il _Friend Service_.
                5. `W` **Message Notification**: gestione della notifica a un giocatore autenticato della ricezione
                   di un messaggio di uno dei suoi amici;

                   {: .text-green-200}
                    - **Handle Message Notification**: nel _Message Service_, gestire la notifica a un giocatore
                      della ricezione di un nuovo messaggio persistente tramite il _Notification Service_.
                6. `C` **Friend Chat Storage**: gestione della memorizzazione dei messaggi scambiati tra ogni
                   giocatore registrato e i suoi amici;

                   {: .text-green-200}
                    - **Install Chat Database**: installare un database in cui memorizzare i dati relativi alle
                      conversazioni scambiate tra i giocatori registrati all'applicazione;
                    - **Design Chat Database**: progettare la struttura dei dati da memorizzare relativi alle
                      conversazioni scambiate tra i giocatori registrati all'applicazione;
                    - **Implement Chat Database Queries**: implementare le query per il reperimento o l'aggiornamento
                      dei dati relativi alle conversazioni scambiate tra i giocatori registrati all'applicazione.
6. `C` **Statistics Management**: permettere a un giocatore di monitorare le statistiche di
   un giocatore registrato all'applicazione, tra cui le proprie statistiche;

   {: .text-green-200}
    - **Create Statistics Page**: creare la schermata del _Frontend_ relativa alle statistiche di un
      giocatore registrato all'applicazione, che permetta di visualizzarne il punteggio ELO e i risultati
      dei tornei a cui ha partecipato;
        - **Mockup Statistics Page**: progettare la schermata del _Frontend_ relativa alle statistiche di un
          giocatore registrato all'applicazione;
        - **Implement Statistics Page**: implementare la schermata del _Frontend_ relativa alle statistiche di un
          giocatore registrato all'applicazione;
        - **Integrate Statistics Page**: integrare la schermata del _Frontend_ relativa alle statistiche di un
          giocatore registrato all'applicazione con l'intero _Frontend_ e _Backend_.
    - **Install Statistics Database**: installare un database in cui memorizzare i dati relativi allo storico dei
      punteggi e ai risultati ai tornei dei giocatori registrati all'applicazione;
    - **Design Statistics Database**: progettare la struttura dei dati da memorizzare relativi allo storico dei
      punteggi e ai risultati ai tornei dei giocatori registrati all'applicazione;

    1. `C` **Score Visualization**: permettere a un giocatore di visualizzare il punteggio ELO
       di un giocatore registrato all'applicazione;

       {: .text-green-200}
        - **Get Score**: nello _Statistics Service_, gestire il reperimento del punteggio ELO di un giocatore registrato
          all'applicazione;

        1. `C` **Score Evaluation**: gestione della valutazione del punteggio di
           un giocatore autenticato al termine di ogni partita;

           {: .text-green-200}
            - **Handle Score Evaluation**: nel _Game Service_, al termine di una partita, gestire l'invio dei risultati
              dei giocatori allo _Statistics Service_, che ne aggiornerà il punteggio ELO di conseguenza.
        2. `C` **Score Storage**: gestione della memorizzazione dello storico dei
           punteggi di ciascun giocatore registrato all'applicazione;

           {: .text-green-200}
            - **Implement Score Database Queries**: implementare le query per il reperimento o l'aggiornamento
              dei dati relativi allo storico dei punteggi dei giocatori registrati all'applicazione.
        3. `W` **Score History Visualization**: permettere a un giocatore di visualizzare come è cambiato
           nel tempo il punteggio ELO di un giocatore registrato all'applicazione;

           {: .text-green-200}
            - **Get Score History**: nello _Statistics Service_, gestire il reperimento dello storico dei punteggi di
              un giocatore registrato all'applicazione.
    2. `C` **Tournament Visualization**: permettere a un giocatore di visualizzare i risultati ottenuti
       nei tornei a cui ha partecipato un giocatore registrato all'applicazione;
        1. `C` **Tournament Storage**: gestire la memorizzazione dei risultati di ogni torneo
           dei giocatori registrati all'applicazione;

           {: .text-green-200}
            - **Implement Tournament Result Database Queries**: implementare le query per il reperimento o
              l'aggiornamento dei dati relativi ai risultati dei tornei dei giocatori registrati all'applicazione.
    3. `C` **Leaderboard Visualization**: permettere a un giocatore di visualizzare la classifica globale
       dei giocatori registrati all'applicazione;
        1. `C` **Rank Visualization**: permettere a un giocatore autenticato di visualizzare la propria
           posizione nella classifica globale;

           {: .text-green-200}
            - **Create Leaderboard Page**: creare la schermata del _Frontend_ relativa alla classifica globale dei
              giocatori registrati all'applicazione, che permetta di visualizzare la posizione in classifica dei
              giocatori dell'applicazione e accedere alle loro statistiche;
                - **Mockup Leaderboard Page**: progettare la schermata del _Frontend_ relativa alla classifica globale
                  dei giocatori registrati all'applicazione;
                - **Implement Leaderboard Page**: implementare la schermata del _Frontend_ relativa alla classifica
                  globale dei giocatori registrati all'applicazione;
                - **Integrate Leaderboard Page**: integrare la schermata del _Frontend_ relativa alla classifica globale
                  dei giocatori registrati all'applicazione con l'intero _Frontend_ e _Backend_.
            - **Get Ranks**: nello _Statistics Service_, gestire il reperimento delle posizioni dei giocatori nella
              classifica globale dell'applicazione.
7. `M` **Notification Management**: gestione delle notifiche in tempo reale dell'applicazione;
    1. `M` **Notification Forwarding**: gestione della notifica in tempo reale ai
       giocatori autenticati degli eventi che li coinvolgono;

       {: .text-green-200}
        - **Handle Notification Forwarding**: nel _Notification Service_, gestire la ricezione e l'invio delle
          notifiche ai giocatori autenticati nell'applicazione.
    2. `M` **Notification Storage**: gestione della memorizzazione delle notifiche
       relative ai giocatori registrati all'applicazione;

       {: .text-green-200}
        - **Install Notification Database**: installare un database in cui memorizzare i dati relativi alle
          notifiche per i giocatori registrati all'applicazione;
        - **Design Notification Database**: progettare la struttura dei dati da memorizzare relativi alle
          notifiche per i giocatori registrati all'applicazione;
        - **Implement Notification Database Queries**: implementare le query per il reperimento o l'aggiornamento
          dei dati relativi alle notifiche per i giocatori registrati all'applicazione.
8. `M` **Sponsor Management**: gestione della pubblicità agli sponsor dell'applicazione
   (es.: banner, video...);

   {: .text-green-200}
    - **Identify Off-The-Shelf Advertisement Solutions**: individuare possibili soluzioni già in commercio per la
      sponsorizzazione di altre aziende sulla propria applicazione;
    - **Integrate Advertisement Solution**: integrare la soluzione acquisita nel _Frontend_ dell'applicazione.

{: .text-green-200}
- **Integrate Services**: integrare i servizi dell'applicazione tra di loro, risolvendo eventuali conflitti;
- **Test System**: collaudo del sistema in un ambiente apposito alla sua verifica;
- **Deploy System**: installazione del sistema nell'ambiente di produzione.

---

[Back to Top](#top) |
[Previous Version](#01-02-2023)