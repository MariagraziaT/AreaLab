# Architettura

<!-- (immagine architettura) -->

## :clipboard: Descrizione
Per sviluppare questa applicazione, la quale descrizione è presente (qui)[DescrizioneProgetto.md], sono presenti piò possibilità. <br>
Quella pensata dal nostro gruppo adotta due aspetti principali: un database, un programma java che si interfaccia con esso. <br>
L'utilizzo di un server web è stato escluso, essendo che complicherebbe le cose a entrambe le parti, sia ai programmatori che a chi riceve il progetto.

## :gear: Features
Nel progetto sono richieste le seguenti features:
- Meccanismo di autenticazione: per eseguire l'accesso al programma;
- Connessione a un database: Dal quale il programma seleziona o inserisce dei particolari dati;
- Interfaccia grafica: Necessaria per interagire con il programma e contenente tutte le funzioni che esso può compiere;
- Impostazioni: Il programma deve essere personalizzabile tramite delle impostazioni (salvate in DB / scritte su file) (Aggiungere 1/+ Corsi) (Modificare impostazioni corso);
- Log: Questa funzionalità e strettamente necessaria per tenere traccia delle attività dell'utente, nonchè dei possibili crash a cui il programma potrebbe andare in contro;

## :busts_in_silhouette: Entità
- Scuole: Ogni scuola è un'entità essendo che il programma e pensato per soddisfare le esigenze di più scuole; (personalizzabile nelle impostazioni?);
- Plessi: Ogni scuola è composta da uno (ex. Marconi) o più plessi (ex: IT13);
- Professori: Persona che lavora in un determinato plesso (molti a molti oppure uno a molti??);
- Corso: Seguito da un professore (trovare tutte le variabili che potrebbe contenere!);

## 📖 :book: Tabelle
- Scuole: IDScuola, denominazioneScuola
- Plessi: IDScuola, IDPlesso, denominazionePlesso, indirizzoPlesso
- Lavori: IDScuola, IDProfessore
- Professori: IDProfessore, nome, cognome, dataNascita
- Corso: IDProfessore, tipologia, durata, dataCorso, note

## :pushpin: Nello specifico
- Per quanto riguarda il database si prevede l'utilizzo di MySql, software reperibile gratuitamente.
- Per quanto riguarda la programmazione, invece, il linguaggio di programmazione utilizzato sarà Java.
