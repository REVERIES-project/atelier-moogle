# Atelier TP MOGGLE

## Première partie : interface et page de démonstration d'un composant

Dans ce TP vous allez concevoir et implémenter diverses améliorations dans le fonctionnement du composant "free-text-question". Ce composant est disponible [à cette adresse](https://github.com/REVERIES-project/free-text-question).

* Se rendre sur la page du composant et consulter la page **documentation et démo** (lien situé en bas de la page principale)

* Cette page présente une **brève description du composant**, ainsi que **l'API publique exposée par ce dernier**.
  * Les **propriétés** (properties) correspondent aux *attributs html* qui peuvent être renseignés pour ce composant. Par exemple la propriété `question` est une chaine de caractère correspondant à la question qui sera affichée à l'utilisateur.
  * Les méthodes correspondent aux nouvelles fonctions que ce composant expose et que l'on peut appeler depuis l'extérieur.

![Api freetext](./images/free-text-api.png)


* Se rendre sur la page de démonstration du composant. En haut à droite en cliquant sur l'icone démo. ![Page démonstration](./images/demo_button.png)

![Page démonstration](./images/demo_freetext.png)

* Cette page de démonstration est divisée en deux parties :
  * Une instance du composant avec laquelle on peut interagir
  * Le code correspondant à cette instance, situé dans la partie inférieure. Ce code fournit un exemple direct d'utilisation du composant, plus efficace souvent que la documentation. 
  * Ici ce code est:

```html 
<free-text-question question="Quelle est la réponse?" response="dans la question" response-label="Entrez votre réponse" media="{&quot;mkdown&quot;:&quot;## La réponse est dans la question&quot;}" correct-message="Bravo vous êtes un individu remarquable" wrong-message="Non c'est faux, essayez encore et encore et encore"></free-text-question>
```

* En regardant le code de l'instance de démonstration, ou l'indice, deviner la bonne réponse. 
  * Se montrer satisfait si on devine correctement
  * Cacher sa frustration et essayer encore en cas de réponse incorrecte

## Deuxième partie : amélioration du composant free-text-question 

Rappel : la modification d'un composant de jeu sera refletée dans **l'editeur MOGGLE** (destiné aux concepteurs de jeux) et dans **MOGGLE Game player** (destiné aux joueurs). 

Les modifications que vous aller réaliser seront uniquement en *localhost* sur votre session. Pour qu'elles soient intégrées dans l'éditeur vous aurez à réaliser une *pull request* que le/les propriétaires du repository accepteront. L'utilisation de github sort du cadre de cet atelier, vous pouvez plus d'informations [ici](https://services.github.com/on-demand/github-cli/open-pull-request-github).


* Commencer par ouvrir une fenêtre terminal (Application/Terminal).
* Créer un dossier Dev pour l'atelier
    ```bash
     mkdir Dev
     cd Dev
     ```
* Depuis le dossier Dev, effectuer un *git clone* du repository de *free-text-question*. Installer ensuite les dépendances bower du composant
     ```bash
     git clone https://github.com/REVERIES-project/free-text-question.git
     bower install 
     ```
* Le composant est maintenant installé localement et peut être modifié et testé facilement. Lancer le serveur Polymer local
     ```bash
    polymer serve
    ```
  * Cette commande affiche une réponse semblable à 

  ` info:    Files in this directory are available under the following URLs`
  
   `applications: http://127.0.0.1:8081`
  
   `reusable components: http://127.0.0.1:8081/components/free-text-question/`

* Ouvrir l'adresse correspondant à *reusable component* (ctrl + clic). Le navigateur Firefox s'ouvre à l'adresse donnée. La page est la même que la page de *documentation/démo* que celle à laquelle vous accediez précédemment. Cependant vous pouvez maintenant modifier le code et voir les modifications par un simple rafraichissement du browser (F5).

  * Ouvrir une nouvelle fenêtre de terminal et se rendre dans le répertoire du composant pour lancer *Visual Studio Code*.
    ```bash
     cd Dev/free-text-question
     code
     ```


  












