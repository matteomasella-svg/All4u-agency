# Interfaccia Agenzia - All4U Talent Platform

Interfaccia interna per la creazione e gestione dei job post della piattaforma All4U Talent Platform.

## Funzione

Questa pagina consente allo staff di:

- creare nuove ricerche
- definire parametri interni del job
- impostare chiavi fondamentali e preferenziali
- generare l’annuncio pubblico per il candidato
- visualizzare una preview finale
- salvare il job post nel foglio Google `Job Posts`

## Obiettivo

Separare in modo chiaro:

- **criteri interni di selezione**, visibili solo lato agenzia
- **contenuti pubblici dell’annuncio**, visibili al candidato

## Funzionalità principali

### Informazioni base
- cliente
- progetto
- ruolo richiesto
- codice ricerca
- stato posizione
- area ammessa

### Parametri interni
- score minimo
- automunita obbligatoria
- altezza minima
- filtro età
- lingue richieste
- attestati obbligatori
- attestati preferenziali

### Must cliente
Selezione delle chiavi fondamentali che devono pesare maggiormente nella logica di scoring.

Esempi:
- CV obbligatorio
- automunita
- area compatibile
- esperienza minima
- altezza
- lingua straniera
- disponibilità weekend

### Preferenziali
Selezione degli elementi che aumentano il punteggio ma non rappresentano criteri principali.

Esempi:
- inglese
- esperienza eventi
- seniorità
- standing elevato

### Annuncio candidato
Generazione e modifica dei campi pubblici:
- titolo annuncio
- testo annuncio
- zona lavoro pubblica
- requisiti pubblici
- documenti richiesti
- stato pubblicazione

### Preview pubblica
Anteprima finale della vista che sarà mostrata al candidato.

## Integrazione backend

La pagina invia i dati al backend Google Apps Script tramite endpoint Web App.

Esempio:

```javascript
const APPS_SCRIPT_URL = "YOUR_APPS_SCRIPT_WEBAPP_URL";
