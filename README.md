#  Meteo App - Applicazione Meteo con Spring Boot

Meteo City è una semplice applicazione web sviluppata con **Spring Boot** che consente di visualizzare le temperature orarie di alcune città italiane tramite l’API di [Open-Meteo](https://open-meteo.com). Il progetto è contenuto all’interno di un'immagine Docker per una più facile esecuzione.

---

##  Funzionalità

- Homepage con elenco delle città disponibili
- API REST `/api/weather/{city}` per ottenere i dati meteo in formato JSON
- Integrazione con Open-Meteo
- Completamente eseguibile tramite Docker

---

##  Tecnologie Utilizzate

- Java 17
- Spring Boot
- Maven
- Docker
- Thymeleaf (per il frontend)

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

##  Come Avviare il Progetto

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
2. Avvio del container

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
