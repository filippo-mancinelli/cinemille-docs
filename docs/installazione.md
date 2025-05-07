# Guida all'avvio

## Prerequisiti

- Java 17 o superiore
- Node.js 20 o superiore
- Docker e Docker Compose (opzionale, se desideri utilizzare un tuo DB in locale)
- PostgreSQL (se non si utilizza Docker)
- Git

## Clonazione del Repository

```bash
git clone https://github.com/tuaorganizzazione/cinemille.git
cd cinemille
```

## Configurazione del Backend

### 1. Configurazione del Database

#### Utilizzando Docker (consigliato per lo sviluppo)

Il progetto include già un file `compose.yaml` per avviare PostgreSQL in un container:

```bash
cd backend
docker-compose up -d
```

#### Utilizzando un Database PostgreSQL esistente

Crea un database chiamato `cinemille`:

```sql
CREATE DATABASE cinemille;
```

### 2. Configurazione delle Variabili d'Ambiente

Crea un file `.env` nella cartella `backend` con le seguenti variabili:

```
DB_URL=jdbc:postgresql://localhost:5432/cinemille
DB_USER=cineuser
DB_PASSWORD=cinepassword
```

Modifica i valori in base alla tua configurazione.

### 3. Compilazione e Avvio del Backend

```bash
cd backend