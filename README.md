# Video Platform

## Durée

Le projet se déroule du 22 novembre au 3 décembre.  
> Une présentation sera requise le 3 décembre après-midi.

## Objectif

Réaliser une interface complète de plateforme vidéo dans le style Netflix, Amazon Vidéo, Disney +, Hulu, ...  
Il s'agit d'un prototype fonctionnel et complet afin de montrer au client le résultat final de son projet.

> :warning: **Aucun streaming ne doit apparaître sur le projet, mais si vous souhaitez ajouter une vidéo, 
> vous pouvez remplacer le streaming par la bande-annonce officiel du film ou de la série tv.**

## Rappel

**Chacun apprend à sa vitesse.** Vous devez faire preuve de patience quand le projet n'avance pas aussi vite que vous le souhaitez, prendre le temps d'expliquer à vos collègues le travail que vous avez effectué et laisser le temps à vos collègues de réaliser le leur. Sachez répartir la masse de travail entre vous et ne faites pas le travail des autres.

## Demandes requises

* SASS ;
* Utilisation de la méthodologie [BEM](https://fr.wikipedia.org/wiki/BEM) pour vos fichiers SASS ;
* Utilisation de GitHub pour le dépôt du projet ;
* Création des modèles de toutes les pages du site ;
* Déploiement du site sur un serveur.

### Options

Il s'agit d'éléments supplémentaires qui peuvent être ajoutés au projet et qui apporteront ou amélioreront des compétences :

* Bien gérer vos commits : https://buzut.net/cours/versioning-avec-git/bien-nommer-ses-commits ;
* Utilisation du [Git Flow](https://grafikart.fr/tutoriels/git-flow-742) pour l'organisation du projet ;
* Utilisation d'un [Linter](https://mindsers.blog/fr/post/linting-good-practices/) pour garder le code propre et conforme à la norme ;
* Déployer le projet sur le serveur en SSH et avec Git.

## Datas

Les données qui apparaîtront sur le prototype seront toutes extraites de l'API du site TheMovieDb : https://developers.themoviedb.org/3/getting-started/introduction

# Spécifications

## Navigation

L'application doit comporter une barre de navigation contenant le titre (et/ou logo), un menu dropdown contenant tous les
différents genres de films et un moteur de recherche.

### Genres

Au clic sur un genre, le visiteur sera redirigé vers une page contenant les 200 premiers films trouvés correspondant au genre choisi.  
Ils devront être paginés à raison de 20 par pages.

### Résultats de la recherche

Les résultats doivent se situer sur une nouvelle page contenant les 200 premiers résultats trouvés (films et séries tv).  
Ils devront être paginés à raison de 20 par pages.

> Si aucun résultat n'est trouvé, un message d'erreur doit s'afficher.

## Homepage

La page d'accueil doit comporter quatre sections :  

* Les 20 films/séries tv les plus tendances ;
* Les 20 films/séries tv les mieux notés ;
* Les 20 films/séries tv les plus populaires ;
* Les 20 comédiens les plus populaires.

Dans les trois premières sections, il doit être possible d'alterner entre les films ou les séries tv. Les deux types ne
peuvent être affichés en même temps.  
**Un menu de filtre est donc nécessaire par section.**

> L'ordre des sections n'est pas figées.

Pour les trois sections affichant des films/séries tv, un minimum d'informations doit apparaître tel que :

* Le titre du film/séries tv ;
* La popularité du film/séries tv ;
* La jaquette du film/séries tv.

La dernière section, celle concernant les artistes populaires. Afficher les éléments suivants :

* Photo de l'artiste ;
* Son prénom et son nom.

> Il est possible d'afficher plus d'informations sur les films ou artistes tant que cela n'est pas une surcharge 
> pour le visiteur.

## Détails d'un film

Au clic sur un film ou série tv, le visiteur sera redirigé vers une page contenant les détails de celui-ci :

* L'image de fond ;
* Jaquette ;
* Titre ;
* Année de sortie ;
* Synopsis ;
* Langue original ;
* Le vote moyen ;
* Les genres ;
* Les différentes productions ;

Les genres du film doivent être cliquables. 

En dessous de ces détails, on trouvera deux sections :
* Le casting complet du film :
  * Photo de l'acteur/actrice ;
  * Prénom et nom de l'acteur/actrice ;
  * Rôle de l'acteur/actrice.
* Les 20 recommandations de films/séries tv par rapport au film choisi.

> Si aucune recommandation n'est trouvée, un message d'erreur doit s'afficher.

## Artistes

Au clic sur un artiste depuis la page d'accueil, le visiteur sera redirigé vers une page contenant les détails de celui-ci :

* Photo de l'artiste ;
* Nom et prénom ;
* Biographie ;
* Date de naissance ;

En dessous de ces détails, on trouvera la filmographie de cet artiste qui doivent aussi être cliquable afin d'avoir 
les détails du film choisi.

## Notes

Il peut arriver que certaines images comme les jaquettes ou fonds de page soient inexistantes. Dans ce cas, afficher 
une image par défaut. 
