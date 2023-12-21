# Architecture MVC

# 

**MVC** (Model-View-Controller) est un modèle de conception de logiciels couramment utilisé pour implémenter des interfaces utilisateur, des données et une logique de contrôle. Il met l'accent sur une séparation entre la logique métier du logiciel et l'affichage. Cette "séparation des préoccupations" prévoit une meilleure division du travail et une meilleure maintenance. Certains autres modèles de conception sont basés sur MVC, tels que MVVM (Model-View-Viewmodel), MVP (Model-View-Presenter) et MVW (Model-View-Whatever).

                               

Les trois parties du modèle de conception logicielle MVC peuvent être décrites comme suit:

1. Modèle: Gère les données et la logique métier.
2. Vue: Poignées mise en page et affichage.
3. Contrôleur: Route les commandes vers le modèle et les parties de vue.

# 

## Exemple complet :

Imaginez une simple application de liste de courses.Tout ce que nous voulons est une liste du nom, de la quantité et du prix de chaque article que nous devons acheter cette semaine. Ci-dessous, nous décrirons comment nous pourrions implémenter certaines de ces fonctionnalités en utilisant MVC.

![MVC](https://developer.mozilla.org/en-US/docs/Glossary/MVC/model-view-controller-light-blue.png)


### [**Le Modèle**]

Le modèle définit les données que l'application doit contenir. Si l'état de ces données change, ensuite, le modèle notifiera généralement la vue (de sorte que l'affichage peut changer au besoin) et parfois le contrôleur (si une logique différente est nécessaire pour contrôler la vue mise à jour).

Pour revenir à notre application de liste de courses, le modèle spécifierait quelles données les éléments de la liste devraient contenir — article, prix, etc. — et quels éléments de la liste sont déjà présents.

### [**La Vue**]

La vue définit comment les données de l'application doivent être affichées.

Dans notre application de liste de courses, la vue définirait comment la liste est présentée à l'utilisateur et recevrait les données à afficher à partir du modèle.

### [**Le Contrôleur**]

Le contrôleur contient une logique qui met à jour le modèle et/ou la vue en réponse aux entrées des utilisateurs de l'application.

Ainsi, par exemple, notre liste d'achats pourrait avoir des formulaires de saisie et des boutons qui nous permettent d'ajouter ou de supprimer des éléments. Ces actions nécessitent la mise à jour du modèle, de sorte que l'entrée est envoyée au contrôleur, qui manipule ensuite le modèle le cas échéant, qui envoie ensuite des données mises à jour à la vue.

Cependant, vous pouvez également mettre à jour la vue pour afficher les données dans un format différent, par exemple, changer l'ordre des éléments en alphabétique ou le prix le plus bas en prix le plus élevé. Dans ce cas, le contrôleur pourrait gérer cela directement sans avoir besoin de mettre à jour le modèle.














