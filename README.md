# Wilder-Event-2.0

Pour installer le projet :
-> composer install
-> yarn install

Pour compiler les assets : 
-> yarn encore dev
-> yarn encore dev --watch

Pour créer la bdd :
-> créer un .en.dev.local à partir du .env
-> ajouter ses id de connection
dans le terminal :
-> symfony console d:d:c

Pour faire remettre le fichier de migration au propre : 
-> supprimer touts les fichiers de migrations
dans le terminal :
-> symfony console d:d:d --force
-> symfony console d:d:c
-> symfony console d:mig
-> symfony console d:m:m
Vous êtes à jour !

Lancer le serveur : 
-> symfony consoler server:start -d

-----------------------------------------------------------------------------------------------
Workflow :

Pour chaque feature :
-> tirer une nouvel branche à partir de dev
-> commit -m 'feature/nomdelafeature'
-> push nomdetabranche
-> PR vers dev

Pour la correction des bugs :
-> tirer une nouvel branche à partir de dev
-> commit -m 'bugfix/nomdubug'
-> push nomdetabranche
-> PR vers dev

Pour une PR non acceptés : 
-> reprendre la branche de sa feature ou son bug
-> commit -m 'fix after review/descriptif'
-> push nomdetabranche
-> pas besoin de PR elle sera automatiquement mis à jour

Good code !
