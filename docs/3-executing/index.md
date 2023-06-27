---
title: Executing
layout: default
nav_order: 5
---

# Executing
{: .no_toc}

In questa sezione, si descriverà il processo seguito per gestire la coordinazione del team di sviluppo durante
l'esecuzione del piano di progetto.

## Contenuti
{: .no_toc}

- TOC 
{:toc}

---

## Executing Kick-Off

In questa fase di Executing, è stato organizzato il seguente meeting per partire con lo sviluppo del progetto.

- Partecipanti:
  - Claudio Rossi, in qualità di Committente e Project Sponsor;
  - Paola Celeste, in qualità di Project Manager lato cliente e Project Champion;
  - Pietro Magnolia, in qualità di Project Manager lato fornitore e di Facilitatore, ovvero mediatore della riunione;
  - Core Team lato cliente, come consulente per il Project Manager lato cliente:
    - Cristina Grigi
    - Camilla Gialli
    - Cesare Neri
    - Carlo Verdi
  - Core Team lato fornitore, come consulente per il Project Manager lato fornitore:
    - Francesco Marroni, in qualità di Tecnografo, per la stesura del verbale.
    - Filippo Ecru
    - Federica Viola
    - Franca Arancioni
- Agenda:
  - Presentazione del Committente, come sponsor del progetto;
  - Presentazione del Project Team;
  - Introduzione al progetto;
  - Revisione del PDS;
  - Revisione della schedula e delle responsabilità;
  - Definizione dei Work Package;
  - Definizione delle regole operative.
- Data: 17-02-2023
- Durata: 8 ore
- Verbale: [link](/pm/attachments/content/meeting-reports/executing/executing-kickoff)

## Project Team

Durante la fase di Executing, prima dell'Executing Kick-Off, è stato formato il Project Team, ovvero il team che si
occuperà dello sviluppo del progetto, già in parte definito durante la fase di Planning.

In particolare, il Project Team si compone dei seguenti membri:
- Developer Team:
  - _Pietro Magnolia_, in qualità di Project Manager e IT Acquisition Specialist;
  - _Francesco Marroni_, in qualità di UX Designer e Senior Frontend Developer;
  - _Filippo Ecru_, in qualità di Quality Assurance Tester e Junior Frontend Developer;
  - _Federica Viola_, in qualità di Database Administrator e Junior Backend Developer;
  - _Franca Arancioni_, in qualità di DevOps Engineer e Senior Backend Developer;
  - _Fiorella Bordeaux_, in qualità di Junior Frontend Developer;
  - _Fernando Kaki_, in qualità di Junior Backend Developer.
- Client Team:
  - _Paola Celeste_, in qualità di Project Manager e Project Champion.

## Work Packages

Durante l'Executing Kick-Off, dopo la revisione delle attività della schedula, sono stati definiti i Work Package del
progetto, ovvero dei raggruppamenti di attività che condividono delle caratteristiche in comune, disponibili al seguente
[link](/pm/attachments/content/work-packages#17-02-2023).

In particolare, si è deciso di suddividere le attività in base ai servizi da realizzare, come già fatto durante la fase
di Planning, quindi definendo un Work Package per ogni servizio, ovvero:
- Frontend Work Package: include tutte le attività relative al servizio di Frontend;
- Backend Work Package: include tutte le attività relative al servizio di Backend;
- Authentication Work Package: include tutte le attività relative all'Authentication Service;
- Statistics Work Package: include tutte le attività relative allo Statistics Service;
- Notification Work Package: include tutte le attività relative al Notification Service;
- Game Work Package: include tutte le attività relative al Game Service;
- Tournament Work Package: include tutte le attività relative al Tournament Service;
- Friend Work Package: include tutte le attività relative al Friend Service;
- Message Work Package: include tutte le attività relative al Message Service.

Quindi, sono stati aggiunti dei Work Package per facilitare la gestione del progetto:
- Closing Work Package: include tutte le attività di chiusura del progetto;
- Critical Work Package: include tutte le attività nel percorso critico.

Infine, è stato definito un Work Package per ciascuno dei membri del Developer Team, contenente le attività che dovrà
svolgere.

## Regole Operative

Al termine dell'Executing Kick-Off, sono state definite le regole operative che il Developer Team dovrà seguire durante
lo sviluppo del progetto.

### Daily Status Meeting

La comunicazione all'interno del team avverrà principalmente attraverso dei meeting giornalieri di breve durata
(all'incirca 15 minuti), che hanno lo scopo di monitorare lo stato di avanzamento del progetto.

In questi meeting, ogni membro del team dovrà indicare l'attività che ha intenzione di svolgere in giornata, il suo
stato di avanzamento ed eventuali problemi che sono stati riscontrati.

### Problem Resolution Meeting

Durante un Daily Status Meeting, nel caso in cui si individuasse un problema, sarà necessario individuarne i membri del
team interessati o responsabili, in modo da organizzare una riunione specifica per la risoluzione del problema.

In tale riunione, sarà necessario chiarire qual è il problema e chi ne è responsabile. A questo punto, il responsabile
dovrà raccogliere dei dati per individuare le cause del problema e proporre possibili soluzioni.

Quindi, segue una breve valutazione delle soluzioni al problema, per determinare quale possa essere la più efficace ed
efficiente.

Infine, bisognerà riportare l'esito dell'implementazione di tale soluzione con eventuali note all'interno dell'Issue
Log, allo scopo di arricchire l'esperienza progettuale dell'azienda.

### Decision-Making

Ogni membro del team ha facoltà di scegliere autonomamente tra le diverse alternative che individua per lo svolgimento
di un'attività di cui è responsabile.

Nel caso in cui un membro del team avesse il dubbio che una scelta potesse influenzare anche altre attività oltre che la
propria, sarà necessario notificarne prima il team durante un Daily Status Meeting. A questo punto, il Project Manager
potrà decidere se affidare la scelta a quel membro del team oppure organizzare una riunione apposita con i diretti
interessati, allo scopo di raggiungere un consenso sulla scelta.

In tale riunione, il Project Manager assumerà il ruolo di Facilitatore. In particolare, nel caso in cui non si riuscisse
a raggiungere un consenso tra i membri coinvolti, avrà il potere di decidere sulla base di quanto detto nella riunione.

### Conflict Resolution

Nel caso in cui si generasse un conflitto tra due o più membri del team, sarà necessario notificarlo durante un Daily
Status Meeting. A questo punto, il Project Manager potrà decidere di organizzare una riunione apposita per la
risoluzione del conflitto.

In tale riunione, ogni membro del team dovrà esprimere la propria opinione, ricordandosi che tutte le opinioni hanno lo
stesso valore. Quindi, nel caso in cui il conflitto non si risolvesse spontaneamente, il Project Manager potrà agire da
mediatore e in casi estremi forzarne la risoluzione.

### Communication Management

Per quanto riguarda la comunicazione tra i membri del team, si dovrà prediligere una comunicazione di tipo verbale da
svolgersi principalmente durante i Daily Status Meeting.

In alternativa, sarà possibile adottare una comunicazione scritta utilizzando l'apposito spazio di lavoro predisposto su
Slack.

### Scope Change Management

Nel caso in cui il Project Manager lato fornitore o il Committente individuassero la necessità di un cambiamento sullo
Scope di progetto, sarà necessario redarre una Scope Change Request, in cui si informa la controparte dei dettagli su
tale cambiamento.

All'approvazione della Scope Change Request dalla controparte, il Project Manager insieme al suo Core Team dovranno
redarre il relativo Project Impact Statement, che analizza l'impatto che tale cambiamento avrà sul progetto (es.:
aumento o diminuzione dei costi del progetto, modifiche sulla schedula, riduzione dei requisiti...).

In seguito all'approvazione del Project Impact Statement da parte del Committente, il Project Manager dovrà impegnarsi
nella revisione del piano di progetto, eventualmente attingendo alla Scope Bank.

---

[Back to Top](#top) |
[Previous Chapter](/pm/2-planning) |
[Next Chapter](/pm/4-monitoring-and-controlling)