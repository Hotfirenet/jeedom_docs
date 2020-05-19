---
title: Jeedom | Plugin Grocy
description: Plugin Grocy pour le système domotique Jeedom. Grocy est un ERP permettant la gestion de stock de vos aliments et de vos tâches ménagères. Le système Grocy est open source est auto-hébergé. 
---

<img align="right" src="../images/grocy_icon.png" width="100">

# Grocy - Plugin pour Jeedom

*→ [Lien market](https://www.jeedom.com/market/index.php?v=d&p=market&type=plugin&plugin_id=3945)*<br />

Plugin Grocy pour le système domotique Jeedom. Grocy est un ERP permettant la gestion de stock de vos aliments et de vos tâches ménagères. Le système Grocy est open source est auto-hébergé. 
Vous devez au préalable avoir un système Grocy fonctionnel !

[Changelog](changelog.md)<br />

[Principe de fonctionnement de Grocy](#installation-de-grocy)<br />
[Intallation de Grocy](#installation-de-grocy)<br />
[Configuration du plugin Grocy](#configuration-du-plugin-grocy)<br />
[Première utilisation](#premiere-utilisation)

## Principe de fonctionnement de Grocy

Le principe du plugin Jeedom pour Grocy, est de scanner le code barre d'un produit et d'ajouter ou de supprimer un produit de votre sytème de gestion d'épicerie. 

Pour scanner le produit, vous pouvez utiliser une application mobile.

{% include lightbox.html src="grocy/images/Workflow-Jeedom-2-Grocy.jpg" data="grocy" title="Principe de fonctionnement" imgstyle="display: block;margin: 0 auto;" %}

https://docs.google.com/drawings/d/1g8rvMz-nGeV2KoqWBMqqui6cWDNtPPV5vTQCnpPCyx0/edit?usp=sharing

## Intallation de Grocy

Il y a 3 possibilités pour installer Grocy

- Sous la forme d'une [Application Windows](https://github.com/grocy/grocy-docker#grocy-on-docker)
- [Nativement](https://github.com/grocy/grocy#how-to-install),
- [Via Docker](https://github.com/grocy/grocy-docker#grocy-on-docker)


## Installation du plugin Grocy

L'installation du plugin se fait depuis l'interface gestion des plugins et / ou depuis le market

## Configuration du plugin Grocy

Vous devez avoir au préalable une instance Grocy. Sur l'inteface de grocy 

{% include lightbox.html src="grocy/images/creation-token-grocy.png" data="grocy" title="Création du token" imgstyle="width:550px;display: block;margin: 0 auto;" %}

{% include lightbox.html src="grocy/images/generation-token-grocy.png" data="grocy" title="Génération du token" imgstyle="width:550px;display: block;margin: 0 auto;" %}

Une fois le token généré, rendez vous dans la configuration du plugin Grocy

{% include lightbox.html src="grocy/images/configuration-jeedom.png" data="grocy" title="Configuration du plugin Grocy" imgstyle="width:550px;display: block;margin: 0 auto;" %}

La commande de notification vous permez d'être notifié lorsque vous passez dans un mode. 

Pensez à valider la configuration et à activer le panel.

## Configuration de l'application mobile

La configuration est propre à votre application. vous pouvez utiliser l'url mis à disposition sur la page du plugin.


## Utilisation du plugin Grocy

Faites une synchronisation de Grocy vers Jeedom. La synchronisation va créer des objets qui sont vos emplacements. Puis les produits seront synchronisés.

Il ne vous reste plus qu'a scanner vos produits depuis l'app et ceux ci seront automatiquement ajoutés ou supprimés.

Si le produit n'existe pas, une recherche est faite sur [openFoodFact](https://fr.openfoodfacts.org/), si une correspondance est faite via le code barre alors celui ci sera ajouté à votre instance Grocy apres une validation de votre part.

## Remerciements

Benoit BRETON 






