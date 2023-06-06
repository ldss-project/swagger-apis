# Requirement Breakdown Structure

---
Data: 15-01-2023

**Goal**: realizzare un'applicazione web per giocare a scacchi online.

1. **Game Management**: permettere a due giocatori dell'applicazione di
   giocare insieme.
   1. **Game Configuration**: permettere a un giocatore di creare e configurare
      una nuova partita di scacchi.
      1. **Public Game**: permettere a un giocatore di creare una partita pubblica
         di scacchi, a cui chiunque può partecipare.
      2. **Private Game**: permettere a un giocatore di creare una partita privata
         di scacchi, a cui solo chi conosce l'id segreto può partecipare.
      3. **Friend Game**: permettere a un giocatore autenticato di creare una partita 
         privata di scacchi invitando un suo specifico amico nell'applicazione a parteciparci.
      4. **Time Constraint**: permette di configurare i vincoli di tempo della partita.
         1. **No Limit**: nessun vincolo di tempo.
         2. **Turn Limit**: vincolo di tempo sul turno di ciascun giocatore (es.: ogni
            giocatore ha 3 minuti ogni turno per fare la propria mossa).
         3. **Player Limit**: vincolo di tempo sul controllo della scacchiera di ciascun
            giocatore (es.: ogni giocatore ha 10 minuti in totale per fare le sue mosse 
            durante un'intera partita).
   2. **Game Participation**: permettere a un giocatore di partecipare a una partita
      di scacchi, già configurata.
      1. **Public Game Participation**: permettere a un giocatore di partecipare a una
         partita pubblica qualsiasi.
      2. **Private Game Participation**: permettere a un giocatore di partecipare a una
         partita privata di cui conosce l'id segreto.
      3. **Friend Game Participation**: permettere a un giocatore autenticato di partecipare
         a una partita privata a cui è stato invitato.
   3. **Game Execution**: gestione dello svolgimento di una partita tra due giocatori.
      1. **Turn Execution**: gestione di un turno della partita.
         1. **Turn Control**: durante il turno di un giocatore, tale giocatore
            deve essere l'unico ad avere il controllo sulla scacchiera.
         2. **Turn Termination**: all'esecuzione di una mossa, il turno termina e
            il controllo è ceduto al giocatore avversario.
      2. **Chessboard Creation**: creazione della scacchiera negli scacchi.
         1. **Rank Creation**: la scacchiera è definita da 8 righe numerate da 1 a 
            8, chiamate Rank.
         2. **File Creation**: la scacchiera è definita da 8 colonne identificate
            con le lettere da A a H, chiamate File.
      3. **Piece Creation**: creazione dei pezzi della scacchiera.
         1. **Pawn Creation**: creazione del pedone.
         2. **Knight Creation**: creazione del cavallo.
         3. **Bishop Creation**: creazione dell'alfiere.
         4. **Rook Creation**: creazione della torre.
         5. **Queen Creation**: creazione della regina.
         6. **King Creation**: creazione del re.
      4. **Piece Movement**: movimento dei pezzi sulla scacchiera. 
         1. **Movement Constraints**: gestione dei vincoli di movimento.
            1. **Border Constraint**: nessun pezzo può muoversi al di fuori della
            scacchiera.
            2. **Block Constraint**: nessun pezzo, ad eccezione del cavallo, può
               muoversi scavalcando gli altri pezzi sulla scacchiera.
            3. **Check Constraint**: nessun pezzo può muoversi se tale mossa pone
               il giocatore corrente in scacco.
         2. **Pawn Movement**: movimento del pedone sulla scacchiera.
            1. **One Forward**: movimento di una casella in avanti.
            2. **Double Forward**: movimento di due caselle in avanti. Possibile
               solo alla prima mossa del pedone.
         3. **Knight Movement**: movimento del cavallo sulla scacchiera. Il cavallo
            può effettuare movimenti seguendo una traiettoria ad L.
         4. **Bishop Movement**: movimento dell'alfiere sulla scacchiera. L'alfiere
            può effettuare movimenti in diagonale.
         5. **Rook Movement**: movimento della torre sulla scacchiera. La torre può
            effettuare movimenti in verticale o in orizzontale.
         6. **Queen Movement**: movimento della regina sulla scacchiera. La regina
            può effettuare movimenti in verticale, in orizzontale e in diagonale.
         7. **King Movement**: movimento del re sulla scacchiera.
            1. **One Around**: movimento di una casella in qualsiasi direzione.
            2. **Castling**: movimento di due caselle a sinistra o a destra, verso
               una delle due torri del giocatore. Quando effettuato, la torre verso
               cui si è mosso il re si muove fino a scavalcare il re.
               Effettuabile solo se il re e la torre non hanno eseguito movimenti 
               in precedenza e se non ci sono altri pezzi tra loro due.
      5. **Piece Capture**: gestione della cattura dei pezzi sulla scacchiera.
         1. **Standard Capture**: tutti i pezzi, ad eccezione del pedone, possono
            catturare un pezzo avversario effettuando un movimento su tale pezzo.
         2. **Pawn Capture**: gestione della cattura da parte del pedone.
            1. **Diagonal Capture**: il pedone può catturare solo un pezzo 
               muovendosi di una posizione in avanti in diagonale.
            2. **En Passant**: il pedone può catturare un pedone avversario che, 
               nel turno precedente, gli si è mosso accanto effettuando una mossa
               doppia. Tale cattura avviene muovendosi dietro il pedone avversario.
      6. **Chessboard Analysis**: riconoscimento dei possibili stati della scacchiera.
         1. **Check**: situazione in cui il re del giocatore corrente può essere
            catturato dal suo avversario nel turno successivo.
         2. **Stale**: situazione in cui il giocatore corrente non ha mosse 
            disponibili.
         3. **Checkmate**: situazione in cui il giocatore corrente è sia in scacco
            che in stallo.
         4. **Promotion**: situazione in cui il giocatore corrente ha portato un
            pedone sul lato opposto della scacchiera e può sostituirlo con un
            cavallo, un alfiere, una torre o una regina.
2. **Tournament Management**: permettere di organizzare dei tornei che includono
   più partite tra diversi giocatori autenticati.
   1. **Tournament Configuration**: permettere a un amministratore di creare e
      configurare dei tornei di scacchi (es.: massimo numero di partecipanti,
      numero di round...).
   2. **Tournament Participation**: permettere a un giocatore autenticato di 
      partecipare a un torneo.
   3. **Tournament Execution**: gestione dell'esecuzione di un torneo, basandosi
      sul sistema svizzero.
      1. **Round Execution**: gestione di un round del sistema svizzero.
         1. **Participant Pairing**: gestione della formazione delle coppie di 
            giocatori autenticati che devono affrontarsi, sulla base dei risultati
            di ciascun giocatore autenticato.
         2. **Match Execution**: gestione dell'esecuzione dei match tra le coppie
            di giocatori autenticati che devono affrontarsi.
         3. **Result Aggregation**: gestione dell'aggregazione dei risultati dei
            match del round eseguiti.
   4. **Tournament Awards**: gestione della premiazione del torneo.
   5. **Tournament Storage**: gestione della memorizzazione dei dati relativi
      ai tornei (es.: numero di partecipanti massimi e correnti...).
3. **Authentication Management**: permettere a un giocatore ospite di autenticarsi 
   all'interno dell'applicazione.
   1. **Sign In**: permettere a un giocatore ospite di registrarsi all'applicazione.
      1. **Registration Form**: gestione dell'inserimento dei dati del giocatore ospite.
         In particolare, sono richiesti la sua email, il suo username e la sua password;
      2. **Confirmation Email**: gestione dell'email per ultimare la registrazione del 
         giocatore ospite, verificando che l'email da lui specificata sia effettivamente
         la sua.
   2. **Log In**: permettere a un giocatore ospite di accedere all'applicazione,
      conoscendo le proprie credenziali.
      1. **Token Creation**: creazione di un token utente riferito a una sessione
         attiva di un giocatore autenticato, richiesto per accedere alle operazioni
         sensibili dell'applicazione (es.: cambio della password...);
      2. **Token Expiration**: gestire la scadenza dei token utente, per limitare
         la validità di uno specifico accesso nel tempo;
      3. **Authorization Management**: gestire i permessi dell'utente in base al
         suo ruolo nell'applicazione (es.: dipendente dell'azienda, giocatore...).
   3. **Log out**: permettere a un giocatore autenticato di disconnettersi 
      dall'applicazione.
      1. **Token Revocation**: gestione la revoca ed eliminazione del token
         utente riferito alla sessione attiva del giocatore autenticato appena 
         disconnesso.
   4. **Sensitive Data Storage**: gestione dei dati sensibili dei giocatori registrati
      all'applicazione.
      1. **Secure Storage**: gestione della memorizzazione dei dati sensibili su
         una piattaforma sicura. Tra i dati sensibili, sono inclusi l'email del
         giocatore, la sua password ed i token utente delle sessioni attive.
      2. **Cryptography**: gestione dell'oscuramento dei dati sensibili (es.:
         password degli utenti dell'applicazione...).
4. **Profile Management**: permettere a un giocatore autenticato di gestire il proprio
   profilo utente.
   1. **Profile Visualization**: permettere a un giocatore autenticato di visualizzare 
      il proprio profilo utente, ovvero le informazioni relative al proprio account 
      (es.: email, username...).
   2. **Profile Update**: permettere a un giocatore autenticato di aggiornare le 
      informazioni relative al proprio account (es.: email, password...).
5. **Socialization Management**: permettere ai giocatori di interagire e socializzare tra di loro.
   1. **Friend Management**: gestione delle amicizie all'interno dell'applicazione.
      1. **Friend Request**: permettere a due giocatori autenticati di stringere amicizia.
         1. **Send Request**: permettere a un giocatore autenticato di inviare una richiesta
            di amicizia a un altro giocatore registrato all'applicazione.
            1. **In-Game Request**: permettere a un giocatore autenticato di inviare una richiesta
               di amicizia al giocatore autenticato avversario durante una partita.
            2. **Request By Username**: permettere a un giocatore autenticato di inviare una richiesta
               di amicizia a un altro giocatore registrato all'applicazione, conoscendone lo username.
         2. **Receive Request**: permettere a un giocatore autenticato di accettare o rifiutare una 
            richiesta di amicizia ricevuta da un altro giocatore registrato all'applicazione.
            1. **Request Visualization**: permettere a un giocatore autenticato di visualizzare
               le richieste di amicizia ricevute dagli altri giocatori registrati all'applicazione.
            2. **Request Notification**: gestione della notifica a un giocatore autenticato della
               ricezione di una nuova richiesta di amicizia.
      2. **Friend Visualization**: permettere a un giocatore autenticato di visualizzare se i propri 
         amici sono offline, online o all'interno di una partita.
      3. **Friend Removal**: permettere a un giocatore autenticato di rimuovere un altro giocatore dalla
         lista dei suoi amici.
      4. **Friend Storage**: gestione della memorizzazione degli amici dei giocatori
         e del loro stato.
   2. **Communication Management**: permettere ai giocatori di comunicare tra di loro.
      1. **Chat**: permettere ai giocatori di scambiarsi dei messaggi testuali tra di loro.
         1. **In-Game Chat**: permettere a un giocatore di scambiare dei messaggi testuali con il 
            proprio avversario durante una partita.
            1. **Send Message**: permettere a un giocatore di inviare messaggi testuali al proprio
               avversario durante una partita.
            2. **Receive Message**: permettere a un giocatore di ricevere messaggi testuali provenienti
               dal proprio avversario durante una partita.
            3. **Message Visualization**: permettere a un giocatore di visualizzare i messaggi testuali
               scambiati con il proprio avversario durante una partita.
            4. **Message Notification**: gestione della notifica a un giocatore della ricezione di un 
               messaggio dell'avversario durante una partita.
         2. **Friend Chat**: permettere a un giocatore autenticato di scambiare dei messaggi testuali con
            un suo amico.
            1. **Send Message**: permettere a un giocatore autenticato di inviare messaggi testuali a un
               suo amico.
            2. **Receive Message**: permettere a un giocatore registrato di ricevere messaggi testuali
               provenienti da un suo amico.
            3. **Message Visualization**: permettere a un giocatore autenticato di visualizzare i messaggi
               testuali scambiati con un suo amico.
            4. **Message Forwarding**: gestione dell'inoltro di un messaggio da un giocatore autenticato
               a un suo amico.
            5. **Message Notification**: gestione della notifica a un giocatore autenticato della ricezione
               di un messaggio di uno dei suoi amici.
            6. **Friend Chat Storage**: gestione della memorizzazione dei messaggi scambiati tra ogni
               giocatore registrato e i suoi amici.
6. **Statistics Management**: permettere a un giocatore di monitorare le statistiche di
   un giocatore registrato all'applicazione, tra cui le proprie statistiche.
   1. **Score Visualization**: permettere a un giocatore di visualizzare il punteggio ELO
      di un giocatore registrato all'applicazione.
      1. **Score Evaluation**: gestione della valutazione del punteggio di
         un giocatore autenticato al termine di ogni partita.
      2. **Score Storage**: gestione della memorizzazione dello storico dei
         punteggi di ciascun giocatore registrato all'applicazione.
      3. **Score History Visualization**: permettere a un giocatore di visualizzare come è cambiato
         nel tempo il punteggio ELO di un giocatore registrato all'applicazione.
   2. **Tournament Visualization**: permettere a un giocatore di visualizzare i risultati ottenuti
      nei tornei a cui ha partecipato un giocatore registrato all'applicazione.
      1. **Tournament Storage**: gestire la memorizzazione dei risultati di ogni torneo
         dei giocatori registrati all'applicazione.
   3. **Leaderboard Visualization**: permettere a un giocatore di visualizzare la classifica globale
      dei giocatori registrati all'applicazione.
      1. **Rank Visualization**: permettere a un giocatore autenticato di visualizzare la propria
         posizione nella classifica globale.
7. **Notification Management**: gestione delle notifiche dell'applicazione.
   1. **Notification Forwarding**: gestione della notifica in tempo reale ai
      giocatori autenticati degli eventi che li coinvolgono;
   2. **Notification Storage**: gestione della memorizzazione delle notifiche
      relative ai giocatori registrati all'applicazione.
8. **Sponsor Management**: gestione della pubblicità agli sponsor dell'applicazione
   (es.: banner, video...).

---
[Back to Index](../index.md) | [Back to Scoping](../1-scoping/index.md#rbs)