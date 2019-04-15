# Digital_Clock_Vue

Widget pour Jeedom permettant d'afficher une horloge digitale intégrant la date et l'heure avec affichage des secondes à partir d'un virtuel.

<img src="/icon.png" alt="présentation"/>

>**Important**: le plugin "Virtuel" doit être installé et activé.

Après avoir téléchargé le widget il est nécessaire de créer un nouveau virtuel en cliquant sur le bouton "**+Ajouter**", de lui donner un nom (*"Horloge"* par exemple) et de valider en cliquant sur la case "**D'accord**":
<img src="/doc/newVirt.jpg" alt="nouveau virtuel"/>

Sélectionner un "**Objet parent**" dans l'onglet *"Equipement"* et cocher les cases "**Activer**" et "**Visible**" puis enregistrer en cliquant sur le bouton "**Sauvegarder**":
<img src="/doc/equConfig.jpg" alt="Config Equipement"/>

Passer sur l'onglet *"Commandes"* et cliquer sur "**Ajouter une info virtuelle**":
<img src="/doc/addCommand.jpg" alt="Ajout commande"/>

Donner un nom à la commande nouvellement créée (*"horloge"* par exemple) et sélectionner le *Sous-type*: "**Autre**" puis décocher la case "**Historiser**". Enregistrer en cliquant sur "**Sauvegarder**":
<img src="/doc/addCommand2.jpg" alt="Ajout commande 2"/>

Cliquer sur le bouton représentant une roue crantée pour accéder à la configuration de la commande puis sélectionner le widget "**Digital_Clock_Vue**" dans l'onglet *"Affichage"* - rubrique *"Widget"* puis cliquer sur "**Enregistrer**":
<img src="/doc/config.jpg" alt="config commande"/>

Sauvegarder le virtuel, l'horloge est à présent installée et fonctionnelle.

---------------------------

Pour aller plus loin, il est possible de choisir la couleur d'affichage de l'horloge.

Pour se faire cliquer sur le bouton "**Configuration avancée**" du virtuel afin d'accéder à la configuration de l'équipement et aller sur l'onglet *"Affichage"*. Dans la rubrique *"Widget"* à la ligne *"Couleur du texte"* vous pouvez sélectionner la couleur de l'horloge indépendamment sur le Dashboard, le Design ou sur une Vue:
<img src="/doc/configColor.jpg" alt="config couleur"/>

>Exemples de rendu:   
><img src="/doc/exemples.jpg" alt="exemples"/>
