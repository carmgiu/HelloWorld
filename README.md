# HelloWorld

Creato il ramo readme-edits

Prova di dettato perché non va eccolo abbiamo tutto per dettare un testo in un file l'ascolto va avanti per molto tempo e si possono eseguire molti paragrafi.

  Digitare Win + h  dopo aver posizionato file: vittorio.txt

 esempio di inserimento di un bot echo, eseguito con framework  - LINK       questo ascolto è a posto   

 https://github.com/microsoft/BotBuilder-Samples/tree/main/samples/javascript_nodejs/01.console-echo

 Esempio di bot console bot di Bot Framework v4

Questo bot è stato creato utilizzando Bot Framework, mostra come creare un semplice bot con cui è possibile parlare dalla finestra della console.

Prerequisiti
Node.js versione 10.14 o successiva

# determine node version
node --version
Per provare questo esempio
Clonare il repository

git clone https://github.com/microsoft/botbuilder-samples.git

... eseguito

PS C:\Users\Carmela> node --version
v14.17.0

PS C:\Users\Carmela> git clone https://github.com/microsoft/botbuilder-samples.git

Cloning into 'botbuilder-samples'...
remote: Enumerating objects: 65562, done.
remote: Counting objects: 100% (508/508), done.
remote: Compressing objects: 100% (260/260), done.
remote: Total 65562 (delta 332), reused 401 (delta 244), pack-reused 65054
Receiving objects: 100% (65562/65562), 83.90 MiB | 11.12 MiB/s, done.
Resolving deltas: 100% (43701/43701), done.
Updating files: 100% (6663/6663), done.
______________________________________________________________________________________________________________________________________  OK

In un terminale, passare a samples/javascript_nodejs/01.console-echo

PS C:\Users\Carmela> cd botbuilder-samples
PS C:\Users\Carmela\botbuilder-samples> dir


    Directory: C:\Users\Carmela\botbuilder-samples


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----       29/01/2022     08:44                .github
d-----       29/01/2022     08:44                build
d-----       29/01/2022     08:44                composer-samples
d-----       29/01/2022     08:44                docs
d-----       29/01/2022     08:44                experimental
d-----       29/01/2022     08:44                generators
d-----       29/01/2022     08:44                Migration
d-----       29/01/2022     08:44                MigrationV3V4
d-----       29/01/2022     08:45                samples
-a----       29/01/2022     08:44          11508 .editorconfig
-a----       29/01/2022     08:44            914 .gitattributes
-a----       29/01/2022     08:44           5421 .gitignore
-a----       29/01/2022     08:44            451 CODE_OF_CONDUCT.md
-a----       29/01/2022     08:44           2959 CONTRIBUTING.md
-a----       29/01/2022     08:44            458 INSTALLING_CLI_TOOLS.md
-a----       29/01/2022     08:44           1131 LICENSE.md
-a----       29/01/2022     08:44          24833 README.md
-a----       29/01/2022     08:44           7458 SPEC.md


PS C:\Users\Carmela\botbuilder-samples> cd samples/javascript_nodejs/01.console-echo

PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo>

cd samples/javascript_nodejs/01.console-echo

 Per Installare i moduli:

 npm install                                     <---  dare

PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo> npm install
npm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.


added 331 packages, and audited 332 packages in 2m

64 packages are looking for funding
  run `npm fund` for details

4 moderate severity vulnerabilities

To address all issues, run:
  npm audit fix --force

Run `npm audit` for details.
PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo> npm audit fix --force
npm WARN using --force Recommended protections disabled.
npm WARN audit Updating botbuilder-core to 4.15.0,which is outside your stated dependency range.

added 36 packages, removed 2 packages, changed 10 packages, and audited 366 packages in 49s

66 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
_________________________________________________________________________________________________________

 Per avviare il bot                                 

 npm start                                        <---  dare  ( quit  <---  dare per finire )

....
PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo> npm start

> console-echobot@1.0.0 start
> node ./index.js

> Console EchoBot is online. I will repeat any message you send me!
> Say "quit" to end.

Bot Attenti!
I heard you say "Bot Attenti!"

Buon lavoro
I heard you say "Buon lavoro"
quit
Bye!

_________________________________________________________________________________________________________

Test del bot
Dopo l'esecuzione, il bot presenta un prompt direttamente nella finestra della console.npm start

Invia messaggi al bot digitandoli nella console. Il bot ti farà eco al tuo messaggio.

Adattatori

Adattatori come il forniscono un'astrazione per il bot per lavorare con una varietà di ambienti e piattaforme di messaggistica.ConsoleAdapter

L'adattatore è responsabile della direzione della comunicazione in entrata e in uscita, dell'autenticazione e così via.

 Gli adattatori per piattaforme e tecnologie di messaggistica diverse differiscono internamente, ma raggiungono lo stesso obiettivo: connettere i bot a un flusso di messaggi

 ed eventi da parte degli utenti. Quando il bot riceve un'attività, l'adattatore racchiude tutto ciò che riguarda tale attività, crea un oggetto contesto, lo passa alla logica

 dell'applicazione del bot e invia le risposte generate dal bot al canale dell'utente.

Nella maggior parte delle situazioni, non lavoriamo direttamente con l'adattatore, ma è bene sapere che è lì e cosa fa. In questo esempio, stiamo usando il ConsoleAdapter,

 che fornisce un modo molto semplice per scambiare messaggi: vengono inviati e ricevuti tramite la finestra della console. 

L'utilizzo di ConsoleAdapter è un ottimo modo per iniziare rapidamente con Botbuilder.

 Consente inoltre di creare e testare bot che operano sul computer locale senza chiamate API esterne o applicazioni client.ConsoleAdapter

Altri adattatori disponibili connettono il bot al Web o, tramite il servizio BotFramework Connector, a molte piattaforme di messaggistica popolari.

Ulteriori letture
Documentazione di Bot Framework
Nozioni di base sui bot
Elaborazione delle attività
Introduzione al servizio Azure Bot     <-- Link - https://docs.microsoft.com/it-it/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-4.0
Documentazione del servizio Azure Bot
Interfaccia della riga di comando di Azure
Portale di Azure
Comprensione del linguaggio con LUIS
Canali e servizio Bot Connector
Restifica
dotenv

::::::::::::::::::  https://docs.microsoft.com/it-it/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-4.0

Che cos'è un bot?
I bot forniscono un'esperienza che non dà tanto la sensazione di usare un computer, quanto di interagire con una persona o almeno con un robot intelligente. Possono essere usati per attività semplici e ripetitive, come la prenotazione di una cena o la raccolta di informazioni sul profilo, e nei sistemi automatizzati che non richiedono più necessariamente l'intervento umano diretto. Gli utenti conversano con un bot usando testo, schede interattive e parlato. Un'interazione con un bot può essere un rapido scambio domanda-risposta oppure una conversazione sofisticata che fornisce l'accesso ai servizi in modo intelligente.
Un bot può essere pensato come un'applicazione Web con un'interfaccia di conversazione. Un utente si connette a un bot tramite un canale come Facebook, Slack o Microsoft Teams.
Il bot è alla base dell'input ed esegue le attività pertinenti. Ciò può includere la richiesta all'utente di informazioni aggiuntive o l'accesso ai servizi per conto dell'utente.
Il bot esegue il riconoscimento dell'input dell'utente per interpretare ciò che l'utente chiede o dice.
Il bot genera risposte da inviare all'utente per comunicare ciò che il bot sta facendo o ha fatto.
A seconda della configurazione e della registrazione del bot con il canale, gli utenti possono interagire con il bot tramite testo o parlato e la conversazione potrebbe includere immagini e video.
....

I bot sono molto simili alle moderne applicazioni Web, che si connettono a Internet e usano le API per inviare e ricevere messaggi. Il contenuto di un bot varia notevolmente a seconda del tipo di bot. Il software bot moderno si basa su una serie di tecnologie e strumenti per fornire esperienze sempre più complesse in una vasta gamma di piattaforme. Un bot semplice può tuttavia semplicemente ricevere un messaggio e inviarlo di nuovo all'utente con la necessità di pochissimo codice.
I bot possono svolgere le stesse operazioni di altri tipi di software: leggere e scrivere file, usare database e API ed eseguire normali attività di calcolo. La peculiarità dei bot risiede nell'uso di meccanismi generalmente riservati alla comunicazione tra esseri umani.
Il servizio Azure Bot e l'Bot Framework offerta:
SDK Bot Framework per lo sviluppo di bot
Bot Framework Tools per gestire il flusso di lavoro di sviluppo di bot end-to-end
Bot Framework Service (BFS) per inviare e ricevere messaggi ed eventi tra bot e canali
Distribuzione dei bot e configurazione dei canali in Azure
I bot possono anche usare altri servizi di Azure, ad esempio:
Servizi cognitivi di Azure per creare applicazioni intelligenti
Archiviazione di Azure come soluzione per l'archiviazione nel cloud
Compilazione di un bot
Il servizio Azure Bot e Bot Framework offrono un set integrato di strumenti e servizi che agevolano questo processo. Scegliere l'ambiente di sviluppo o gli strumenti da riga di comando preferiti per creare il bot. Sono disponibili SDK per C#, JavaScript, Typescript e Python. L'SDK per Java è in fase di sviluppo. Sono disponibili strumenti per diverse fasi dello sviluppo del bot, per semplificarne la progettazione e la creazione.

... seguono i due file principali dell'esempio

PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo> type index.js

// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT License.

// @ts-check

const path = require('path');
const { ConsoleAdapter } = require('./consoleAdapter');

// load environment variables from .env file.
const ENV_FILE = path.join(__dirname, '.env');
require('dotenv').config({ path: ENV_FILE });

// Create the bot adapter, which is responsible for sending and receiving messages.
// We are using the ConsoleAdapter, which enables a bot you can chat with from within your terminal window.
const adapter = new ConsoleAdapter();

// Import our bot class.
const { EchoBot } = require('./bot');
const bot = new EchoBot();

// A call to adapter.listen tells the adapter to start listening for incoming messages and events, known as "activities."
// Activities are received as TurnContext objects by the handler function.
adapter.listen(async (context) => {
    bot.onTurn(context);
});

// Emit a startup message with some instructions.
console.log('> Console EchoBot is online. I will repeat any message you send me!');
console.log('> Say "quit" to end.');
console.log(''); // Leave a blank line after instructions.

....

PS C:\Users\Carmela\botbuilder-samples\samples\javascript_nodejs\01.console-echo> type bot.js

// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT License.

// @ts-check

class EchoBot {
    async onTurn(context) {
        // Check to see if this activity is an incoming message.
        // (It could theoretically be another type of activity.)
        if (context.activity.type === 'message' && context.activity.text) {
            // Check to see if the user sent a simple "quit" message.
            if (context.activity.text.toLowerCase() === 'quit') {
                // Send a reply.
                context.sendActivity('Bye!');
                process.exit();
            } else {
                // Echo the message text back to the user.
                return context.sendActivity(`I heard you say "${ context.activity.text }"`);
            }
        }
    }
}

module.exports = { EchoBot };
 

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
