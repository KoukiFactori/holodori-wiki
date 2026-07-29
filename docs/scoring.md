---
title: Skills/Scoring System - Deep Dive
description: Explication détaillée du système de scoring et de skills d'hololive Dreams et des effets relatifs aux cartes
---

:::warning

En cours d'écriture, certaines informations pourront changer au fil du temps.

:::


## Intro

Si c'est votre premier jeu de rythme sur mobile ou que vous êtes un joueur "casual", le nombre d'informations présents dans le jeu dès le départ peut rapidement vous embrouiller. Entre le système d'`Holomem Board`, les skills, les effets sur le score et bien d'autres encore, il devient vite nécessaire de mettre les choses à plat pour ne rien manquer dès le départ.

## Holomem

Cette section concerne le fonctionnement des holomems. Chaque holomem se débloque en complétant sa quête associée (Deux quêtes sont proposées chaque jour grauitemement, avec la possibilité d'en inviter plus en échange de `holomem Invitation`).
Récupérer une holomem permet de l'utiliser comme `leader`, d'avoir accès au `Score Rating` de l'holomem ainsi que de débloquer l'accès à l'`holomem Board`.

Le fonctionnement précis du `leader` sera détaillé dans la section suivante, son utilité n'ayant aucun impact pour la suite de cette section.

### Holomem Score Rating

Le `Holomem Score Rating` est un leaderboard dédié à chaque membre permettant de classer les joueurs avec le plus de points sur une membre. Afin de gagner des points sur ce leaderboard, il est nécessaire de jouer certaines musiques spécifiques en ayant mis l'holomem en tant que `leader`. Chaque membre possède une liste de musiques donnée par le jeu. Chaque partie jouée en respectant ces conditions donnera un `Rate` sur la musique, le meilleur `Rate` étant conservé pour la suite.
Afin d'établir le `Score Rating` final, le jeu ne conserve que les **trois** meilleurs ratings et les additionne.

Par exemple, Shiori dispose de 4 musiques éligibles au `Holomem Score Rating`:  
    - Kyoufuu All Back  
    - Megistune  
    - Monsters and Men  
    - Rebellion  
Admettons que je joue chaque musique et que j'obtienne un `Rate` de 196, 103, 183 et 180 respectivement. Megitsune étant la chart avec le `Rate` le plus bas, elle est éliminée du processus. La somme des trois autres musiques donne un total de 559 points de `Holomem Score Rating`, me permettant de me classer 92eme à l'heure actuelle où j'écris ces lignes.

Après un certain temps, les joueurs les mieux classés reçoivent une récompense temporaire (comme un badge).
Note: Le classement n'est pas réinitialisé entre les périodes.


**Instant maths:**  
Avec quelques parties servant de données, il est très vite possible de retrouver la formule utilisée pour calculer tous les `Ratings`.
Le système actuel attribue **100 Rate** par tranche de **500k points**. On obtient alors la formule suivante: $1\text{ Point} = 0.0002 \text{ Rate}$.

| Score     | Rate |
|-----------|------|
|   500 000 |  100 |
|   625 000 |  125 |
|   750 000 |  150 |
| 1 000 000 |  200 |
| 1 500 000 |  300 |
| 2 000 000 |  400 |

Bien sûr, une telle formule donnera lieu à des nombres à virgule qui n'apparaissent pas dans le jeu tels quels. Après conversion du score, le jeu effectue un arrondi à l'entier supérieur, un rate de 341.0866 vaudra en réalité 342.  

### Holomem Board



## Members

## Unit Setup

## Live

## Sources

[Tweet du compte officielle sur le Holomem Score Rating](https://x.com/holo_dreams_en/status/2081258216856715716)