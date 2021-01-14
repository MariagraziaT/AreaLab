# Architettura

## Features
Nel progetto sono richieste le seguenti features:
* Interfaccia grafica
  * Necessaria per interagire con il programma
* 

Scuole (IDScuola, denominazione) -> Plessi (IDPlesso, denominazione, locazione) -> Professori (IDProfessore, guarda docx) -> Attestato (tipo -base/specifico/agg durata -ore)
--------------------------------------------------------------------------------------------------------------------------
Scuole(IDScuola, denominazione) -> COMPRENDE -> Plessi (IDScuola, IDPlesso, denominazione, locazione) -> LAVORA IN (n,n oppure 1,n?) -> Professori (IDProfessore, ...) -> POSSIEDE -> Attestato (IDProfessore, tipo -base/specifico/agg durata -ore)

(Devono essere previste delle impostazioni per la gestione delle ore da fare)
(Deve essere previsto un meccanismo di log)
