---
title: 'Mes débuts avec Hugo'
date: 2023-11-14T11:39:24+01:00
draft: false
tags: ["blog", "hugo"]
categories: ["Développement Web", "GitHub-Pages"]
author: 'Samuel LUNION'
summary: 'Voici ma première expérience avec Hugo, un générateur de site statique.'
featured_image: '/HETIC-gitpages/img/hugo.png'
---

# Découverte de Hugo 

![Image d'entête](/HETIC-gitpages/img/hugo-logo-wide.svg)

Bonjour à tous ! C'est Samuel LUNION, et je suis ravi de partager avec vous ma première expérience avec Hugo, un générateur de site statique.

## Contexte

Ayant récemment commencer un MT4 CTO tech lead, j'ai était iniciée a Github Pages afin de créer mon propre blog pour partager mes découvertes, astuces et projets. Après avoir exploré différentes options, j'ai choisi Hugo pour sa simplicité, sa rapidité et sa flexibilité.

## Installation de Hugo

L'installation de Hugo s'est avérée être trés simple. En utilisant scoop, j'ai pu installer hugo rapidement :

```bash
$ scoop install hugo-extended
```

## Création de siteavec contenue & deploiment avec Github pages

Utiliser Hugo a facilité la création de mon premier site avec le thème "Ananke". Les fichiers nécessaires se sont automatiquement créés, accélérant ainsi le processus de mise en place.
Pour rendre mon site un peux plus vivant j'ai du r'ajouter du contenu sous forme d'articles ou de posts, Hugo simplifie également cette étape. 
```bash
$ hugo new post/mon_premier_article.md
```
Un nouveau fichier Markdown est généré dans le dossier "content" du projet. Cela pré-remplit le Front Matter avec des informations par défaut telles que la date de création, le statut de brouillon, etc.
```bash
---
title: "My First Post"
date: 2022-11-20T09:03:20-08:00
draft: true
---
```
Grâce à l'utilisation de GitHub Pages, le déploiement de mon site Hugo a été simplifié. Après avoir configuré les paramètres de la bonne branche sur GitHub Pages et suivi les étapes recommandées, mon site est désormais en ligne et accessible à l'adresse https://unitigris.github.io/HETIC-gitpages/.


## Automatisation Github pages

L'inconvénient de cette méthode est que la création d'une branche spécifique pour GitHub Pages peut entraîner une duplication de mon code, avec une branche dédiée aux fichiers générés pour le site. En automatisant le déploiement avec GitHub Actions, j'ai pu surmonter ces inconvénients et bénéficier d'avantages. Cela m'a permis une intégration continue, ce qui signifie que chaque fois que je pousse des modifications dans ma branche principale, une action peut être déclenchée pour générer et déployer automatiquement le site.


