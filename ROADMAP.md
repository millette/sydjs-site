# Roadmap RoLLodeQc

## Étapes

### Site alpha (voir ci-bas)
* Basé sur SydJS/Keystone 0.4.0-alpha avec MongoDB 3.2
    * Enlever meetups, talks rsvp et updater le frontpage
    * Enlever showbag
* Login par github (SydJS)
* Association au compte Twitter (SydJS)
* Partage de token github pour accélérer le scrapping
* Fil aggrégé twitter/github/blog
* Blogue/news du site (SydJS, rss à faire)
* Sitemap (visible et machine)
* Français, *mostly* ([i18n-node](https://github.com/mashpie/i18n-node) pour un site bilingue)

### Trouver des sponsors
Par exemple:

* Plotly
* SFL (1500$ déjà)
* membres de l'APELL
* membres de yuldev

## Composantes

### Site avec user login
* https (letsencrypt avec nginx, keystone/nodejs, couchdb)
* passport (github, gitlab, bitbucket, openhub, twitter) (SydJS)
* passport, more (facebook, g+) (SydJS)
* keystone: express, mongoose, jade (or ejs - mais SydJS utilise jade)
* theme bootswatch (less bootstrap avec SydJS)
* profil utilisateur public (SydJS)

### Scrappers
* users (github, gitlab, bitbucket, etc.)
* projects (github, gitlab, bitbucket, etc.)
* groups (github, gitlab, bitbucket, etc.)
* activities (github, gitlab, bitbucket, etc.)
* rss (planet)

### Visualisations
* plotly?
* listes
* stats
* maps
* graphiques (lignes, barres)

### Données historiques
* croissance
* etc.

## Modèles

### Users
* type (programmeur, traducteur, support, etc.)
* location (ville du Québec)
* bio
* photo/avatar
* site web/rss
* disponible (hireable)
* email
* source (github, bitbucket, etc.)
* id
* prénom, nom

### Projets

### Groupes

## Divers

### Rôles
* admin
* self
* dev
* cie

### Permissions des champs
* Voir
* Éditer

## Dépendances
<dl><dt>Maintenant<dd>Keystone 0.3 avec MongoDB 3.0
<dt>Éventuellement<dd>Keystone 0.4 avec MongoDB 3.2</dl>

* [SydJS][]
* Keystone (0.3: mongoose 3.8; 0.4: 4.0)
* Mongoose (~3.8.22, 4.x: MongoDB 3.0; >=4.3.0: 3.2)
* MongoDB
* WiredTiger (disponible dans MongoDB 3.0, par défaut dans 3.2)

[SydJS]: https://github.com/JedWatson/SydJS-site