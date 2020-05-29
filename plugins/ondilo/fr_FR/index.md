---
title: Jeedom | Plugin Ondilo - ICO
description: Les flotteurs de la gamme Ico conçus par la société Ondilo sont des capteurs Wifi qui permettent l'analyse de votre piscine ou de votre SPA.
---

<img align="right" src="../images/ondilo_icon.png" width="100">

# ondilo - Plugin pour Jeedom

*→ [Lien market](https://market.jeedom.com/index.php?v=d&p=market&type=plugin&plugin_id=3945)*<br />

Les flotteurs de la gamme Ico conçus par la société Ondilo sont des capteurs Wifi qui permettent l'analyse de votre piscine ou de votre SPA. Installation rapide, connexion Wi-Fi compatible piscines sel, brome ou chlore.. Le plugin Ondilo - ICO pour jeedom vous permet de remonter les informations mises à disposition tels que: 

- La température de l’eau, 
- L’acidité (pH), Le redox (ORP), 
- Le sel, 
- Total des Solides Dissous (TDS), 
- ou encore les recommandations. Il vous est également possible de valider les recommandations depuis un scénario. (Exemple: je dois mettre du chlore, un bouton est situé à côté permet de valider l’action). 

[Changelog](changelog.md)<br />

## Installation du plugin Ondilo - ICO

L'installation du plugin se fait depuis l'interface gestion des plugins et / ou depuis le market.

## Configuration du plugin Ondilo - ICO

Dans un premier temps vous devez vous authentifier à votre compte Ondilo depuis la page de configuration.

{% include lightbox.html src="ondilo/images/authentification-a-api-ondilo.png" data="ondilo" title="Authentification à l'api Ondilo" imgstyle="width:550px;display: block;margin: 0 auto;" %}

Une nouvelle page va s'ouvrir, vous devez renseigner vos identifiants. (Pas de craintes vous êtes sur le site d'ondilo le fabriquant de l'ICO. Le plugin ne sauvegarde aucun ni login, ni mot de passe).

**ATTENTION** le choix de la langue est important, car les recommandations seront dans la langue sélectionnée.

{% include lightbox.html src="ondilo/images/authentification-ondilo.png" data="ondilo" title="Authentification à l'api Ondilo" imgstyle="width:550px;display: block;margin: 0 auto;" %}

Une fois connecté, vous revenez sur une page blanche. Vous pouvez fermer celle-ci et recharger votre page de configuration.

Vous pouvez choisir d'utiliser la tuile personnalisé ou les widgets natifs à jeedom. A vous de choisir en cochant cette option.

{% include lightbox.html src="ondilo/images/activer-widget-custom.png" data="ondilo" title="Activation widget personnalisé" imgstyle="width:550px;display: block;margin: 0 auto;" %}

Ce qui donnera:

> Widget Natif

{% include lightbox.html src="ondilo/images/standard-ondilo-widget-jeedom.png" data="ondilo" title="Widget Natif" imgstyle="width:550px;display: block;margin: 0 auto;" %}

> Widget (Tuile) personnalisé

{% include lightbox.html src="ondilo/images/custom-ondilo-widget-jeedom.png" data="ondilo" title="Widget Natif" imgstyle="width:550px;display: block;margin: 0 auto;" %}

### Synchronisation de votre Ondilo - ICO

Il est possible d'avoir plusieurs ilots ICO.

{% include lightbox.html src="ondilo/images/synchronisation-jeedom-ondilo-ico.png" data="ondilo" title="Synchronisation des ilots" imgstyle="width:550px;display: block;margin: 0 auto;" %}

#### Les équipements

Pour savoir ce qu'est un équipement je vous invites à lire les [Concepts Jeedom sur les équipements](https://doc.jeedom.com/fr_FR/concept/#tocAnchor-3)

##### Un ilot ICO
Un îlot ICO est un équipement dans Jeedom, ainsi, il dispose de commande type informations ou actions. Voici la liste des commandes:

- (info) Température
- (info) Acidité (pH)
- (info) Désinfection (ORP)
- (info) Sel si piscine au sel
- (info) Conductivité (TDS)
- (info) Puissance du signal WIFI (dB)
- (info) Vu Dernière Fois
- (action) Rafraichir 

Un équipement dispose d'un paramètre permettant d'indiquer le niveau de batterie. Vous pouvez retrouver l'info sur le widget ou dans la partie: Analyse > Equipements : exemple https://jeedom.local/index.php?v=d&p=eqAnalyse

{% include lightbox.html src="ondilo/images/ondilo-battery.png" data="ondilo" title="Analyse des équipements, niveau de batterie" imgstyle="width:550px;display: block;margin: 0 auto;" %}

##### Les recommandations

Les recommandations sont visibles dans le centre de message:

{% include lightbox.html src="ondilo/images/centre-de-message-jeedom-recommandations-ondilo.png" data="ondilo" title="Synchronisation des ilots" imgstyle="width:550px;display: block;margin: 0 auto;" %}

## FAQ

Est ce que le plugin utlise des API tierces ?

Oui le plugin utilise l'[api officielle de Ondilo](https://interop.ondilo.com/docs/api/customer/v1/).

## Remerciements

