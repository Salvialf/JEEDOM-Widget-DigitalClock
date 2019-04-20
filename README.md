# Digital_Clock_Vue

Widget pour Jeedom permettant d'afficher, à partir d'un virtuel, une horloge digitale intégrant la date et l'heure avec affichage des secondes.

<img src="/icon.png" alt="présentation"/>

>**Important**: le plugin "Virtuel" doit être installé et activé.

## Installation:  
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

## Paramètres optionnels:  
De nombreux paramètres optionnels sont inclus afin d'être en mesure de générer une horloge unique en fonction des goûts de chacun. L'ensemble des paramètres est rappelé au début du code du widget.

#### Date:  
* **datefont**: permet de sélectionner la police d'écriture *(ou "font")* pour la date.
* **datesize**: choix de la taille de la date en pixels. *('20' par défaut)*
* **dateweight**: choix de l'épaisseur du texte de la date - *normal* ou *bold*. *('bold' par défaut)*
>**Astuce**: une **datesize** à 0 fait disparaître la date.

#### Heure:
* **timefont**: permet de sélectionner la police d'écriture *(ou "font")* pour l'heure.
* **timesize**:  choix de la taille de l'heure en pixels. *('45' par défaut)*
* **timeweight**: choix de l'épaisseur du texte de l'heure - *normal* ou *bold*. *('bold' par défaut)*
>**Astuce**: une **timesize** à 0 fait disparaître l'heure.

38 polices d'écritures différentes sont d'ores et déjà intégrées dans le widget. La liste de ces polices est consultable <a href="/doc/FontList.md">ici</a> et est rappelée au début du code dans le widget.  
Il est également possible d'intégrer vos propres polices d'écriture, pour se faire il suffit d'ajouter le fichier \*.ttf au widget via le bouton *"**Fichiers**"*.  
>**Astuce**: les fichiers avec l'extension \*.otf peuvent être modifiés en \*.ttf.  
>**Attention**: le nom du fichier ne doit pas comporter d'espaces et l'extension \*.ttf doit être en minuscule.

#### Horloge:
* **halo**: permet de faire apparaître ou disparaître le halo lumineux autour de l'horloge. *('on' par défaut)*

## Personnalisation avancée:  
Il est possible de choisir la couleur d'affichage de l'horloge.

Pour se faire cliquer sur le bouton "**Configuration avancée**" du virtuel afin d'accéder à la configuration de l'équipement et aller sur l'onglet *"Affichage"*. Dans la rubrique *"Widget"* à la ligne *"Couleur du texte"* vous pouvez sélectionner la couleur de l'horloge indépendamment sur le Dashboard, le Design ou sur une Vue:
<img src="/doc/configColor.jpg" alt="config couleur"/>
>Exemples de rendu:   
><img src="/doc/exemples.jpg" alt="exemples"/>

Le paramètre optionnel **halo** inclut également différents styles tels que:
* **flame**: effet flamme.
* **rainbow**: effet arc-en-ciel.
* **neon**: effet néon animé.
>Exemples de rendu:   
><img src="/doc/exempleshalo.jpg" alt="exempleshalo"/><img src="/doc/exempleneon.gif" alt="exempleneon"/>

Pour aller plus loin dans la personnalisation, il est tout à fait possible de créer 2 commandes dans le virtuel dont le widget serait appliquée sur chacune et de cacher la date sur l'une et l'heure sur l'autre (**datesize** = 0 & **timesize** = 0).


