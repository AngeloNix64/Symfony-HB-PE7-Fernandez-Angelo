# Symfony Projet HB Shop

Ce projet est un système de gestion de liste de produits.

### Techno

- Symfony - Framework d'application web en PHP
- Bootstrap - outils pour le développement avec HTML, CSS et JS
- Sonata Admin - fournit des fonctionnalités d'administration (Plus complexe que EasyAdmin... ;))
- Knp Paginator - paginateur Symfony

### Exigences

- PHP 7.1 - 7.4 (ATTENTION PAS 8.2 ! Sinon il y aura des problèmes avec les dépendances, j'en ai eu lorque j'ai changé du pc fixe au pc de formation...)
- MySQL
- Composer
- Twig

### Installation

Configuration de la base de donnée :

- A la racine du projet créer un fichier .env.local
- Remplir le fichier avec l'url de votre base de donnée comme l'exemple ci-dessous

```sh
APP_ENV=dev
APP_SECRET=secret
DATABASE_URL="mysql://root@127.0.0.1:3306/S-shop?serverVersion=5&charset=utf8mb4"
```

Charger la variable d'environnement :

```sh
$ source .env.local
```

Installer les dépendances

```sh
$ composer install
```

Configurer la base de données et créez le schéma à partir des migrations

```sh
$ php bin/console d:d:c
$ php bin/console d:m:m
```

Charger les fixtures

```sh
$ php bin/console d:f:l
```

Lancer le serveur

```sh
$ symfony serve --no-tls
```

### Utilisation

- Allez sur l'équivalent de ce lien en fonction de votre machine et de votre serveur http://127.0.0.1:8080/admin/login
- Connectez-vous avec le nom d'utilisateur et le mot de passe (identifiants de connexion ci-dessous)
- Ajoutez des catégories et des produits
- Allez sur la page principale pour voir une liste de catégories
- Cliquez sur un élément de la liste des catégories pour voir une liste de produits

### Connection

Nom d'utilisateur | Mot de passe 
--- | --- 
root | root 
admin | admin 

### Bilan Projet

J'ai pour une partie du projet suivi un tutoriel (d'où ma version étrange de php...).
Mais j'ai rarement autant appris en si peu de temps, donc je dirais que malgré la course que ça a été et les nombreuses erreurs venues d'un autre monde auquel je me suis confronté.. C'était quand même sympa comme expérience (VRAIMENT désolé pour le retard Lucas, je voulais au moins que le reedme soit carré, et je m'y suis aussi pris trop tard comme un débile...)
J'aurais voulu faire bien plus de choses, je le continuerai très sûrement de mon côté.