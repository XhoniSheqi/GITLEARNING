GIT
-Tool da riga da comando
-Tenere traccia delle modifiche che facciamo al codice
-Utile quando stai lavorando con molte persone allo stesso tempo
-Conservare il codice in una reposity , e più collaboratori possono accedere allo stesso filee modificare quest'ultimi e pushare al server
-Ci consente di testare il nostro codice
-Possiamo creare un ramo nuovo dove testiamo un codice modificato rispetto al codice originale e poi unire il tutto o no
-Posso tornare alle versioni precedenti del mio codice

Gol of today ?? --> learn how to deal with Git and etc ...

Per accedere al codice abbiamo bisogno di un posto dove poszionare il nostro codice per questo una delle piattaforme di hosting più usate è GitHub

GitHub --> sito web in cui possiamo depositare le Git reposity ( possiamo pensarlo come una cartella dove ci sono i nostri file di codice ...)

GitHub.com/new --> ci porta alla pagina dove creare una nuova reposity

prima cosa da fare --> nome della reposity
--> descrizione della reposity
--> scegliere se è private o public

Primo comando git
git clone --> grazie il quale possiamo scaricare le repostiy

    git clone url :
        prende la reposity dal server e la scarica localmente sul computer

( su CMD call >> nome.estensione crea un file , code . apre il code editor di default , start nome file apre il file su browser)

    Quando salvo lo stato corrente del codice sto facendo un commit del codice

Comando per committare

git add --> dire a git che voglio creare un commit e dire a git di quale file parliamo , possiamo anche solo committare una parte dei file e non tutti

git commit --> voglio salvare lo stato in cui ora si trova la reposity

git commit -m "messaggio del commit"

per specificare la tua identità di github usa

git --global user.email "youremail@gmail.com"
git --global user.name "YourName"

Tutti questi comandi stavano solamente influenzando la reposity locale

git status --> per controllare lo stato della reposity ( ci dice anche quanti commit abbiamo )

git push --> tutti i commit e i salvatti arrivano al server di github

git push --set-upstream origin main --> nel caso non ci trovassiamo su origin/master bensi su origin/main usiamo questo comando per pushare al server la reposity

git-pull --> scarica l'ultima versione su github , nel caso quella locale sia meno recente rispetto alla reposity sul server

Posso usare anche github web per modificare i file

Sommario

git clone url
git add file.ext
git commit -m ""
git status
git push
git pull
git commit -am ""

DOMANI MATTINA --> Merge Conflict

Quando facciamo una dichiarazione sul nostro progetto locale e idem un nostro collab. e le due modifiche collidono avviene ciò che chiamiamo merge conflict
Ogni conflic ha un codice hash univico , per risolvere un merge conflict dobbiamo semplicemente scegliere tra una delle due parti e cancellare il resto e pushare

git log --> ci riporta tutti i commit fatti sul progetto
