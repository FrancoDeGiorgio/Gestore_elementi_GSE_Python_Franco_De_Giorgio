# 🌿 LookBook
> *Un nuovo modo di dare vita ai vestiti dimenticati*

![LookBook Logo](https://raw.githubusercontent.com/FrancoDeGiorgio/Gestore_elementi_GSE_Python_Franco_De_Giorgio/49d7c9e3b07d8d0822a76feea3c9f863ebda6242/Logo%20Ecologico%20LookBook.png)

## 💡 Da dove nasce l'idea

Vendere e comprare vestiti usati può essere complicato, tanto che spesso si rinuncia per frustrazione. 

I fondatori di LookBook hanno vissuto questa difficoltà in prima persona e hanno deciso di creare un sistema più semplice e veloce per dare nuova vita ai capi.

## 🌟 Vision
> ♻️ **Normalizzare l'utilizzo dell'abbigliamento second-hand, dando una seconda vita a ogni capo dimenticato nell'armadio.**

## 🧭 Mission
> Promuovere un modello di consumo sostenibile e diffondere la cultura del riuso come scelta consapevole per il pianeta.

## 👥 Chi siamo

I fondatori di LookBook sono tre ex professionisti del settore del fast fashion che da un paio d'anni hanno deciso di cambiare rotta. 

Il loro obiettivo è rivoluzionare il concetto di second-hand, allontanandolo dai pregiudizi che lo vedono come qualcosa di poco attraente, fuori moda o legato solo al risparmio.

Per LookBook, l'abbigliamento di seconda mano significa:
- Qualità
- Funzionalità
- Sostenibilità

LookBook vuole dare una seconda vita a capi belli, funzionali e a volte in molti casi praticamente nuovi, perché acquistati d'impulso e mai indossati.

## ⚙️ Come funziona

Dopo aver scaricato l'app, gli utenti possono caricare le foto dei capi che desiderano vendere direttamente sul proprio profilo personale. L'app fornisce una stima del prezzo medio di vendita in base alle caratteristiche del capo.

L'app offre anche l'opzione **Swap**, che permette di scambiare un capo con un altro utente, a condizione che entrambe le parti accettino la proposta.

*Il servizio è attualmente disponibile in tutta Italia.*

Per chi desidera donare i propri vestiti, è disponibile una lista di Onlus partner che raccolgono indumenti da destinare a persone in difficoltà.

---

## 🎯 Obiettivo del Progetto

Realizzare un'applicazione Python (su Jupyter Notebook) per gestire un catalogo di vestiti second-hand caricati dagli utenti, con funzioni base e avanzate, simulando il backend di LookBook.

## 📋 Analisi dei Requisiti

### Funzionalità base:
- ✅ Inserimento nuovi capi (nome, marca, taglia, colore, prezzo, condizione, categoria, disponibilità)
- ✅ Visualizzazione capi presenti in catalogo
- ✅ Modifica dati di un capo già inserito
- ✅ Eliminare capi presenti
- ✅ Ricerca di capi (tramite criterio testuale)
  

### Funzionalità avanzate:
- 🔍 **Filtraggio avanzato**
  - Solo capi "nuovi"
  - Solo "marca X"
  - Solo "per scambio"
  - Per fascia di prezzo
  - ecc.

- 💰 **Stima prezzo medio dinamica**
  - In base ad attributi ( condizione + categoria)

- 📊 **Statistiche**:
  - Numero capi per categoria
  - Percentuale per condizioni
  - Percentuali disponibilità

## 🗂️ Struttura dei Dati

### Attributi di ogni capo:
| Attributo | Descrizione |
|-----------|-------------|
| `id` | Univoco, generato automaticamente |
| `nome` | Nome del capo |
| `marca` | Brand del capo |
| `taglia` | Taglia del capo |
| `colore` | Colore principale |
| `prezzo` | Prezzo |
| `condizione` | Nuovo, usato, ecc. |
| `categoria` | T-shirt, pantalone, scarpe, ecc. |
| `modalità_disponibilità` | Vendita, scambio, donazione |

### Rappresentazione:
- **Lista di dizionari** 

## 🛣️ Roadmap di sviluppo

| Fase | Descrizione | Priorità |
|------|-------------|----------|
| 1 | Strutturazione dei dati (dizionari) | Alta |
| 2 | Funzioni base (inserimento, visualizzazione, modifica, ecc) | Alta |
| 3 | Funzioni avanzate (filtri avanzati) | Media |
| 4 | Stima prezzo media dinamica | Media |
| 5 | Statistiche sui capi | Bassa |

## 📑 Organizzazione Notebook:

- 📄 **Introduzione** (descrizione progetto)
- 🛠️ **Setup** (inizializzazione dati)
- ✍️ **Funzioni Base**
- 🔍 **Funzioni Avanzate**
- 📊 **Statistiche**
- 🚀 **Testing finale** (esempi pratici d'uso delle funzioni)

## 📚 Dettaglio Funzioni da Progettare

| Nome Funzione | Cosa farà |
|---------------|-----------|
| `insert_capo()` | Inserisce un nuovo capo nella lista globale |
| `genera_id()` | Genera un ID incrementale per i capi inseriti |
| `view_capi()` | Visualizza tutti i capi registrati |
| `stampa_tabella_capi()` | Visualizza in capi in formato tabella |
| `modifica_capo()` | Permette di modificare i dati di un capo tramite il suo ID |
| `elimina_capo()` | Inserisce un nuovo capo nella lista globale |
| `ricerca_capo()` | Cerca capi tramite criteri testuali |
| `filtra_capi()` | Filtra capi secondo criteri avanzati (es: solo "nuovi", solo "scambio", fascia di prezzo) |
| `statistiche_capi()` | Raccoglie statistiche generali: numero capi, per tipologia, per stato d'uso, prezzo medio |
| `stima_prezzo()` | Stima il prezzo medio di un capo basandosi su attributi categoria e condizione  |
| `view_carrello()` | Visualizza il carrello e il totale in € |
| `menu_carrello()` | Gestisce il sotto menù carrello |
| `aggiungi_al_carrello()` | Aggiunge elemento al carrello |
| `rimuovi_dal_carrello()` | Rimuove elemento al carrello |
| `svuota_carrello()` | Rimuove tutti gli elementi dal carrello |
| `menu_principale()` | Visualizza menù principale |
| `main()` | Gestisce il menù principale 
| `funzioni_avanzate()` | Gestisce sotto menù avanzate |


## 🔄 Dettaglio Flusso Utente

1. **Avvio programma** → Messaggio di benvenuto
2. **Menu principale** → L'utente sceglie l'azione:
   - Inserisci un nuovo capo
   - Visualizzare tutti i capi
      - Aggiungi al carrello
   - Modificare un capo
   - Elimina capi
   - Cercare un capo
      - Aggiungi al carrello
   - Funzioni avanzate (filtri, stima prezzi, statistiche)
      - Ricerca tramite filtri
         - Aggiungi al carrello
      - Statistiche generali
      - Torna al menù principale
   - Visualizza carrello
3. **Esecuzione** della funzione scelta
4. **Tornare** al menu principale o uscire
