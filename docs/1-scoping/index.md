# Scoping

In questa sezione, si descriverà il processo seguito per comprendere la situazione attuale del committente e i
suoi desideri, definendo gli obiettivi del progetto di conseguenza.

All'interno di questa sezione si distingueranno due Project Manager: quello _lato cliente_ (rappresentante di
GameCo) e quello _lato fornitore_ (rappresentante della nostra azienda).

## Scoping Meetings

In questa fase di Scoping, sono stati organizzati i seguenti meeting in giornate separate, distribuiti nell'arco
di due settimane:
- **Problem Definition Meeting**:
  - Partecipanti:
    - Project Manager lato cliente;
    - Project Manager lato fornitore;
    - Facilitatore, come mediatore della riunione;
    - Tecnografo, per la stesura del verbale.
  - Agenda:
    - Presentazione tra il Project Manager lato cliente e Project Manager lato fornitore;
    - Presentazione del business di GameCo;
    - Descrizione della situazione attuale di GameCo (ovvero dell'_as is_);
    - Descrizione del problema o dell'opportunità individuata da GameCo;
    - Descrizione della situazione desiderata da GameCo (ovvero del _to be_);
    - Definizione delle Conditions of Satisfaction a livello di progetto.
  - Data: 10-01-2023
  - Durata: 4 ore
  - Verbale: [link](../attachments/meeting-reports/scoping/problem-definition-meeting.md)
- **Requirements Definition Meeting**:
  - Partecipanti:
      - Project Manager lato cliente;
      - Project Manager lato fornitore;
      - Core Team lato cliente, come consulente per il Project Manager lato cliente;
      - Core Team lato fornitore, come consulente per il Project Manager lato fornitore;
      - Facilitatore, come mediatore della riunione;
      - Tecnografo, per la stesura del verbale.
  - Agenda:
    - Presentazione dei Core Team di entrambe le parti;
    - Definizione delle User Stories, ovvero dei requisiti del progetto e delle Conditions of Satisfaction a livello
      di deliverable;
    - Discussione del gap tra l'_as is_ ed il _to be_;
    - Discussione e revisione della RBS.
  - Data: 12-01-2023, 16-01-2023
  - Durata: 8 ore, divise su due giornate
  - Verbale: [link](../attachments/meeting-reports/scoping/requirements-definition-meeting.md)
- **POS Submission Meeting**:
  - Partecipanti:      
    - Project Manager lato cliente;
    - Project Manager lato fornitore;
    - Core Team lato cliente, come consulente per il Project Manager lato cliente;
    - Core Team lato fornitore, come consulente per il Project Manager lato fornitore;
    - Facilitatore, come mediatore della riunione;
    - Tecnografo, per la stesura del verbale.
  - Agenda:
    - Discussione del POS redatto dal Project Manager lato fornitore:
      - Discussione sul problema e sulle opportunità del progetto;
      - Discussione sugli obiettivi del progetto;
      - Discussione dei criteri di successo del progetto;
      - Discussione di assunzioni, rischi e ostacoli;
      - Discussione del PMLC Model.
    - Discussione sulla fattibilità di massima del progetto;
    - Approvazione o rifiuto del POS.
  - Data: 23-01-2023
  - Durata: 4 ore.
  - Verbale: [link](../attachments/meeting-reports/scoping/pos-submission-meeting.md)

## Conditions of Satisfaction

Durante il Problem Definition Meeting, sono state definite delle Conditions of Satisfaction a livello di progetto, 
disponibili al seguente [link](../attachments/CoS.md), allo scopo di formalizzare e dettagliare gli effettivi
desideri del committente.

Inizialmente, particolare importanza è stata data alla definizione di vincoli di tempi e budget più precisi, per
comprendere meglio l'entità del progetto e successivamente facilitare la pianificazione e la gestione delle 
risorse.

## Definizione dei requisiti

### User Stories
Durante il Requirements Definition Meeting, sono stati definiti i requisiti di progetto in termini di User Stories,
disponibili al seguente [link](../attachments/user-stories.md). 
In questo modo, è stata condotta un'analisi sulle necessità degli utenti finali, ovvero dei giocatori dell'applicazione,
quindi i requisiti del progetto saranno il più vicino possibile all'utente finale. Quindi, le User Stories potranno
essere il riferimento per la verifica del sistema.

### RBS
Tra le due giornate del meeting, allo scopo di facilitare la pianificazione nelle fasi successive del progetto, si è 
lavorato per trasformare le User Stories in un RBS, disponibile al seguente [link](../attachments/RBS.md).

Siccome GameCo ha già realizzato un progetto relativo al gioco degli scacchi, sarà possibile riutilizzare alcuni dei 
requisiti di quel progetto, almeno per quanto riguarda la gestione delle regole di una partita di scacchi (`1.i.d` e
`1.iii`).

Dopo aver presentato e discusso l'RBS con il cliente, si è ottenuto un suo riscontro positivo, in seguito a cui è stata
iniziata la stesura del POS.

## Swot Analysis
Come fase preliminare alla stesura del POS, è stata svolta la SWOT Analysis, per cui sono stati analizzati i punti di 
forza e le debolezze del progetto, da cui sono state derivate le possibili opportunità e minacce per il progetto.

In particolare, i risultati della SWOT Analysis sono i seguenti:
- **Strength**: i fattori interni che possono contribuire al successo del progetto, ovvero:
  - Il cliente ha già realizzato un'applicazione di scacchi in passato, quindi è possibile usufruire della sua
    esperienza in ambito, oltre che riutilizzare parte dei requisiti di quell'applicazione;
  - Il cliente ha espresso una grande disponibilità riguardo il proprio coinvolgimento nel progetto, quindi si ha una
    maggiore garanzia che il risultato finale del progetto soddisfi le sue aspettative;
  - Il cliente è disposto a investire molto su questo progetto, quindi si ha una maggiore flessibilità sul budget;
  - Il fornitore ha molta esperienza nello sviluppo di applicazioni web, quindi si ha una maggiore garanzia sulla
    qualità e sul successo del progetto;
  - Il fornitore ha a disposizione l'applicazione concorrente come punto di riferimento per il risultato del progetto,
    quindi è possibile condurre delle analisi per individuare anticipatamente dei possibili difetti, pregi o
    miglioramenti della soluzione in fase di progettazione.
- **Weaknesses**: i fattori interni che possono contribuire al fallimento del progetto, ovvero:
  - Il cliente ha poca esperienza nel nuovo modello di business che ha intenzione di adottare, quindi esiste un rischio
    concreto che il cliente non riesca a soddisfare le sue aspettative, nonostante l'adeguatezza della soluzione.
  - Il cliente ha espresso una forte urgenza nel terminare il progetto, quindi si rischia di ridurre la qualità della
    soluzione, o addirittura di rinunciare a parte dei requisiti in caso di ritardi.
- **Opportunities**: i fattori esterni e gli obiettivi che possono contribuire al successo del progetto, ovvero:
  - L'opportunità di costruire una community attorno all'applicazione e quindi intorno all'azienda del cliente, 
    fidelizzando i giocatori coinvolti nella community e aumentando la popolarità dell'azienda.
  - L'opportunità di sviluppare un'applicazione accessibile direttamente dal browser, facilitando l'uso 
    dell'applicazione da parte dei giocatori e facilitando il contatto con nuovi utenti.
  - L'opportunità di entrare in un mercato con pochi competitori, quindi facilitando l'acquisizione di clienti
    fidelizzati.
- **Threats**: i fattori esterni che possono contribuire al fallimento del progetto, ovvero:
  - Il rischio di non distinguersi dall'applicazione concorrente abbastanza da risaltare sul mercato. 
    Per ridurre questo rischio, sarà necessario non ispirarsi troppo all'applicazione concorrente e adottare dei processi
    d'innovazione o creazione.
  - Il rischio che vengano rilasciate nuove applicazioni simili concorrenti, riducendo potenzialmente le opportunità di
    mercato. 
  - Il rischio che l'azienda concorrente aggiorni e migliori la propria applicazione, ostacolando l'entrata nel mercato
    da parte dell'azienda del cliente. 
    Per ridurre questo rischio, sarà necessario monitorare la concorrenza e adottare un approccio di sviluppo del 
    progetto flessibile rispetto ai requisiti (es.: iterativo), in modo da poter modificare tempestivamente la direzione
    del progetto.
    Tuttavia, questa flessibilità introduce nuovi rischi, come la difficoltà nella gestione dei cambiamenti dello Scope.
  - Il rischio che l'azienda del cliente non riesca ad individuare degli sponsor interessati a finanziare il mantenimento
    dell'applicazione, impedendo al cliente di coprire i costi del progetto e trarne profitto.
  - Il rischio che l'applicazione non diventi abbastanza popolare da riuscire a coprire i costi del progetto tramite i
    soli investimenti da parte degli sponsor.
    Per ridurre questo rischio, sarà necessario individuare nuove fonti di entrata, oltre alla sponsorizzazione (es.:
    offrire diversi template grafici a pagamento per il gioco, modificando l'aspetto dei pezzi e della scacchiera...)
  - Il rischio dovuto all'incertezza sulla tecnologia da usare per scalare i server di gioco, che richiede una fase di
    ricerca a tempo non determinato, potenzialmente ritardando il progetto.
    Per ridurre questo rischio, si potrebbe ricorrere a una consulenza esterna.
  - Il rischio dovuto all'incertezza sulla domanda dell'applicazione, per cui al rilascio l'applicazione potrebbe
    supportare troppi giocatori rispetto agli utilizzatori effettivi, quindi provocando un costo aggiuntivo inutile,
    oppure non supportare abbastanza giocatori rispetto agli utilizzatori effettivi, quindi provocando insoddisfazione
    nei giocatori.
    Per ridurre questo rischio, si dovrà eseguire un'analisi predittiva sulla domanda dell'applicazione oppure ricorrere
    a una consulenza esterna.

## PMLC Model
In seguito all'analisi del progetto, si ha ragionato sull'approccio migliore per la gestione del progetto.

Per quanto riguarda la possibilità di adottare un approccio tradizionale, si è considerato che si potrebbe approfittare
dell'esperienza di GameCO nello sviluppo di applicazioni di scacchi e dell'esperienza del fornitore nello sviluppo di
applicazioni web per produrre un piano completo del progetto, senza che sia necessario introdurre i rischi della
flessibilità dell'approccio iterativo (es.: posticipazione della pianificazione...).

Tuttavia, considerando i rischi legati alle aziende competitrici sul mercato, si è concluso che un approccio iterativo
possa essere la soluzione migliore, per poter reagire tempestivamente alle modifiche sui requisiti che potrebbe insorgere
durante il monitoraggio delle aziende competitrici.

## POS
- POS o Project Charter

---

[Back to Index](../index.md) |
[Previous Chapter](../0-request/index.md) |
[Next Chapter](../2-planning/index.md)