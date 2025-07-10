#  Meteo App - Applicazione Meteo con Spring Boot

Meteo City è una semplice applicazione web sviluppata con **Spring Boot** che consente di visualizzare le temperature orarie di alcune città italiane tramite l’API di [Open-Meteo](https://open-meteo.com). Il progetto è contenuto all’interno di un'immagine Docker per una più facile esecuzione.

---

##  Funzionalità

- Homepage con elenco delle città disponibili
- API REST `/api/weather/{city}` per ottenere i dati meteo in formato JSON
- Integrazione con Open-Meteo
- Completamente eseguibile tramite Docker

---

##  Città visualizzate

- Roma
- Torino
- Napoli
- Milano
- Salerno
- Matinella

---

##  Tecnologie Utilizzate

- Java 17 : Linguaggio di programmazione principale.
- Spring Boot : Framework per lo sviluppo rapido dell'applicazione web.
- Maven : Strumento per la gestione del progetto e delle dipendenze.
- Docker : Per la containerizzazione dell'applicazione.
- Thymeleaf (per il frontend) : Motore di template per la generazione delle pagine HTML dinamiche.
- Chart.js : Libreria JavaScript per la creazione di grafici sul frontend.

---

##  Struttura Principale del Progetto

meteo/
├── src/
│ └── main/
│ ├── java/com/meteo/meteo/
│ │ ├── MeteoApplication.java
│ │ └── controller/WeatherController.java
│ └── resources/templates/index.html
├── pom.xml
├── Dockerfile
└── README.md

---

## Prerequisiti

Per poter utilizzare l'applicazione Meteo App, assicurati di avere Docker Desktop installato sul tuo computer.

##  Come Avviare il Progetto

###  Clona il progetto

```bash
git clone https://github.com/noemirenna/meteo-app.git

```
```bash
cd meteo-app
```
2. Costruisci l'immagine Docker
Apri il terminale nella cartella principale del progetto e digita:

```bash
docker build -t meteo-app .
```
3. Avvia il container Docker

```bash
docker run -p 8080:8080 meteo-app
```

## Come Avviare il Progetto

###  Clona il progetto

```bash
git clone https://github.com/noemirenna/meteo-app.git

```
```bash
cd meteo-app
```
Apri il terminale nella cartella principale del progetto e digita:

```bash
docker build -t meteo-app .
```

###  Costruzione e avvio del container

Con Docker Compose puoi costruire ed eseguire il progetto con un solo comando:

```bash
docker-compose up --build
```

L'app sarà disponibile su:

http://localhost:8080


---

## Autrice 

Noemi Renna
