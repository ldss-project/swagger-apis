---
title: Planning
layout: default
nav_order: 4
---

# Planning
{: .no_toc}

In questa sezione, si descriverà il processo seguito per entrare nel dettaglio di ciò che è stato definito in fase di
Scoping, allo scopo di ridurre l'incertezza sul progetto e determinare la schedula e i costi del progetto.

## Contenuti
{: .no_toc}

- TOC 
{:toc}

---

## Joint Project Planning Sessions

In questa fase di Planning, sono stati organizzati i seguenti meeting in giornate separate, distribuiti nell'arco
di due settimane.

### Planning Kick-Off

- Partecipanti:
  - Claudio Rossi, in qualità di Committente e Project Sponsor; 
  - Paola Celeste, in qualità di Project Manager lato cliente e Project Champion;
  - Pietro Magnolia, in qualità di Project Manager lato fornitore;
  - Core Team lato cliente, come consulente per il Project Manager lato cliente:
    - Cristina Grigi
    - Camilla Gialli
    - Cesare Neri
    - Carlo Verdi
  - Core Team lato fornitore, come consulente per il Project Manager lato fornitore:
    - Francesco Marroni
    - Filippo Ecru
    - Federica Viola
    - Franca Arancioni
  - Pietro Magnolia, in qualità di Facilitatore, come mediatore della riunione;
  - Francesco Marroni, in qualità di Tecnografo, per la stesura del verbale.
- Agenda:
  - Presentazione del Committente, come sponsor del progetto;
  - Presentazione del Project Manager lato cliente e del Project Manager lato fornitore;
  - Presentazione dei Core Team lato cliente e lato fornitore;
  - Definizione del Planning Facilitation Team;
  - Presentazione del progetto;
  - Revisione e assegnamento delle priorità ai requisiti;
  - Organizzazione delle successive Joint Project Planning Sessions.
- Data: 30-01-2023
- Durata: 4 ore
- Verbale: [link](/pm/attachments/content/meeting-reports/planning/planning-kickoff)

### Work Definition Meeting

- Partecipanti:
  - Paola Celeste, in qualità di Project Manager lato cliente e Project Champion;
  - Pietro Magnolia, in qualità di Project Manager lato fornitore;
  - Core Team lato cliente, come consulente per il Project Manager lato cliente:
    - Cristina Grigi
    - Camilla Gialli
    - Cesare Neri
    - Carlo Verdi
  - Core Team lato fornitore, come consulente per il Project Manager lato fornitore:
    - Francesco Marroni
    - Filippo Ecru
    - Federica Viola
    - Franca Arancioni
  - Pietro Magnolia, in qualità di Facilitatore, come mediatore della riunione;
  - Francesco Marroni, in qualità di Tecnografo, per la stesura del verbale;
  - Renato Beige, in qualità di Resource Manager lato fornitore.
- Agenda:
  - Presentazione dell'architettura di massima del sistema;
  - Presentazione e revisione delle attività del progetto;
    - Presentazione e revisione della WBS;
    - Presentazione e revisione dell'analisi sulle attività, discutendo tempi, costi e risorse.
  - Revisione del PMLC Model.
- Data: 06-02-2023, 07-02-2023
- Durata: 8 ore, divise su due giornate
- Verbale: [link](/pm/attachments/content/meeting-reports/planning/work-definition-meeting)

### Project Proposal Submission Meeting

- Partecipanti:
  - Claudio Rossi, in qualità di Committente e Project Sponsor;
  - Paola Celeste, in qualità di Project Manager lato cliente e Project Champion;
  - Pietro Magnolia, in qualità di Project Manager lato fornitore;
  - Core Team lato cliente, come consulente per il Project Manager lato cliente:
    - Cristina Grigi
    - Camilla Gialli
    - Cesare Neri
    - Carlo Verdi
  - Core Team lato fornitore, come consulente per il Project Manager lato fornitore:
    - Francesco Marroni
    - Filippo Ecru
    - Federica Viola
    - Franca Arancioni
  - Pietro Magnolia, in qualità di Facilitatore, come mediatore della riunione;
  - Francesco Marroni, in qualità di Tecnografo, per la stesura del verbale;
- Agenda:
  - Discussione della proposta di progetto:
    - Descrizione della situazione attuale;
    - Descrizione della situazione desiderata;
    - Descrizione della strategia da applicare;
    - Descrizione delle attività del progetto;
    - Descrizione della schedula e dei costi del progetto.
  - Discussione sulla fattibilità di dettaglio del progetto;
  - Approvazione del piano di progetto.
- Data: 13-02-2023
- Durata: 4 ore
- Verbale: [link](/pm/attachments/content/meeting-reports/planning/project-proposal-submission-meeting)

## Priorità dei requisiti

Durante il Planning Kick-Off, dopo la presentazione del progetto, il Committente ha indicato le priorità degli obiettivi
del progetto, riportate di seguito. Per definire la priorità dei requisiti è stato adottato lo standard MoSCoW.

| Obiettivo                 | Descrizione                                                                                                                                                                                                                         | Priorità    | Motivazione                                              |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|----------------------------------------------------------|
| Game Management           | Gestire la creazione, la configurazione e la partecipazione a delle partite di scacchi online, allo scopo di permettere agli utenti dell'applicazione di divertirsi insieme.                                                        | Must-Have   | Necessario per l'applicazione.                           |
| Authentication Management | Gestire l'autenticazione degli utenti all'interno dell'applicazione ed i loro permessi, allo scopo di permettere al Committente di amministrare l'applicazione e di permettere ai giocatori di tenere traccia dei propri progressi. | Must-Have   | Necessario per amministrare l'applicazione.              |
| Sponsor Management        | Gestire la pubblicità agli sponsor del progetto, allo scopo di permettere al Committente di adottare una nuova strategia di business aggiuntiva.                                                                                    | Must-Have   | Necessario per adottare la nuova strategia di business.  |
| Tournament Management     | Gestire la creazione, la configurazione e la partecipazione a dei tornei di scacchi, allo scopo di aumentare la visibilità e la popolarità dell'applicazione.                                                                       | Should-Have | Molto importante per la visibilità dell'applicazione.    |
| Statistics Management     | Gestire il monitoraggio delle statistiche dei giocatori e una classifica globale, allo scopo di permettere ai giocatori di osservare la propria crescita nel tempo e di competere con altri giocatori.                              | Could-Have  | Importante per il coinvolgimento dei giocatori.          |
| Socialization Management  | Gestire un sistema di amicizie e di comunicazione tra i giocatori nell'applicazione allo scopo di permettere agli utenti di socializzare all'interno dell'applicazione, facilitando la creazione di una comunità di giocatori.      | Could-Have  | Importante per la crescita di una comunità di giocatori. |

In questa fase, si è iniziata la stesura del Project Definition Statement (PDS), che sarà completata durante il Planning.
Inoltre, sono stati aggiornate le User Stories, disponibili al seguente [link](/pm/attachments/content/user-stories#31-01-2023),
e la RBS, disponibile al seguente [link](/pm/attachments/content/rbs#31-01-2023).

## Work Breakdown Structure (WBS)

Tra il Planning Kick-Off e la Work Definition Meeting, il fornitore ha lavorato per trasformare la RBS nella WBS,
disponibile al seguente [link](/pm/attachments/content/wbs/#01-02-2023), identificando il design architetturale della
soluzione e le attività del progetto. 

Siccome il Core Team è piuttosto piccolo, si è deciso di coinvolgere l'intero team nella definizione della WBS, senza
suddividerlo in sub-team.

### Design Architetturale

Durante una serie di riunioni interne all'azienda del fornitore, si è delineato il design architetturale della soluzione
da realizzare. In particolare, si è deciso di adottare un'architettura a servizi, che raggruppano i requisiti del 
progetto definiti nella RBS.

Per tale architettura, si è deciso di applicare il pattern Ports&Adapters, anche conosciuto come architettura esagonale.

I servizi individuati dal Core Team sono i seguenti:
- **Frontend Service**: servizio che si occupa della rappresentazione grafica dell'applicazione web e della
  sponsorizzazione da parte degli investitori esterni.
  Dipende da:
  - _Backend Service_: che utilizza per accedere alle funzionalità dell'applicazione.
- **Backend Service**: servizio che gestisce l'inoltro delle richieste e delle connessioni dell'utente all'interno del 
  sistema. Questo servizio agisce da interfaccia ai seguenti servizi:
  - **Authentication Service**: servizio che gestisce l'autenticazione e l'autorizzazione dei giocatori nell'applicazione.
    Questo servizio necessita di uno storage persistente per mantenere le informazioni relative al profilo degli utenti e
    i token necessari per gestire i loro permessi all'interno dell'applicazione;
  - **Statistics Service**: servizio che si occupa della gestione delle statistiche dei giocatori, tenendo traccia del
    loro punteggio ELO e dei loro risultati nei tornei in cui hanno partecipato. Inoltre, gestisce la leaderboard 
    dell'applicazione.
    Dipende da:
    - _Authentication Service_: che utilizza per verificare l'identità dei giocatori.
  - **Notification Service**: servizio che gestisce la creazione, l'eliminazione e l'inoltro in tempo reale delle notifiche
    ai giocatori dell'applicazione. Questo servizio necessita di uno storage persistente per le notifiche non ancora
    visualizzate dall'utente. \
    Dipende da:
    - _Authentication Service_: che utilizza per verificare l'identità dei giocatori.
  - **Game Service**: servizio che si occupa della creazione, configurazione, partecipazione ed esecuzione delle partite 
    di scacchi. \
    Dipende da:
    - _Notification Service_: che utilizza per notificare i giocatori dello sviluppo della partita a cui stanno partecipando;
    - _Statistics Service_: a cui invia i risultati delle partite per aggiornare il punteggio ELO dei giocatori.
  - **Tournament Service**: servizio che si occupa della creazione, configurazione, partecipazione ed esecuzione dei
    tornei di scacchi. Questo servizio necessita di uno storage persistente per i tornei, che potrebbero essere organizzati
    mesi prima dell'esecuzione e quindi avere un ciclo di vita a lungo termine, al contrario delle semplici partite di
    scacchi. \
    Dipende da:
    - _Game Service_: che utilizza per gestire le partite dei tornei;
    - _Notification Service_: che utilizza per notificare i giocatori dello sviluppo del torneo a cui stanno partecipando;
    - _Statistics Service_: a cui invia i risultati dei tornei per aggiornare le statistiche dei giocatori;
    - _Authentication Service_: che utilizza per verificare l'identità dei giocatori.
  - **Friend Service**: servizio che si occupa della gestione delle amicizie tra i giocatori dell'applicazione, tenendo
    traccia delle richieste di amicizia pendenti oppure accettate. \
    Dipende da:
    - _Notification Service_: che utilizza per notificare i giocatori delle richieste di amicizia;
    - _Authentication Service_: che utilizza per verificare l'identità dei giocatori.
  - **Message Service**: servizio che si occupa dell'inoltro dei messaggi tra i giocatori amici nell'applicazione.
    Dipende da:
    - _Notification Service_: che utilizza per notificare i giocatori dei messaggi ricevuti;
    - _Friend Service_: che utilizza per verificare l'amicizia tra i giocatori.

### Attività del progetto

Dopo aver definito le attività del progetto a partire dalla RBS, quindi motivandole rispetto ai requisiti del progetto,
si è deciso di riorganizzarle rispetto ai servizi previsti dal design architetturale.

## Analisi delle attività

In seguito alla definizione della WBS, il Core Team lato fornitore si è riunito per stimare il carico di lavoro, la
durata e le risorse relativamente alle attività di progetto. I risultati di tale analisi sono disponibili al seguente
[link](/pm/attachments/content/task-analysis#03-02-2023).

In particolare, per l'analisi delle attività è stato utilizzata la _Wideband Delphi Technique_, ovvero un metodo
iterativo per convergere a un consenso dei partecipanti sulla complessità delle attività.

Inizialmente, è stata stimata la complessità delle attività in _ore/uomo_, quindi tale complessità è stata
trasformata in durata, considerando una sola risorsa assegnata all'attività, con un'efficienza pari al 75% e prevedendo
ritardi pari al 33% della durata ideale dell'attività.

Infine, per ogni attività sono state individuate le risorse e le skill necessarie.

Al termine dell'analisi, è stata estrapolata la durata massima attesa per il progetto, pari a circa 14-15 mesi, nel caso
in cui il team di sviluppo fosse composto da una sola persona, ovvero senza parallelismo tra le attività. Durante la 
stesura della Schedula, sarà necessario parallelizzare il maggior numero di attività per rientrare nei 6 mesi previsti
dalle Conditions of Satisfaction.

## Assegnamento delle risorse

Una volta individuate le risorse necessarie allo svolgimento di ogni attività, è stato possibile individuarne il
responsabile tra il personale aziendale. Come risultato di questo processo, è stata derivata la matrice delle
responsabilità, disponibile al seguente [link](/pm/attachments/content/responsibility-matrix#03-02-2023).

## Analisi dei rischi

In seguito all'analisi delle attività, è stata eseguita un'analisi sui rischi individuati durante la fase di Scoping
nella Swot Analysis, allo scopo di determinarne l'impatto atteso e trasformarlo in un costo atteso per i rischi del
progetto.

I risultati di tale analisi sono disponibili al seguente [link](/pm/attachments/content/risk-analysis#03-02-2023).

In previsione del monitoraggio dei rischi, insieme all'analisi, è già stato predisposto un template da usare come Risk
Log.

## Analisi dei costi

Dopo aver individuato il carico di lavoro, la durata e le risorse necessarie per le singole attività del progetto, è
stato possibile portare avanti l'analisi dei costi su tali attività, disponibile al seguente 
[link](/pm/attachments/content/cost-analysis#03-02-2023).

In seguito all'analisi dei costi, è stato possibile determinare una stima sul costo del progetto, basata su tre fattori
principali:
- Costi di Manodopera: dovuti al mantenimento del team incaricato allo sviluppo del progetto;
- Costi di Strumentazione: dovuti all'acquisizione di strumenti hardware o software;
- Costi di Gestione: dovuti alla gestione delle attività di progetto (es.: stipendio del Project Manager...).

Al termine dell'analisi, è stato estrapolato il costo atteso per il progetto, pari a circa 150000$, al quale si ha
intenzione di aggiungere un 10% di riserva giustificato dai rischi del progetto, pari a circa 15000$, e almeno un 20% di
margine, pari a circa 30000$.

Il Project Manager potrà attingere a tale margine nel caso di imprevisti rispetto al piano di progetto, previa
consultazione del senior management. Tuttavia, è richiesta la sua competenza per minimizzare i rischi legati a tali 
imprevisti, massimizzando il margine per l'azienda.

### Cash Flow Management

Per quanto riguarda la gestione dei costi del progetto, il Project Manager lato fornitore ha intenzione di richiedere
al Committente di distribuire il pagamento del progetto in quattro fasi:
- Anticipo a inizio progetto: un primo pagamento con un valore pari al 20% del costo del progetto, ovvero 39000$;
- Primo controllo: dopo due mesi dall'inizio progetto, si prevederà un primo controllo in cui sarà coinvolto il 
  Committente per mostrargli lo stato dei lavori. Se durante tale controllo, si converrà che il piano di progetto è
  stato rispettato opportunamente, allora si prevederà un secondo pagamento di importo pari a 39000$;
- Secondo controllo: dopo quattro mesi dall'inizio del progetto, si prevederà un secondo controllo, a cui seguirà un
  terzo pagamento pari a 39000$;
- Saldo a fine progetto: alla consegna del progetto, si prevederà un ultimo pagamento pari al 40% del costo del progetto,
  ovvero 78000$.

## Schedula

Tra il Work Definition Meeting e il Project Proposal Submission Meeting, il Project Manager lato fornitore
ha definito prima il Project Network Diagram (PND), per poter quindi generare il Gantt Chart per la schedula del
progetto.

### Project Network Diagram (PND)

Per definire il Project Network Diagram (PND), è stato necessario esplicitare le dipendenze tra le attività del
progetto.

Le dipendenze individuate tra le varie attività del progetto sono state principalmente di due tipi:
- _Vincoli logici_: impediscono a un'attività di cominciare prima di un'altra da cui dipende;
- _Vincoli di risorse_: impediscono a un'attività di cominciare prima che il suo responsabile sia disponibile.

Il risultato dell'analisi delle dipendenze tra le attività è il diagramma seguente.

[![Project Network Diagram](/pm/resources/diagrams/project-network-diagram.jpg)](https://miro.com/app/board/uXjVM9abzds=/?share_link_id=313338560385)

> _**NOTA**_: cliccare sull'immagine per visualizzare il diagramma su _Miro_.

Nel diagramma, per ogni attività sono state descritte le seguenti informazioni:
- _Id_: identificatore dell'attività;
- _Descrizione_: descrizione del contenuto dell'attività;
- _Responsabile_: la persona incaricata dello svolgimento dell'attività;
- _Durata_: la durata in ore dell'attività;
- _Slack_: il massimo ritardo in ore che l'attività può subire senza ritardare la consegna del progetto;
- _Earliest Start/Finish_: la prima data disponibile per cominciare/terminare l'attività;
- _Latest Start/Finish_: l'ultima data disponibile per cominciare/terminare l'attività, senza causare un ritardo
  sulla consegna del progetto.

Quindi, è stato evidenziato il percorso critico (visibile nelle transizioni in grassetto) e conseguentemente
è stata determinata una stima della durata del progetto, pari a circa 112 giorni lavorativi, a cui sono stati
aggiunti circa 11 giorni lavorativi come Scope Bank, equivalenti al 10% della durata del progetto.

Pertanto, la durata effettiva del progetto ammonta a poco meno di 6 mesi, garantendo il rispetto delle Conditions
of Satisfaction.

### Gantt Chart

Dopo la definizione del Project Network Diagram, è stato possibile generare il Gantt Chart, disponibile al seguente
[link](https://app.asana.com/0/1204894076877574/1204894076877574), in cui sono state decise le date effettive delle
attività del progetto.

> _**NOTA**_: per utilizzare il link è necessario possedere delle credenziali di un account Asana appartenente al
> gruppo del progetto.

## Contratto

Il contratto che il Project Manager ha intenzione di proporre al Committente è un contratto a corpo, quindi a prezzo
predeterminato, stabilito sulla base del piano di progetto. Tuttavia, come già menzionato, saranno previsti diversi
pagamenti durante lo svolgimento del progetto.

## PDS

...

---

[Back to Top](#top) |
[Previous Chapter](/pm/1-scoping) |
[Next Chapter](/pm/3-executing)