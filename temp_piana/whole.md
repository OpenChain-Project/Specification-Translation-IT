
# Introduzione

L'iniziativa "OpenChain" iniziò nel 2013 quando un gruppo di operatori impegnati nella _supply chain_ del software open source osservò l'insorgenza di due tendenze:

  * esistevano significative similitudini tra organizzazioni con programmi maturi di _compliance_ open source; e
  * permaneva un ampio numero di organizzazioni che scambiavano software con programmi meno evoluti.

 Dalla seconda osservazione scaturiva una mancanza di fiducia nella uniformità e qualità dei risultati in termini di compliance che si accompagnavano al software così scambiato. Come conseguenza, a ogni passaggio nella catena di fornitura, le organizzazioni a valle si trovavano frequentemente a compiere nuovamente gli sforzi di _compliance_ già eseguiti da altre organizzazioni a monte.

Fu formato un gruppo di studio al fine di considerare se potesse essere creato un programma di specifiche standardizzate che

  * facilitasse più alta qualità e uniformità delle informazioni sulla _compliance_ open source che si scambiavano all'interno dell'industria; e
  * diminuisse gli elevati costi di transazione associati all'open source risultante dal rifacimento della _compliance_.

Il gruppo di studio evolvette in un gruppo di lavoro e, in aprile 2016 venne formalmente organizzato come un progetto collaborativo della Linux Foundation.

La Visione e la Missione dell'OpenChain Initiative sono le seguenti:

  * Visione: una _supply chain_ dove il software libero/open source (FOSS) fosse trasmesso con informazioni sulla compliance affidabili e uniformi.
  * Missione: stabilire requisiti per ragiungere una gestione efficiente del software libero/open source (FOSS) per i partecipanti alla _supply chain_ del software, in modo che tali requisiti e [`associated collateral`] siano sviluppati in modo collaborativo e aperto da rappresentanti della _supply chain_ del software, dalla comunità open source e dal mondo accademico.

In coerenza con la Visione e la Missione, queste specifiche definiscono un insieme di requisiti che, se rispettati, incrementerebbero significativamente la probabilità che un programma di _compliance_ open source abbia raggiunto un sufficiente livello di qualità, uniformità e completezza; ciononostante, un programma che soddisfi tutte i requisiti delle specifiche non garanisce una piena _compliance_. I requisiti rappresentano un insieme di livello base (minimo) di requisiti che un programma deve rispettare per essere considerato essere conforme con OpenChain. Le specifiche si focalizzano sulle qualità "cosa" e "perché" di un programma di _compliance_, in contrapposizione a considerazioni sul  "come" e sul "perché". [ `<!-- FIXME --> ` `il tutto è un po' oscuro anche in inglese`]. Ciò assicura un livello pratico di flessibilità che permette a diverse organizzazioni di confezionare su misura le proprie procedure e processi per adattarsi megliio ai propri obiettivi.

La Sezione 2 `<!-- FIXME verificare se non sia capitolo o articolo--> ` introduce definizioni dei termini chiave usati all'interno delle specifiche. La Sezione 3 presenta i requisiti delle specifiche dove ciascuna ha una lista di uno o più Prodotti di Verifica. Essi rappresentano la prova che deve sussistere al fine di considerare un dato requisito soddisfatto. Se tutti i requisiti sono stati rispettati per un dato programma, esso viene considerato OpenChain Conforming <!-- FIXME lo terrei non tradotto --> nel rispetto della versione 1.1 delle specifiche. I prodotti di Verifica non sono pubblici, ma possono essere forniti sotto NDA o su richiesta confidenziale da parte di un'organizzazione OpenChain <!-- FIXME  confrontarsi con Shane, che cavolo vuol dire questa parte qui, non è chiaro -->  per validare la conformità.

# Definizioni

FOSS (Free and Open Source Software)
:    Software sottoposto a una o più licenze che rispettano la Open Source Definition, pubblicat dalla Open Source Initiative (OpenSource.org) o la Free Software Definition (pubblicata dalla Free Software Foundation) o licenze simili.

Contatti FOSS <!-- Nota, anche questo è stato modificato rispetto all'ultima verisione -->
:    Una persona designata a ricevere [`domande | richieste di informazioni` `<!-- FIXME scegliere -->` ] circa il FOSS.

Licenze identificate
:    Un insieme di licenze FOSS identificate a seguito dell'applicazione di un metodo appropriato di identificazione di tali licenze.` <!-- FIXME E che cazz'è? --> `

Conforme a OpenChain [`Oppure "OpenChain-conforme?" `]
:    un programma che soddisfi tutti i requisiti di questa specifica.

Staff del Software <!-- attenzione, modificata rispetto precedente versione -->   
:    un dipendente o un appaltatore che definisce, contribuisce a o ha responsabilità circa la preparazione di Software fornito. A seconda dell'organizzazione, ciò potrebbe includere (ma non si limita a) sviluppatori software, specialisti del rilascio, responsabili della qualità, [`product marketing e product management` `<!-- FIXME come tradurre questa roba? Ha senso? --> `]

SPDX o Software Package Data Exchange
:    il formato standard creato dall'SPDX Working Group per lo scambio di informazioni di licenza e copyright circa un determinato pacchetto software. Una descrizione delle specifiche SPDX può essere reperita a http://www.spdx.org `<!-- FIXME sengnalare che gli URL vanno sempre identificati con il protocollo! -->`

Software Fornito <!-- supplied software nell'originale  -->
:    software che un'organizzazione fornisce a terze parti (per esempio, a un'altra organizzazione o a un'altra persona)

Prodotti di Verifica
:    prove che debbono esistere al fine di considerare soddisfatto un determinato requisito.

# Requisiti

## Conosci le tue responsabilità in materia di FOSS
---------------------------------------------------------------------------------------------------------------------------------

### **Esiste una policy FOSS interna, la quale regola il rispetto delle licenze FOSS nella distribuzione del Software Fornito.** La Policy deve essere comunicata internamente.

#### Prodotti di Verifica

* Esistenza di una policy FOSS scritta
* Esistenza di Una procedura documentata che renda tutto lo Staff del Software informato dell'esistenza di una policy FOSS (per esempio, tramite formazione, un wiki interno, ovvero altri metodi di comunicazione).

#### Razionale

> Assicurare che passi `[necessari?]` siano stati intrapresi per creare, registrare e rendere lo Staff del Software informato dell'esistenza di una policy FOSS. Sebbene qui non sono forniti requisiti su cosa debba essere incluso in tale policy, altre sezioni potrebbero imporre requisiti sulla policy.

<!-- nuovo paragrafo (duplicare) -->
### Esiste un aggiornamento FOSS obbligatorio per tutto lo Staff del Software, tale per cui:
- **Il training, come minimo, copra le seguenti aree:**

    - La policy FOSS e dove reperire una copia;
    - Fondamenti del diritto della proprietà industriale attinente al FOSS e alle licenze FOSS;
    - I concetti del licensing FOSS (inclusi i concetti di licenze permissive e copyleft);
    - I modelli di licenza del FOSS;
    - Ruoli e responsabilità dello Staff Software riguardo specificamente alla compliance FOSS e in generale alla policy FOSS; e
    - Processi per identificare, registrare e/o tenere traccia di componenti FOSS contenuti nel Software Fornito.

- Lo Staff Software deve aver completato un aggiornamento FOSS nei 24 mesi (per essere considerato aggiornato). Un test può essere impiegato per consentire allo Staff Software di soddisfare il requisito di aggiornamento.

#### Prodotti di Verifica

* Esiste materiale di aggiornamento FOSS che copra le aree di cui sopra (per esempio, set di slide, corsi online o altro materiale di aggiornamento).
* Un metodo per tenere traccia del completamento dell'aggiornamento per tutto lo Staff Software.
* Almeno l'85% dello Staff Software è aggiornato, come da definizioni nella sezione superiore.

#### Razionale

> Assicurare che lo Staff Software abbia recentemente partecipato a un aggiornamento FOSS e che un insieme fondamentale di argomenti FOSS siano stati affrontati. L'intento è di assicurare che un livello di base fondamentale di argomenti siano stati affrontati, ma un programma di aggiornamento tipico sarebbe verosimilmente più ampio di quanto qui è richiesto.

### Esiste un processo per esaminare le Licenze Identificate per determinare le obbligazioni, le restrizioni e i diritti conferiti da ciascuna licenza.

#### Prodotti di Verifica

* Esistenza di una procedura documentata per la revisione e la documentazione delle obbligazioni, delle restrizioni e dei diritti conferiti da ciascuna Licenza Identificata che regoli il Software Fornito.

#### Razionale

> Assicurare l'esistenza di una procedura documentata per la revisione e la documentazione delle obbligazioni, delle restrizioni e dei diritti conferiti da ciascuna Licenza Identificata per le varie ipotesi d'uso.

## Assegna responsabilità per raggiungere la compliance

### Identifica le Funzioni di coordinamento esterno del FOSS ("Contatti FOSS")

* Nomina i soggetti responsabili per ricevere domande esterne sul FOSS;
* I Contatti FOSS devono intraprendere sforzi commercialmente ragionevoli per rispondere appropriatamente alle richieste circa la compliance FOSS; e
* Identificare pubblicamente un mezzo tramite il quale si possa contattare il Contatto FOSS.

#### Prodotti di Verifica

- Identificazione pubblica della funzione di Contatto FOSS (per esmepio, tramite un indirizzo email pubblicizzato, o la Open Compliance Directory della Linux Foundation).
- Esistenza di una procedura interna documentata che assegni le responsabilità per ricevere richieste circa la compliance FOSS.

#### Razionale

> Assicurare che vi sia un modo ragionevole per i terzi di contattare l'organizzazione per domande circa la compliance FOSS e che questa responsabilità sia stata effettivamente assegnata.

### Identifica i ruoli interni di compliance FOSS

* Nomina i soggetti responsabili per gestire la compliance FOSS interna. Il ruolo circa la compliance FOSS interna e il ruolo di Contatto FOSS possono coesistere nella stessa persona.
* L'attività di gestione della compliance FOSS è dotata di sufficienti risorse:
    * Il tempo per svolgere le funzioni del ruolo è stato allocato; e
    * Un budget commercialmente ragionevole è stato assegnato.
* Assegna responsabilità di sviluppare e manutenere le policy e i processi FOSS;
* Competenze legali circa la compliance FOSS sono accessibili ai ruoli di compliance FOSS (potrebbero essere risorse interne o esterne); e
* Esiste un processo per la risoluzione di questioni di compliance FOSS.

#### Prodotti di Verifica

- I nomi delle persone, gruppi o fuznioni nei ruoli di compiance FOSS identificati internamente.
- L'identificazione di risorse di competenza legale disponibili alle funzioni di compliance FOSS, che possono essere interne o esterne.
- Esistenza di una procedura identificata per asegnare responsabilità interne per la compliance FOSS.
- Esistenza di una procedura documentata per gestire la revisione di casi di mancata conformità e porvi rimedio.

#### Razionale

> Assicurare che le responsabilità FOSS siano effettivamente assegnate.

<!-- FIXME continuare con il resto  -->
