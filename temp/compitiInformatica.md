# Progetto Palestra [Compiti vacanze Natale 2019]

Realizzato da D'Onofrio Alessandro

## Sommario

1. [Progetto Concettuale]()  
    1.1 Analisi  
    1.2 Diagramma ER  
    1.3 Documentazione diagramma  
2. [Progetto Logico]()  
    2.1 Schema relazionale  
    2.2 Istanze del DB  

## Progetto Concettuale

### 1.1 _Analisi_

* Per identificare i tipi di abbonamento userò 2 variabili booleane per indicare accesso a sala pesi e corsi
* Ogni utente può consegnare più certificati medici
* Per ogni certificato medico sarà registrato proprietario e data di scadenza
* Le SchedeAllenamento saranno comprese di variabile booleana per segnare l'attività della scheda (possono esserci più schede nel tempo per ogni membro)
* Ogni scheda contiene almeno un set di esercizi (allenamento) ma gli allenamenti possono comparire in più schede
* Uso l'entità attrezzo per arricchire il corso comunicando quali attrezzi verranno usati per ogni esercizio

### 1.2 _Diagramma ER_

### 1.3 _Documentazione Diagramma_

## 2. Progetto Logico

### 2.1 _Schema Relazionale_

* **CertificatoMedico**(<u>codiceCliente</u>, <u>scadenza</u>)  
    > **codiceCliente** ha un vincolo di integrità referenziale con **codice** di **Cliente**

* **Cliente**(<u>codice</u>, codiceAbbonamento, cognome, nome, dataNascita, luogoNascita, recapito, email, numeroTelefono)
    > **codiceAbbonamento** ha un vincolo di integrità referenziale con **codice** di **Abbonamento**

* **Abbonamento**(<u>codice</u>, scadenza, salaPesi, corsi)

* **Corso**(<u>codice</u>, descrizione)

* **Partecipazione**(<u>codiceCorso</u>, <u>codiceAbbonamento</u>)
    > **codiceCorso** ha un vincolo di integrità referenziale con **codice** di **Corso**
    > **codiceAbbonamento** ha un vincolo di integrità referenziale con **codice** di **Abbonamento**

* **Attrezzo**(<u>codice</u>, nome)

* **Utilizzo**(<u>codiceCorso</u>, <u>codiceAttrezzo</u>)
    > **codiceCorso** ha un vincolo di integrità referenziale con **codice** di **Cliente**
    > **codiceAttrezzo** ha un vincolo di integrità referenziale con **codice** di **Attrezzo**

* **Sala**(<u>codice<u>)

* **SvolgimentoCorso**(<u>codiceCorso</u>, <u>codiceSala</u>, giorno, oraInizio, oraFine)
    > **codiceCorso** ha un vincolo di integrità referenziale con **codice** di **Corso**
    > **codiceSala** ha un vincolo di integrità referenziale con **codice** di **Sala**

* **Scheda**(<u>codice</u>, data, obiettivo, difficoltà, attivo, codiceAbbonamento)
    > **codiceAbbonamento** ha un vincolo di integrità referenziale con **codice** di **Abbonamento**

* **Esercizio**(<u>codice</u>, descrizione, peso, ripetizioni)

* **PraticaSchedaEsercizio**(<u>codiceScheda</u>, <u>codiceEsercizio</u>, numeroOrdine)
    > **codiceScheda** ha un vincolo di integrità referenziale con **codice** di **Scheda**
    > **codiceEsercizio** ha un vincolo di integrità referenziale con **codice** di **Esercizio**

### 2.2 _Istanze del DB_
