Ce système de documentation utilise [Hugo](https://gohugo.io). Contrairement aux autres outils de génération de site static, Hugo est un unique binaire à copier dans votre PATH.

## Installation

La procédure d'installation d'Hugo est accessible [via ce lien](https://gohugo.io/getting-started/quick-start/).

## Pour démarrer

```
git clone https://github.com/govpf/helpthemall
cd helpthemall
hugo server --disableFastRender
```

Vous vous connecterez sur votre page via le lien suivant : [http://127.0.0.1:1313](http://127.0.0.1:1313)

## Contenu

Le contenu de la documentation se trouve dans le répertoire "content".

### Les sujets

Dans notre configuration, nous allons considérer les répertoires de premier niveau comme des sujets affichés sur la landing page. En réalité, il suffit d'ajouter dans un fichier l'entête suivante pour qu'il s'affiche en première page :

```
---
title: "MON_TITRE"
description: "MA_DESCRIPTION"
icon: "MON_ICONE"
draft: false
type: docs
weight: 1
---
```

Le paramètre weight indique la position du sujet par rapport aux autres sujets.

### Les articles

Pour créer un article, il suffit de rajouter l'entête suivant dans un fichier texte :

```
---
title: "MON_TITRE"
draft: false
---
```

La position de l'article dépends du répertoire dans lequel il est stocké dans l'arborescence.

## Pour contribuer

Vous pouvez contribuer de deux façons :

- en nous indiquant les sujets ou thèmes à aborder dans cette documentation ([un sujet/thème par issue](https://github.com/govpf/helpthemall/issues)).
- en intégrant une team pour l'écriture des documents concernant un sujet.

### Pour les rédacteurs

Pour contribuer, il suffit de nous envoyer vos articles sous forme de branches. Passez faire un tour sur la [documentation de Gitflow](https://guides.github.com/introduction/flow/) si vous n'êtes pas familiés avec le concept.

Une fois vos modifications acceptées, elle seront automatiquement disponible sur le lien suivant : [https://govpf.netlify.app/](https://govpf.netlify.app/)

Merci !
