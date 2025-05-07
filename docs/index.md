# Documentazione Cinemille

## Panoramica del Progetto

Il progetto è stato realizzato con:

- **Backend**: Spring Boot, Spring Security, JPA/Hibernate
- **Frontend**: Angular 19 + Angular Material
- **Database**: PostgreSQL
- **VCS**: Git
- **IDE**: IntelliJ

L'applicazione permette visualizzare una lista completa delle programmazioni, oppure solo la lista dei film in programmazione nella settimana attuale,  in base al ruolo dell'utente/servizio.

## Struttura del Progetto

Il progetto è organizzato con una struttura Maven:

```
cinemille/
├── backend/         # Spring Boot
└── frontend/        # Angular
```
Per una spiegazione più dettagliata, vedere la sezione "Architettura"

## Funzionalità Principali

- **Autenticazione**: Sistema di autenticazione basato su JWT
- **Lista Film**: Storico completo delle programmazioni dei film nelle varie sale
