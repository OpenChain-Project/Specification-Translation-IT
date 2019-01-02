---
title: Specifica openchain
numberSections: true
sectionsDepth: 3
secPrefixTemplate: "\\[p\\]&nbsp;\\[i\\]"
---


Versione 1.2

*This file serves as a template to facilitate the translation of the
OpenChain specification from English to other languages. The OpenChain
project designates one official translation per language lead by an
approved maintainer. Only official translations are allowed to use the
OpenChain logo and trademark as they appear in this template. For more
details about the translation policy and process please visit: *

[*https://wiki.linuxfoundation.org/openchain/spec-translations*](https://wiki.linuxfoundation.org/openchain/spec-translations)


## Contents {- label="content"}


<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=2 orderedList=false} -->
<!-- code_chunk_output -->

	* [Contents](#contents)
* [Introduzione](#introduzione)
* [Definizioni](#definizioni)
* [Requisiti](#requisiti)
	* [Obiettivo 1: Conosci le Tue Responsabilità FOSS](#obiettivo-1-conosci-le-tue-responsabilità-foss)
	* [Obiettivo 2: Assegna Responsabilità per Conseguire Conformità](#obiettivo-2-assegna-responsabilità-per-conseguire-conformità)
	* [Obiettivo 3: Verifica e Approva il Contenuto FOSS](#obiettivo-3-verifica-e-approva-il-contenuto-foss)
	* [Obiettivo 4: Consegna la Documentazione e gli Elaborati del Contenuto FOSS](#obiettivo-4-consegna-la-documentazione-e-gli-elaborati-del-contenuto-foss)
	* [Obiettivo 5: Comprendere il Coinvolgimento della Comunità FOSS](#obiettivo-5-comprendere-il-coinvolgimento-della-comunità-foss)
	* [Obiettivo 6: Certificare l\'Adesione ai Requisiti OpenChain](#obiettivo-6-certificare-ladesione-ai-requisiti-openchain)
* [Appendice I: Traduzioni](#appendice-i-traduzioni)

<!-- /code_chunk_output -->

> This is an official translation from the OpenChain Project. It has been
translated from the original English text. In the event there is
confusion between this translation and the English version, The English
text shall take precedence.

> Questa è una traduzione ufficiale del progetto OpenChain. Il testo è
stato tradotto dall'originale inglese. Nel caso in cui vi sia ambiguità
tra questa traduzione e la versione Inglese, il testo inglese prevale.

---

Copyright © 2016-2018 Linux Foundation. Questo documento è concesso in
licenza secondo I termini della licenza Creative Commons Attribuzione
4.0 Internazionale (CC-BY 4.0). Una copia della licenza è reperibile
presso <https://creativecommons.org/licenses/by/4.0/>.

---

# Introduzione

L\'OpenChain Initiative ebbe inizio nel 2013 quando un gruppo di
operatori impegnati nella filiera di approvvigionamento del software
open source osservò l\'insorgenza di due tendenze: 1) esistevano
significative similitudini tra organizzazioni con programmi di
conformità open source maturi; e 2) permaneva un ampio numero di
organizzazioni che scambiavano software con programmi meno evoluti.
Dalla seconda osservazione scaturiva una mancanza di fiducia nella
uniformità e qualità degli Elaborati di Conformità che accompagnavano il
software così scambiato. Come conseguenza, a ogni passaggio nella catena
di fornitura, le organizzazioni a valle si trovavano frequentemente a
compiere nuovamente le attività di valutazione della conformità già
eseguite da altre organizzazioni a monte.

Fu formato un gruppo di studio al fine di considerare se potesse essere
creato una specifica di programma standard che potesse: i) facilitare
una più alta qualità e uniformità delle informazioni sulla conformità
open source che si scambiavano all\'interno dell\'industria; e ii)
diminuire gli elevati costi di transazione associati all\'open source
risultante dal rifacimento della conformità. Il gruppo di studio
evolvette in un gruppo di lavoro e, in aprile 2016 venne formalmente
organizzato come un progetto collaborativo della Linux Foundation.

La Visione e la Missione dell\'OpenChain Initiative sono le seguenti:

-   **Visione**: Una filiera di approvvigionamento nella quale il
    software libero/open source (FOSS) sia trasmesso con informazioni
    sulla conformità affidabili e uniformi.
-   **Missione**: stabilire i requisiti per conseguire una gestione
    efficiente del software libero/open source (FOSS) per i partecipanti
    alla filiera di approvvigionamento del software, in modo tale che i
    requisiti e il relativo materiale di supporto siano sviluppati in
    modo collaborativo e aperto da rappresentanti della filiera di
    approvvigionamento del software, della comunità open source e del
    mondo accademico.

In coerenza con la Visione e la Missione, questa specifica definisce un
insieme di requisiti che, se rispettati, incrementerebbero
significativamente la probabilità che un programma di conformità open
source abbia raggiunto un sufficiente livello di qualità, uniformità e
completezza; ciononostante, un programma che soddisfi tutti i requisiti
della specifica non garantisce una piena conformità. I requisiti
rappresentano un insieme di requisiti di livello base (minimo) che un
programma deve rispettare per essere considerato di Conformità a
OpenChain. La specifica si focalizza sul \"cosa\" e sul \"perché\" di un
programma di conformità, in contrapposizione a considerazioni sul
\"come\" e sul \"quando\". Ciò assicura un livello pratico di
flessibilità che permette a diverse organizzazioni di confezionare su
misura le proprie procedure e i propri processi per meglio adattarsi ai
propri obiettivi.

Il Capitolo 2 introduce le definizioni dei termini chiave usati
all\'interno della specifica. Il Capitolo 3 presenta i requisiti della
specifica dove ciascuno ha una lista di uno o più Materiali di Verifica.
Essi rappresentano la prova che deve sussistere al fine di considerare
un dato requisito soddisfatto. Se tutti i requisiti sono stati
rispettati per un dato programma, esso viene considerato di Conformità a
OpenChain nel rispetto della versione 1.2 della specifica. I Materiali
di Verifica non è previsto che siano pubblici, ma possono essere forniti
secondo un accordo di riservatezza o in base a una richiesta
confidenziale da parte dell'organizzazione OpenChain per validare la
conformità.

Ulteriori chiarimenti su come interpretare la specifica possono essere
ottenuti esaminando le Domande Frequenti (FAQ) sulla Specifica
disponibili all\'indirizzo:
<https://www.openchainproject.org/specification-faq>

# Definizioni

**Elaborati di Conformità**
:   una raccolta di elaborati che rappresentano il risultato del programma di
gestione FOSS per una versione del Software Fornito. La raccolta può includere
(ma non è limitata a) uno o più dei seguenti: codice sorgente, note di
attribuzione, note di diritto d'autore, copia delle licenze, notifiche di
modifica, offerte scritte, distinta dei materiali del componente FOSS, documenti
SPDX e così via.

**FOSS** (Free and Open Source Software)
:   software sottoposto a una o più licenze che rispettano la Open Source
Definition, pubblicata dalla Open Source Initiative (OpenSource.org) o la Free
Software Definition (pubblicata dalla Free Software Foundation) o licenze
simili.

**Contatto FOSS**
:   una persona designata a ricevere richieste esterne
di informazioni circa il FOSS.

**Licenze identificate**
:   un insieme di licenze FOSS identificate a seguito dell\'applicazione di un
metodo appropriato di identificazione delle licenze che regolano il Software
Fornito.

**Programma di Conformità OpenChain**
:   un programma che soddisfa tutti i requisiti di questa specifica.

**Personale del Software**
:   un dipendente o un appaltatore che definisce, contribuisce a o ha responsabilità
circa la preparazione di Software Fornito. A seconda dell\'organizzazione, ciò
potrebbe includere (ma non si limita a) sviluppatori software, specialisti del
rilascio, responsabili della qualità, responsabili del marketing di prodotto,
responsabili di prodotto.

**SPDX** o Software Package Data Exchange
:   il formato standard creato dall\'SPDX Working Group per lo scambio di
informazioni di licenza e diritto d'autore circa un determinato pacchetto
software. Una descrizione della specifica SPDX può essere reperita presso
[www.spdx.org](http://www.spdx.org/).

**Software Fornito**
:   software che un\'organizzazione fornisce a terze
parti (per esempio, altre organizzazioni o altre persone).

**Materiali di Verifica**
:   prove che debbono esistere al fine di
considerare soddisfatto un determinato requisito.

# Requisiti

## Obiettivo 1: Conosci le Tue Responsabilità FOSS {- label="Obiettivo 1"}

1.   **Esiste una politica FOSS interna che regola il rispetto delle licenze
     FOSS nella distribuzione del Software Fornito.** La Politica deve essere
     comunicata internamente.

#### Materiali di Verifica

-   1.1.1 Una politica FOSS documentata
-   1.1.2 Una procedura documentata che rende il Personale del Software
    consapevole dell\'esistenza di una politica FOSS (per esempio,
    tramite formazione, un wiki interno, ovvero altri metodi di
    comunicazione).

#### Razionale:

Assicurare che siano intrapresi passi per creare, registrare e rendere
il Personale del Software informato dell\'esistenza di una politica
FOSS. Sebbene qui non sono forniti requisiti su cosa debba essere
incluso in tale politica, altre sezioni potrebbero imporre requisiti
sulla politica.

1.  **Esiste una formazione FOSS obbligatoria per tutto il Personale del
    Software, tale per cui:**

-   **La formazione, come minimo, copre le seguenti aree:**
-   **La politica FOSS e dove reperirne una copia;**
    -   **Fondamenti di diritto di proprietà intellettuale attinente al
        FOSS e alle licenze FOSS;**
    -   **Concetti sulla licenza del FOSS (inclusi i concetti di licenze
        permissive e copyleft);**
    -   **I modelli di licenza dei progetti FOSS;**
    -   **Ruoli e responsabilità del Personale del Software riguardo
        specificamente alla conformità FOSS e in generale alla politica
        FOSS; e**
    -   **Processi per identificare, registrare e/o tenere traccia dei
        componenti FOSS contenuti nel Software Fornito.**

<!-- -->

-   **Il Personale del Software deve aver completato una formazione FOSS
    negli ultimi 24 mesi per essere considerato aggiornato ("Attualmente
    Formato"). Un test può essere impiegato per consentire al Personale
    del Software di soddisfare il requisito di formazione.**

#### Materiali di Verifica

-   1.2.1 Materiali di formazione FOSS che coprono le aree di cui sopra
    (per esempio, serie di slide, corso online o altri materiali di
    formazione).
-   1.2.2 Un metodo documentato per tenere traccia del completamento
    della formazione per tutto il Personale del Software.
-   1.2.3 Almeno l\'85% del Personale del Software è Attualmente
    Formato, come da definizioni di cui sopra. L'85% può non riferirsi
    necessariamente a tutta l'organizzazione, ma alla totalità del
    Personale del Software regolato dal programma di Conformità
    OpenChain.

#### Razionale:

Assicurare che il Personale del Software abbia recentemente partecipato
a una formazione FOSS e che un insieme fondamentale di argomenti FOSS
siano stati affrontati nella formazione. L\'intento è di assicurare che
un insieme di argomenti centrali di livello base siano stati affrontati,
ma un programma di formazione tipico sarebbe verosimilmente più ampio di
quanto qui è richiesto.

1. **Esiste un processo per esaminare le Licenze Identificate per
        determinare le obbligazioni, le restrizioni e i diritti
        conferiti da ciascuna licenza.**

#### Materiali di Verifica

-   1.3.1 Una procedura documentata per la revisione e la documentazione
    delle obbligazioni, delle restrizioni e dei diritti conferiti da
    ciascuna Licenza Identificata.

#### Razionale:

Assicurare l\'esistenza di una procedura per la revisione e
l'identificazione delle obbligazioni per ciascuna Licenza Identificata
per i vari casi d\'uso.

## Obiettivo 2: Assegna Responsabilità per Conseguire Conformità {-}

**2.1 Identifica la Funzione di Contatto Esterno del FOSS (\"Contatto
FOSS\")**

-   **Nomina il/i soggetto/i responsabile/i di ricevere domande esterne
    sul FOSS;**
-   Il Contatto FOSS deve fare sforzi commercialmente ragionevoli per
    rispondere appropriatamente alle richieste circa la conformità FOSS;
    e
-   Identifica pubblicamente un mezzo tramite il quale si possa
    contattare il Contatto FOSS.

#### Materiali di Verifica

-   2.1.1 Identificazione pubblicamente visibile del Contatto FOSS (per
    esempio, tramite un indirizzo email pubblicato, o la Open Compliance
    Directory della Linux Foundation).

<!-- -->

-   2.1.2 Una procedura interna documentata che assegna le
    responsabilità per ricevere richieste circa la conformità FOSS.

#### Razionale:

Assicurare che vi sia un modo ragionevole per i terzi di contattare
l\'organizzazione per domande circa la conformità FOSS e che questa
responsabilità sia stata effettivamente assegnata.

**2.2 Identifica il/i Ruolo/i di Conformità Interna FOSS**

-   **Nomina il/i responsabile/i per gestire la conformità interna FOSS.
    Il ruolo di Conformità FOSS e il ruolo di Contatto FOSS possono
    coesistere nella stessa persona.**
-   L\'attività di gestione della conformità FOSS è dotata di
    sufficienti risorse:

    -   Tempo per svolgere le funzioni del ruolo è stato assegnato; e
    -   Budget commercialmente ragionevole è stato assegnato.

-   **Assegna le responsabilità di sviluppare e mantenere le politica e
    i processi FOSS;**
-   **Competenze legali circa la conformità FOSS sono accessibili al
    ruolo di Conformità FOSS (potrebbero essere risorse interne o
    esterne); e**
-   Esiste un processo per la risoluzione di questioni di conformità
    FOSS.

#### Materiali di Verifica

-   2.2.1 I nomi delle persone, gruppi o funzioni nel/nei ruolo/i di Conformità
    FOSS sono identificati internamente.
-   2.2.2 Identificazione di competenze legali disponibili ai ruoli di
    Conformità FOSS, che possono essere interne o esterne.
-   2.2.3 Una procedura documentata per assegnare le responsabilità interne per
    la conformità FOSS.
-   2.2.4 Una procedura documentata per gestire la revisione di casi di mancata
    conformità e porvi rimedio.

#### Razionale:

Assicurare che le responsabilità interne FOSS siano effettivamente
assegnate.

## Obiettivo 3: Verifica e Approva il Contenuto FOSS {-}

**3.1 Esiste un processo per creare e gestire una lista di materiali del
componente FOSS che include ciascun componente (e le sue Licenze
Identificate) del quale è composto il Software Fornito.**

#### Materiali di Verifica

-   3.1.1 Una una procedura documentata per identificare, tracciare e
    archiviare informazione sulla raccolte di componenti FOSS dei quali
    è composta una versione del Software Fornito.
-   3.1.2 Registrazioni dei componenti FOSS per ciascuna versione del
    Software Fornito che dimostrano che la procedura documentata è stata
    seguita correttamente.

#### Razionale:

Garantire che esiste un processo per creare e gestire una lista dei
materiali del componente FOSS utilizzata per costruire il Software
Fornito. Una lista dei materiali è necessaria per supportare la
revisione sistematica dei termini di licenza di ciascun componente per
comprendere gli obblighi e le restrizioni applicabili alla distribuzione
del Software Fornito.

**3.2 Il programma di gestione del FOSS deve essere in grado di gestire
i casi comuni d\'uso di licenza FOSS incontrati dal Personale del
Software per il Software Fornito, che possono includere i seguenti casi
d\'uso (si noti che l\'elenco non è esaustivo e possono non applicarsi
tutti i casi d\'uso):**

-   distribuito in formato binario;
-   distribuito in formato sorgente;
-   integrato con altro FOSS che può attivare degli obblighi copyleft;
-   contiene FOSS modificato;
-   contiene FOSS o altro software con una licenza incompatibile che
    interagisce con altri componenti del Software Fornito; e/o
-   contiene FOSS con requisiti di attribuzione.

#### Materiali di Verifica

-   3.2.1 Una procedura documentata per gestire i casi comuni d\'uso di
    licenza FOSS per i componenti FOSS del Software Fornito.

#### Razionale:

Assicurare che il programma è sufficientemente robusto per gestire i
casi comuni d\'uso di licenza FOSS per un\'organizzazione. Che esiste
una procedura per supportare quest\'attività e che la procedura è
seguita.

## Obiettivo 4: Consegna la Documentazione e gli Elaborati del Contenuto FOSS {-}

**4.1 Esiste un processo per creare l'insieme degli Elaborati di
Conformità per ciascun Software Fornito**

#### Materiali di Verifica

-   4.1.1 Una procedura documentata che assicura che gli Elaborati di
    Conformità vengono preparati e distribuiti con la versione del
    Software Fornito come richiesto dalle Licenze Identificate.
-   4.1.2 Copie degli Elaborati di Conformità della versione del
    Software Fornito sono archiviate e facilmente recuperabili, ed è
    previsto che l\'archivio esista almeno fino a quando il Software
    Fornito viene offerto o è richiesto dalle Licenze Identificate (a
    seconda di quale sia il termine più lungo).

#### Razionale:

Assicurare che la raccolta completa degli Elaborati di Conformità
accompagni il Software Fornito come richiesto dalle Licenze Identificate
insieme alle altre relazioni create nel quadro del processo di revisione
FOSS.

## Obiettivo 5: Comprendere il Coinvolgimento della Comunità FOSS {-}

**5.1 Esiste una politica scritta che regola i contributi ai progetti
FOSS da parte dell\'organizzazione. La politica deve essere comunicata
internamente.**

#### Materiali di Verifica

-   5.1.1 Una politica documentata di contributo FOSS;
-   5.1.2 Una procedura documentata che rende tutto il Personale del
    Software consapevole dell\'esistenza della politica di contributo
    FOSS (per esempio, mediante formazione, un wiki interno, altri
    metodi pratici di comunicazione).

#### Razionale:

Assicurare che un\'organizzazione abbia ragionevole preso in
considerazione lo sviluppo di una politica per contribuire pubblicamente
al FOSS. La politica di contributo FOSS può far parte della politica
globale FOSS di un\'organizzazione o può essere una politica specifica.
Nella situazione in cui i contributi non sono consentiti del tutto,
dovrebbe esistere una politica che renda chiara questa posizione.

**5.2 Se un\'organizzazione consente i contributi ai progetti FOSS allora
deve esistere un processo che implementa la politica di contributo FOSS
prevista nel capitolo 5.1.**

#### Materiali di Verifica

-   5.2.1 Se la politica di contributo FOSS consente di contribuire, una
    procedura documentata che disciplina i contributi FOSS.

**Razionale**:

Assicurare che un\'organizzazione abbia un processo documentato riguardo
come l\'organizzazione contribuisce pubblicamente il FOSS. Può esistere
una politica tale per cui i contributi non sono consentiti del tutto. In
questa situazione è chiaro che una procedura può non sistere e questo
requisito sarebbe comunque soddisfatto.

## Obiettivo 6: Certificare l\'Adesione ai Requisiti OpenChain {-}

**6.1 Affinché un\'organizzazione sia Certificata OpenChain, deve
dichiarare di disporre di un programma di gestione FOSS che soddisfa i
criteri descritti in questa versione 1.2 della Specifica OpenChain.**

#### Materiali di Verifica

-  6.1.1 Una dichiarazione dell'esistenza di un programma di gestione FOSS che
   soddisfa tutti i requisiti di questa Specifica OpenChain versione 1.2.

#### Razionale:

Per garantire che se un\'organizzazione dichiara di avere un programma
che è di Conformità OpenChain, tale programma ha soddisfatto *tutti* i
requisiti di questa specifica. La semplice conformità ad un sottoinsieme
di tali requisiti non sarebbe considerata sufficiente.

**6.2 La conformità a questa versione della specifica durerà 18 mesi
dalla data di ottenimento della convalida della conformità. I requisiti
di convalida della conformità possono essere trovati sul sito web del
progetto OpenChain.**

#### Materiali di Verifica

-  6.2.1 L\'organizzazione afferma che esiste un programma di gestione FOSS che
soddisfa tutti i requisiti di questa Specifica OpenChain versione 1.2 entro 18
mesi dall'ottenimento della convalida di conformità.

#### Razionale:

È importante che l\'organizzazione rimanga aggiornata con la specifica
se l'organizzazione vuole affermare la conformità al programma nel
tempo. Questo requisito assicura che i processi e i controlli di
supporto del programma non si erodono se l'organizzazione che si
conforma continua ad afferma la conformità nel tempo.

# Appendice I: Traduzioni {-}

Per facilitare l\'adozione globale, accogliamo con piacere gli sforzi
per tradurre la specifica in più lingue. Poiché OpenChain funziona come
un progetto open source le traduzioni sono guidate da coloro che
vogliono contribuire con il loro tempo e le loro competenze per eseguire
le traduzioni secondo i termini della licenza CC-BY 4.0 e secondo la
politica di traduzione del progetto. I dettagli della politica e le
traduzioni disponibili si trovano nella [pagina web
della specifica](https://wiki.linuxfoundation.org/openchain/spec-translations)
del progetto OpenChain.
