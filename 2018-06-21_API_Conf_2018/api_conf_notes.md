# API Conf
[conference link](https://2018.apiconf.it/)
[web app](https://live.apiconf.it/)
`@_CloudConf`

## GraphQL as an API Gateway,
Massimiliano Mantione `@M_a_s_s_i` - #GraphQL

Quando si espongono delle API in rete, oltre ad implementarle, e' necessario definirle formalmente, documentarle, organizzarle in modo coerente, e spesso anche specificare come API diverse interagiscano tra loro. GraphQL si pone come *middleman* tra il client ed il back end, e vuole razionalizzare tutti questi aspetti in modo alternativo al classico REST.

GraphQL: query language for API, linguaggio di query per i servizi
si possono interrogare i dati
linguaggio di query che non è json ma che lo ricorda
perchè non semplicemente rest? rest in realtà ha qualche problema:
  * overfetching: richiesta di dati che non mi servono
  * underfetching: ok, facciamo risorse più piccole per avere più granularità, ma poi quello che succede è che fai più richieste
  * latency (round trips): facendo più richieste aumenta la lateza

quello che uno vorrebbe è "exact fetching"; rest has a fixed, url-based resource granularity
rest funziona con una risorsa sola ma se devo prendere più di una risorsa sono costretto a fare paginazione o ottenere risposte grosse

graphql: si basa su una singola risorsa: "the graph"
ogni richiesta di graphql è una post
definisce un linguaggio di query per esplorare questo grafo
CQRS ready

è possibile definire i propri microservizi sfruttando graphql

graphql è nata in facebook per ottemperare al grande numero di api complesse
utilizzato da: facebook, github, netflix (falcor)

graphql ha un costo, ovviamente; costo che uno paga per avere dei benefici sull'interazione

## Eliminare le Spaghetti API
Giulio Roggero `@giulioroggero` - #BestPractice

Il software che oggi produce valore è stato scritto parecchi anni fa. Il costo di manutenzione ed evoluzione sta diventando sempre più alto. Parallelamente stiamo vivendo una forte accelerazione sul digitale: omnicanalità, self-service e ubiquità sono fattori che stanno influenzando i comportamenti delle persone. Alle aziende si chiede sempre più innovazione e semplicità dei servizi offerti. In questa presentazione proveremo a dare una risposta a questa domanda: come possiamo evitare di accumulare un debito tecnico difficilmente ripagabile e nel contempo seguire l’accelerazione che il mercato ci sta chiedendo senza impattare sul business esistente?

Nel mondo dell'innovazione e dell'avanzamento tecnologico, l'effetto wow si va trasformando sempre di più in bisogno base
debito tecnico
il costo di evolutive software nel tempo cresce
curva costo teorico + debito tecnico accumulato nel tempo = curva costo reale per aggiungere nuove funzionalità

## Coffee Break
  #GraphQL -> Gian Marco Toso
  #KubernetesAPI -> Gianluca Arbezzano (CNCF)
  #Blockchain -> Marco Roberti (Ethereum Blockchain Torino)
  #Serverless -> Walter Dal Mut

## Progettare un sistema Blockchain con Hyperledger per la condivisione sicura di dati
Edoardo Conte - #Blockchain

La Blockchain si presenta come una tecnologia in pieno sviluppo, in grado di ospitare in maniera immutabile i dati di chi ne fa utilizzo. Durante la talk verrà descritta in maniera approfondita la blockchain privata Hyperledger Fabric. Tramite un framework, chiamato Hyperledger Composer, verrà mostrato il design di un applicativo, con il quale sarà possibile interagire da una web application tramite API.

## Microservizi e API: dalla progettazione al deploy e monitoring
Walter Dal Mut `@walterdalmut` - #Security #Performance

Best practice, tool e metodologie per sviluppare architetture complesse a microservizi. Dall'esperienza diretta sul campo un intervento focalizzato su come affrontare uno sviluppo API e la gestione dei microservizi, partendo dalla progettazione e proseguento, step by step, alle fasi di sviluppo, gestione dei rilasci, monitoring e loggin.

## Serverless APIs su AWS
Alessandro Gambirasio - #AWS #Serverless

In questa sessione verranno illustrate le funzionalità e le linee guida per la costruzione di API serverless sulla piattaforma AWS. Verranno presentati strumenti come Lambda e API gateway per l'implementazione di processi basati su eventi.

## API for robots
Federico Minzoni - #CaseStudy

Nelle moderne assembly line, digitali, i vari servizi lavorano insieme comunicano tra loro tramite API. Così, ad esempio, sulla base della telemetria, viene cambiato adeguatamente il numero di risorse attive, una modifica al codice scatena tutte le operazioni necessarie per il test e la distribuzione dei nuovi artifact, tutto automaticamente, senza l’intervento di noi umani. Il talk mostra alcuni scenari di produzione in cui queste dinamiche sono già reali, raccontando la nostra soluzione tecnologica per creare efficienti processi di automazione

## Velocizzare lo sviluppo di web API in PHP con Expressive
Enrico Zimuel `@ezimuel` - #PHP #Performance

In questo talk verrà presentato il framework di sviluppo Expressive 3 (http://getexpressive.org) per il linguaggio PHP. Questo framework consente di sviluppare web API in pochi minuti fornendo un'infrastruttura RESTful pronta con un sistema di autenticazione e autorizzazione OAuth2, filtro e validazione dei dati in ingresso, gestione degli errori, etc. Inoltre, l'approccio middleware di Expressive consente di ottenere delle prestazioni elevate utilizzando l'estensione open source Swoole per PHP 7. Durante il talk verrà presentato un benchmark effettuato su un'applicazione d'esempio in PHP con tempi di esecuzione 4 volte inferiori rispetto a nginx o Apache.

## Progettare una UI per i Microservices
Mauro Servienti `@mauroservienti` - #Microservices

Come possiamo progettare una UI quando il back-end è composto da decine (se non di più) di Microservices? Abbiamo la giusta separazione e autonomia lato back-end, ma tutto alla fine deve tornare insieme lato front-end. Come evitiamo che si trasformi nel solito caos di spaghetti code? Come evitiamo che operazioni semplici si trasformino in un tornado di web request? Durante questa sessione costruiremo un esempio di UI per Microservices, usando .NET Core, in modo da capire a fondo cosa sia la Services UI Composition e come progettare e implementare con successo una UI per i nostri Microservices.

## Dagli anni '00 agli anni '20: da REST a gRPC
Gianfranco Reppucci `@giefferre` - #gRPC #JSON-RPC

REST sta per representational state transfer, ed indica un tipo di architettura software proposto e descritto da Roy Fielding nella sua tesi di dottorato presentata nel 2000. Da allora è stata ampiamente adottato, ma sfortunatamente non tutti coloro che hanno implementato API REST hanno letto quella tesi. Come se non bastasse, ci sono casi in cui un’architettura software del genere non soddisfa le esigenze. Vale ancora utilizzare REST? Diamo un’occhiata a soluzioni più moderne di tipo RPC, come JSON-RPC e gRPC.
