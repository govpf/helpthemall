---
title: "Un mot sur la stack technique"
draft: false
weight: 1
date: 2021-10-09T11:02:05+06:00
lastmod: 2021-10-10T7:37:26+06:00
keywords: ["stack", "technique", "langage officiel"]
---
La stack technique est la liste de tous les outils technologiques utilisés pour développer et faire fonctionner les applications développées ou mises en oeuvre pour le Pays. C'est une combinaison d'outils et de languages de programmation qui sont utilisés en fonction des domaines d'applications.

### Norme et protocole standard

| Nom            | Description                                             |
|----------------|---------------------------------------------------------|
| RGPD           | Référentiel général de protection des données           |
| RGS            | Référentiel général de sécurité                         |
| RGI            | Référentiel général d'interopérabilité                  |
| RGAA           | Référentiel général d'accessibilité                     |
| REST           | Standard d'architecture pour API                        |
| OpenAPI        | Standard de documentation d'API                         |
| AsyncAPI       | Standard de documentation de file d'attente applicative |
| Oauth2         | Protocole de délégation d'autorisation                  |
| OpenID Connect | Protocole d'authentification                            |
| S3             | Protocole de stockage d'objets                          |

### Stack technique validée

La stack technique suivante est actuellement validée/acceptée au SIPf.

{{% notice tip %}}
Les équipes ont le choix de prendre les outils ci-dessous ou de proposer de nouveaux outils à ajouter à la liste pour expérimentation. Vous devrez ensuite pitcher votre outils au comité d'architecture en le comparant s'il y a lieu à un outils équivalent en terme de fonctionnalité et qui serait valide dans la liste.
{{% /notice %}}

#### Langage de développement

| Nom         | Version                                               |
|-------------|-------------------------------------------------------|
| Java        | Dernière version long-term support (LTS)              |
| Python      | Version 3.8                                           |
| Node.js     | Dernière version long-term support (LTS)              |
| Javascript  | ES6 / ECMAScript 2015                                 |
| Typescript  | Dernière version stable (LTS si elle existe)          |

#### Framework

| Nom            | Version                                               |
|----------------|-------------------------------------------------------|
| Spring Boot    | Dernière version stable (LTS si elle existe)          |
| Angular        | Dernière version long-term support (LTS)              |
| React          | Dernière version stable (LTS si elle existe)          |
| Vue.js         | Dernière version stable (LTS si elle existe)          |
| **Flask**      | **En expérimentation**                                |
| **FastAPI**    | **En expérimentation**                                |
| **OpenLayers** | **En expérimentation**                                |
| **Leaflet**    | **En expérimentation**                                |
| **Tensorflow** | **En expérimentation**                                |

#### Outils de versionning

| Nom         | Version                                               |
|-------------|-------------------------------------------------------|
| Git         | Dernière version stable (LTS si elle existe)          |

{{% notice note %}}
Nous avons deux outils de versionning actifs : https://gitlab.gov.pf et https://github.com/govpf.
{{% /notice %}}

#### Bases de données

| Nom           | Version                                               |
|---------------|-------------------------------------------------------|
| PostgreSQL    | Dernière version stable (LTS si elle existe)          |
| MongoDB       | Version 5                                             |
| Elasticsearch | Version 7                                             |
| **Neo4J**     | **En expérimentation**                                |
| **Redis**     | **En expérimentation**                                |

#### Message Queue

| Nom           | Version                                               |
|---------------|-------------------------------------------------------|
| **RabbitMQ**  | **En expérimentation**                                |

#### Infrastructure

| Nom           | Version                                               |
|---------------|-------------------------------------------------------|
| Docker        | Dernière version stable                               |
| Docker Swarm  | Dernière version stable                               |
| Kubernetes    | Dernière version stable                               |

{{% notice info %}}
Les services numériques que vous développez devront, obligatoirement, être livrés sous forme de conteneur Docker. La recette, le mode de construction et de déploiement doivent être totalement transparente (le code devra être hébergé dans un de nos 2 gestionnaires de code source).
{{% /notice %}}

{{% notice info %}}
Mieux vaut utiliser les conteneurs que nous construisons (au lieu de conteneurs publics), cela facilitera grandement les contrôles avant la mise en production effective de votre service numérique. Ils sont disponible à cette adresse : https://hub.docker.com/u/govpf
{{% /notice %}}

#### Reverse proxy

| Nom           | Version                                               |
|---------------|-------------------------------------------------------|
| Apache        | Dernière version stable                               |
| Nginx         | Dernière version stable                               |
| Traefik       | Dernière version stable                               |

#### Services transverses

Les services transverses sont mutualisés à la plupart des services numériques en production.

| Nom             | Description                                                                    |
|-----------------|--------------------------------------------------------------------------------|
| Gitlab          | Gestionnaire de code source                                                    |
| Github          | Gestionnaire de code source                                                    |
| Tefenua         | Service de cartographie                                                        |
| Keycloak        | Provider d'identité (Version 4.12)                                             |
| Openfisca       | Moteur de calcul centralisé                                                    |
| Alfresco        | Gestionnaire électronique de documents                                         |
| Odoo            | ERP/CRM                                                                        |
| Payzen          | Paiement en ligne                                                              |
| Timestamp       | Plateforme SaaS d'horodatage                                                   |
| Artifactory     | Gestionnaire d'artefact, utilisé aussi pour les échanges de données extérieurs |
| **Gravitee**    | **En expérimentation**                                                         |
| **CKAN**        | **En expérimentation**                                                         |
| **SendingBlue** | **En expérimentation**                                                         |
| **Mailjet**     | **En expérimentation**                                                         |

#### Les CMS

| Nom           | Version                                               |
|---------------|-------------------------------------------------------|
| Strapi        | Dernière version stable                               |
| Wordpress     | Dernière version stable                               |

{{% notice info %}}
On veillera à limiter le nombre de plugins Wordpress, aussi, une validation des plugins sera demandé lors du processus de mise en production.
{{% /notice %}}

### Les autres services

| Nom                   | Version                                               |
|-----------------------|-------------------------------------------------------|
| Démarches simplifiées | Dernière version stable                               |
| Talend                | Dernière version stable                               |
| ArcGis                | Dernière version stable                               |
| Jasper                | Dernière version stable                               |

### Stack technique dépréciée

La stack technique dépréciée comprend des outils et/ou langages de programmation anciennement utilisés au SI et désormais déconseillés pour la création de nouveaux projets.

| Nom             | Version                                               |
|-----------------|-------------------------------------------------------|
| Subversion      | Toutes les versions                                   |
| CVS             | Toutes les versions                                   |
| Evidian         | Toutes les versions                                   |
| Tapestry        | Toutes les versions                                   |
| Oracle Forms    | Toutes les versions                                   |
| Oracle Database | Toutes les versions                                   |
| Java            | Toutes les versions < 8                               |
| Spring          | Toutes les versions < 5                               |
| PHP             | Toutes les versions                                   |