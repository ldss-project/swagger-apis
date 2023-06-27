---
title: Final Project Report
layout: default
parent: Allegati
nav_order: 16
---

# Final Project Report
{: .no_toc}

## Versioni
{: .no_toc}

- TOC
{:toc}

---

## 14-08-2023

[Back to Top](#top) |
[Back to Closing](/pm/5-closing#final-project-report)

### Problema

Il Committente ha subito un calo inaspettato nelle vendite di una sua applicazione di scacchi, pari a
circa il 70% rispetto ai valori attesi. La causa è stata attribuita alla pubblicazione di una nuova applicazione web
gratuita di scacchi, appartenente a un'azienda competitrice.

### Opportunità

Il Committente ha individuato l'opportunità di adottare una nuova strategia di business aggiuntiva,
permettendo di essere più robusti agli eventi esterni del mercato.

Rispetto alla strategia di business corrente, basata sulla vendita di applicazioni a pagamento tramite intermediario,
la nuova strategia di business aggiuntiva è basata sulla distribuzione di applicazioni gratuite sponsorizzate da
investitori esterni.

### Goal

Progettare un'applicazione web che permetta a una comunità di utenti di giocare a scacchi online, che sia
competitiva rispetto alle altre applicazioni concorrenti, entro sei mesi dall'approvazione del progetto.

### Obiettivi

In ordine di priorità decrescente:
1. `Must-Have` **Game Management**: gestire la creazione, la configurazione e la partecipazione a delle partite di
   scacchi online, allo scopo di permettere agli utenti dell'applicazione di divertirsi insieme;
2. `Must-Have` **Authentication Management**: gestire l'autenticazione degli utenti all'interno dell'applicazione e i
   loro permessi, allo scopo di permettere al Committente di amministrare l'applicazione e di permettere ai giocatori di
   tenere traccia dei propri progressi;
3. `Must-Have` **Sponsor Management**: gestire la pubblicità agli sponsor del progetto, allo scopo di permettere al
   Committente di adottare una nuova strategia di business aggiuntiva;
4. `Should-Have` **Tournament Management**: gestire la creazione, la configurazione e la partecipazione a dei tornei di
   scacchi, allo scopo di aumentare la visibilità e la popolarità dell'applicazione;
5. `Could-Have` **Statistics Management**: gestire il monitoraggio delle statistiche dei giocatori e una classifica
   globale, allo scopo di permettere ai giocatori di osservare la propria crescita nel tempo e di competere con altri
   giocatori;
6. `Could-Have` **Socialization Management**: gestire un sistema di amicizie e di comunicazione tra i giocatori
   nell'applicazione, allo scopo di permettere agli utenti di socializzare all'interno dell'applicazione, facilitando la
   creazione di una comunità di giocatori.

### Criteri di successo

- **Increased Revenue**:
    - Coprire i costi del progetto e trarre un profitto pari al 40% dei costi, entro i primi due anni dal deployment
      dell'applicazione.
- **Service Quality**:
    - La disponibilità del sistema deve essere tale da garantire l'accesso concorrente da parte di almeno 100000 utenti
      per il 95% del tempo in cui il sistema è online;
    - Il tempo medio di attesa tra una richiesta di un utente e la relativa risposta dal sistema dev'essere inferiore a
      200 millisecondi per l'80% dei casi e inferiore a un secondo per il 95% dei casi;
    - L'accessibilità dell'applicazione dev'essere almeno di livello AA, secondo lo standard WCAG 2.0, nell'intero sito
      web.

### Assunzioni e rischi principali

- Possibilità di riutilizzare alcuni dei requisiti dell'applicazione che il Committente ha già realizzato in passato;
- Possibilità di analizzare delle applicazioni concorrenti disponibili pubblicamente;
- Pochi competitori sul mercato;
- Flessibilità sul budget a disposizione per il progetto;
- Poca flessibilità sul tempo a disposizione per il progetto;
- Poca esperienza nella nuova strategia di business che il Committente vuole adottare;
- Rischio di non distinguersi abbastanza dalle applicazioni concorrenti;
- Rischio che le aziende concorrenti migliorino le proprie applicazioni prima del completamento di questo progetto;
- Rischio di non riuscire a generare sufficiente profitto tramite gli investimenti degli sponsor;
- Rischio dovuto all'incertezza sulle tecnologie da applicare per rendere l'applicazione scalabile;
- Rischio dovuto all'incertezza sulla domanda dell'applicazione al rilascio.

### Strategia

Per la gestione del progetto, si è adottato un PMLC Model di tipo incrementale, con una pianificazione preliminare molto
dettagliata e una sequenza di milestone da raggiungere durante lo sviluppo del progetto.

### Soluzione

Realizzare un'architettura che comprende i seguenti servizi:
- **Frontend Service**: servizio che si occupa della rappresentazione grafica dell'applicazione web e della
  sponsorizzazione da parte degli investitori esterni;
- **Backend Service**: servizio che gestisce l'inoltro delle richieste e delle connessioni dell'utente all'interno del
  sistema;
- **Authentication Service**: servizio che gestisce l'autenticazione e l'autorizzazione dei giocatori nell'applicazione.
- **Statistics Service**: servizio che si occupa della gestione delle statistiche dei giocatori, tenendo traccia del
  loro punteggio ELO e dei loro risultati nei tornei in cui hanno partecipato. Inoltre, gestisce la leaderboard
  dell'applicazione;
- **Notification Service**: servizio che gestisce la creazione, l'eliminazione e l'inoltro in tempo reale delle
  notifiche ai giocatori dell'applicazione;
- **Game Service**: servizio che si occupa della creazione, configurazione, partecipazione ed esecuzione delle partite
  di scacchi;
- **Tournament Service**: servizio che si occupa della creazione, configurazione, partecipazione ed esecuzione dei
  tornei di scacchi;
- **Friend Service**: servizio che si occupa della gestione delle amicizie tra i giocatori dell'applicazione, tenendo
  traccia delle richieste di amicizia pendenti oppure accettate;
- **Message Service**: servizio che si occupa dell'inoltro dei messaggi tra i giocatori amici nell'applicazione.

### Costi

| Categoria      | Importo     |
|----------------|-------------|
| Manodopera     | 50000$      |
| Strumentazione | 50000$      |
| Gestione       | 50000$      |
| Rischi         | 15000$      |
| Margine        | 30000$      |
| **Somma**      | **195000$** |

### Schedula

| Milestone         | Data di scadenza | Pagamento   |
|-------------------|------------------|-------------|
| Inizio progetto   | 20-02-2023       | 39000$      |
| Primo controllo   | 20-04-2023       | 39000$      |
| Secondo controllo | 20-06-2023       | 39000$      |
| Consegna progetto | 14-08-2023       | 78000$      |
| **Somma**         | **< 6 mesi**     | **195000$** |

### Svolgimento

La gestione dell'esecuzione del progetto è avvenuta principalmente attraverso la definizione di alcune regole operative,
in generale di carattere consultivo, e il monitoraggio tramite brevi meeting giornalieri e aggiornamenti settimanali dei
report del progetto.

### Conclusioni

Il progetto si è concluso con successo, soddisfacendo i criteri di successo e le Conditions of Satisfaction definite
assieme al Committente, ad eccezione di quelli per cui sarà necessario attendere un certo periodo di esecuzione del
sistema nell'ambiente di produzione.

In particolare, sono stati rispettati i tempi e i budget concordati con il Committente e si è fruttato un margine di
all'incirca 32000$ alla consegna del progetto.

### Retrospettiva

Il Project Manager ha leggermente sovrastimato i tempi ed i costi relativi ai rischi del progetto. Inoltre, sarebbe
stato più opportuno prevedere un maggior numero di milestone per controllare meglio le entrate durante lo svolgimento
del progetto.

### Contatti

- Committente: Claudio Rossi.
- Project Manager lato cliente: Paola Celeste.
- Project Manager lato fornitore: Pietro Magnolia.

### Allegati

- Conditions of Satisfaction: [link](/pm/attachments/content/cos)
- User Stories: [link](/pm/attachments/content/user-stories)
- Requirement Breakdown Structure: [link](/pm/attachments/content/rbs)
- SWOT Analysis: [link](/pm/attachments/content/swot-analysis)
- Work Breakdown Structure: [link](/pm/attachments/content/wbs)
- Analisi delle attività: [link](/pm/attachments/content/task-analysis)
- Matrice delle responsabilità: [link](/pm/attachments/content/responsibility-matrix)
- Analisi dei rischi: [link](/pm/attachments/content/risk-analysis)
- Analisi dei costi: [link](/pm/attachments/content/cost-analysis)
- Project Network Diagram: [link](https://miro.com/app/board/uXjVM9abzds=/?share_link_id=313338560385)
- Schedula: [link](https://app.asana.com/0/1204894076877574/1204894076877574)
- Work Packages: [link](/pm/attachments/content/work-packages)
- Rapporto Cumulativo - Schedula: [link](/pm/attachments/content/schedule-cumulative-report)
- Rapporto Cumulativo - Costo: [link](/pm/attachments/content/cost-cumulative-report)

---

[Back to Top](#top) |
[Previous Version](#14-08-2023)