Ce système de documentation utilise [Hugo](https://gohugo.io). Contrairement aux autres outils de génération de site static, Hugo est un unique binaire à copier dans votre PATH.

## Installation

La procédure d'installation est accessible [via ce lien](https://gohugo.io/getting-started/quick-start/).

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

Pour contribuer, il suffit de nous envoyer vos articles sous forme de branches. Passez faire un tour sur la [documentation de Gitflow](https://guides.github.com/introduction/flow/) si vous n'êtes pas familier avec le concept.

Une fois vos modifications acceptées, il sera automatiquement disponible sur le lien suivant : [https://govpf.netlify.app/](https://govpf.netlify.app/)

Merci !
