# Happy Quizz 

# Lien vers le site 
URL prod: https://react-wdcvalentin.herokuapp.com/
URL preprod: https://react-wdcvalentin-preprod.herokuapp.com/

# Comment installer le projet 
## Cloner le projet 
```
git clone https://github.com/IIM-Creative-Technology/react-wdcvalentin.git && cd react-wdcvalentin
```

## Installer les dépendences
```
npm install
ou 
yarn install
```


## Démarrer le projet 
```
npm start
ou 
yarn start
```
Enjoy :)

## CI/CD
-   Lorsque l'on push, une pipeline se met en route à l'aide du fichier deploy.yml 
    qui se trouve dans le dossier caché nommé : .github
-   Dans ce fichier, je définis que je veux lancer la pipeline sur les pull-request et mes branches
-   J'ai crée deux environnements sur github: Staging et Prod
-   Chaque environnement lancera :
    - Son initialisation
    - Une mise en cache des dépendances pour améliorer workflow
    - Une installation de node
    - Un build
    - Les tests unitaires
    - Et son déploiement sur heroku