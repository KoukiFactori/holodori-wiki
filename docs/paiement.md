---
sidebar_position: 3
title: Résoudre les problèmes de paiement
description: Ce qu'il faut faire lorsque le paiement échoue dans hololive Dreams avec un compte Google ou Apple créé pour une autre région.
---

## Le problème

Après avoir installé le jeu avec un compte créé pour une autre région (voir la page [Installation](./installation.md)), il arrive que le paiement échoue au moment d'effectuer un achat dans le jeu. C'est généralement dû au fait que le compte, ou son profil de paiement, n'est pas (ou plus) associé au bon pays.

Si vous êtes dans ce cas, la marche à suivre ci-dessous permet de vérifier et de corriger la situation.

## Android

**Toutes les étapes sont à effectuer en étant connecté au VPN**, sur un serveur du pays dans lequel le compte Google a été créé.

### Vérifier la localisation du compte

1. Allez dans les paramètres du compte Google que vous avez créé.
2. Ouvrez l'onglet **Données et confidentialité**, puis descendez jusqu'à la section **Outils** et cliquez sur **Google Dashboard**.
3. Dans le Dashboard, vérifiez que vous êtes bien localisé dans le pays où vous avez créé le compte Google avec le VPN.
4. Si ce n'est pas le cas, regardez si Google vous propose de changer de pays en ajoutant une méthode de paiement.

### Corriger le profil de paiement

1. Toujours dans Google Dashboard, ouvrez la section **Paiements** (Google Pay).
2. Mettez le profil de paiement sur le pays qu'il faut, ou supprimez carrément le profil FR s'il en existe un.

Une fois le profil corrigé, retentez l'achat dans le jeu.

## iOS

Sur iOS, l'achat passe par le compte Apple américain utilisé pour installer le jeu. PayPal n'est pas une option : votre compte PayPal est associé à la France, il sera systématiquement refusé.

### Ajouter une carte bancaire

Contrairement à la création du compte, où une adresse de facturation aléatoire suffit, l'adresse renseignée compte réellement à cette étape.

1. Dans l'**App Store**, connecté avec votre compte américain, ouvrez les réglages du compte puis la section **Moyen de paiement**.
2. Modifiez l'adresse de facturation et renseignez votre véritable adresse.
3. Pour le code postal (ZIP code), cherchez quel état des États-Unis « correspond » au vôtre.
4. Vous pouvez alors ajouter votre carte bancaire sans souci.

:::warning
Le code postal choisi n'est pas anodin : certains états appliquent des règles strictes concernant les achats en ligne effectués par des mineurs. C'est le cas du Texas, dont les codes commencent par 75XXX, ce qui correspond aussi aux codes postaux parisiens. Si votre vrai code postal vous amène vers un état de ce type, Apple réclamera une vérification supplémentaire (une carte de débit américaine, ou des papiers d'identité américains). Dans ce cas, **l'ajout de la carte est impossible**.
:::

### Utiliser une carte cadeau

Si l'ajout d'une carte bancaire est bloqué, vous pouvez vous rabattre sur les cartes cadeaux App Store américaines, achetables en ligne.

:::warning
N'achetez pas de carte cadeau dans un magasin français : ce sont des cartes App Store **France**, elles ne peuvent pas être créditées sur un compte américain.
:::
