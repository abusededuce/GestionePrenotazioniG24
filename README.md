# Sistema di Prenotazione Aule Universitarie

Progetto per il corso di **Ingegneria del Software** (Università degli Studi di Salerno - DIEM).

## Struttura del Repository
* `docs/`: Documentazione di specifica dei requisiti e diagrammi dei casi d'uso.
* `src/main/java/`: Codice sorgente dell'applicazione.
* `src/test/java/`: Suite di unit test automatizzati (JUnit).

## Compilazione, Test e Documentazione

Il progetto utilizza **Apache Maven** (configurato per **Java 8**) per la gestione della build e dei test unitari, e **Doxygen** per la documentazione delle interfacce delle classi.

### Prerequisiti
* **JDK 8** (Il gruppo ha utilizzato: Azul Zulu JDK 8 FX: https://www.azul.com/downloads/?version=java-8-lts&package=jdk-fx#zulu)
* **Apache Maven**
* **Doxygen** (per generare la documentazione HTML)

### Comandi principali (da eseguire nella radice del progetto)

* **Compilare i file sorgente:**
  ```bash
  mvn compile
  ```

* **Compilare ed eseguire tutti gli unit test (JUnit 5):**
  ```bash
  mvn test
  ```

* **Creare il pacchetto eseguibile (`.jar` nella cartella `target/`):**
  ```bash
  mvn package
  ```

* **Pulire la cartella di build (rimuove `target/` e i file compilati):**
  ```bash
  mvn clean
  ```

* **Generare la documentazione delle classi (cartella `html/`):**
  ```bash
  doxygen Doxyfile
