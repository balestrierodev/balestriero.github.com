Questa pagina è una single page application sviluppata puramente in Angular che elabora in maniera dinamica i titoli, i paragrafi, le formattazioni e li renderizza mostrandoti il testo così come lo vedi.
            
Sfrutta il provider HttpClient tramite il metodo this.httpClient.get() per effettuare una richiesta GET al <a rel="nofollow" target="_blank" href="[jsonDataUrl]">seguente indirizzo</a> ed ottenere quindi in formato RAW, il JSON contenente un oggetto che contiene a sua volta delle chiavi che contengono a loro volta le stringhe dei paragrafi così come li leggi.
            
Il componente, tramite un Observable, rimarrà in alscolto sul'eventuale emissione di dati di tale richiesta tramite il metodo this.observable.subscribe().

Una volta ricevuto il dato, viene ciclato ed elaborato.

L'applicazione sfrutta inoltre un sistema di routing mediante RouterModule, rimanendo in ascolto sull'Observable che si occcupa di emettere un valore ad ogni cambio di pagina (es: "/storia")

Per quanto riguarda lo stile invece è stato scritto in SCSS interno ad Angular, per stilizzare componente per componente tramite un innesto di selettori padri / figli.

Se hai curiosità e vuoi vedere l'intero sorgente dell'applicazione, puoi dare un'occhiata alla <a rel="nofollow" target="_blank"  href="[repoUrl]">repository corrispondente su Github</a>
