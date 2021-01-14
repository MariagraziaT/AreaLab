# Architettura

## Features
Nel progetto sono richieste le seguenti features:
- Connessione a un database: Dal quale il programma seleziona o inserisce dei particolari dati;
- Interfaccia grafica: Necessaria per interagire con il programma e contenente tutte le funzioni che esso può compiere;
- Impostazioni: Il programma deve essere personalizzabile tramite delle impostazioni (salvate in DB / scritte su file) (Aggiungere 1/+ Corsi) (Modificare impostazioni corso);
- Log: Questa funzionalità e strettamente necessaria per tenere traccia delle attività dell'utente, nonchè dei possibili crash a cui il programma potrebbe andare in contro;

## Entità
- Scuole: Ogni scuola è un'entità essendo che il programma e pensato per soddisfare le esigenze di più scuole; (personalizzabile nelle impostazioni?);
- Plessi: Ogni scuola è composta da uno (ex. Marconi) o più plessi (ex: IT13);
- Professori: Persona che lavora in un determinato plesso (molti a molti oppure uno a molti??);
- Corso: Seguito da un professore (trovare tutte le variabili che potrebbe contenere!);
EX 1:
Scuole (IDScuola, denominazione) -> Plessi (IDPlesso, denominazione, locazione) -> Professori (IDProfessore, guarda docx) -> Attestato (tipo -base/specifico/agg durata -ore)
EX 2:
Scuole(IDScuola, denominazione) -> COMPRENDE -> Plessi (IDScuola, IDPlesso, denominazione, locazione) -> LAVORA IN (n,n oppure 1,n?) -> Professori (IDProfessore, ...) -> POSSIEDE -> Attestato (IDProfessore, tipo -base/specifico/agg durata -ore)
