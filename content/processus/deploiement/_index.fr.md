---
title: "Processus de déploiement"
description: "Processus de déploiement des services numériques"
date: 2021-10-15T09:29:49-10:00
icon: "ti-book"
type: docs
draft: false
weight: 3
keywords: ["processus", "deploiement", "continu", "container", "cloud"]
---

Nous utilisons aujourd'hui plusieurs processus de déploiement. Ces
déploiements peuvent être continu ou nécessiter une action manuelle
selon le contexte.

## Déploiement sur des orchestrateurs de containers

Nous privilégions le déploiement de nos services numériques via des orchestrateurs de containers.

Nous déployons nos environnements de dev dans un cluster Kubernetes sur AWS et nos environnements de préproduction et de production dans des clusters swarm en intranet.

[schema déploiement via orchestrateur de containers](/images/dpl-swarm-k8s.png)

Pour ce faire, on installe un runner gitlab dans chaque cluster et nous installons les applications via des pipelines.
