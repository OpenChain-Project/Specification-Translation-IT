
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
