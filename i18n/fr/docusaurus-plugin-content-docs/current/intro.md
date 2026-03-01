---
sidebar_position: 1
title: "Introduction"
---

# AAM (Abstract Alias Mapping)
## Présentation d'AAM
Les fichiers de configuration ont tendance à croître de manière incontrôlée. Ils deviennent volumineux, difficiles à lire et encore plus difficiles à maintenir. Les diviser en plusieurs fichiers aide, mais ne résout pas la complexité sous-jacente de la gestion des relations de données. Nous avions besoin d'un moyen plus intuitif de gérer les mappings — nous avions besoin d'AAM.
### Le problème - Le Mapping Verbeux
Imaginez que vous devez gérer un grand ensemble d'alias bidirectionnels (où vous pouvez chercher une clé par sa valeur et vice-versa). Dans des formats comme TOML, vous êtes contraint d'écrire beaucoup de code répétitif :
```toml
[alias]
a = "b"
b = "a"
```
Ce sont trois lignes pour un seul mapping. Multipliez cela par cent, et votre configuration devient un cauchemar.
### La solution - AAM
AAM est une syntaxe simple et élégante qui vous permet de définir des mappings bidirectionnels en une seule ligne. Avec AAM, vous pouvez écrire :
```aam
a = b
```
Cette unique ligne crée un mapping bidirectionnel entre `a` et `b`. Vous pouvez chercher `a` pour obtenir `b`, et chercher `b` pour obtenir `a`. C'est concis, clair et élimine le code répétitif.
AAM est conçu pour être concis, lisible et facile à utiliser, en supprimant le boilerplate afin que vous puissiez vous concentrer sur la logique de votre configuration.
## Comment l'idée est née
Je travaillais sur un projet qui m'obligeait à gérer un grand nombre d'alias. J'utilisais TOML pour mes fichiers de configuration, et j'ai trouvé qu'il était très difficile de gérer mes alias. Je devais écrire beaucoup de code répétitif pour les gérer, et il était très facile de faire des erreurs. Je voulais une meilleure façon de gérer mes alias, et c'est comme ça que l'idée d'AAM m'est venue.
## Démarrer
Prêt à simplifier vos configurations ? Consultez le [Guide de démarrage rapide](using/getting-started) pour apprendre à utiliser AAM dans vos projets.
