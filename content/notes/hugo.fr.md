---
title: Hugo
date: 2024-03-08T15:47:28.529Z
---
# Hugo

## Disponibilité de node_modules dans Hugo

[Hugo](https://gohugo.io) s'appuie sur [esbuild](https://esbuild.github.io) pour bundler les assets et celui-ci utilise automatiquement `node_modules` comme dossier de résolution. Il est donc pas nécessaire de [monter](https://gohugo.io/hugo-modules/configuration/#module-configuration-mounts) une dépendance pour l'importer et l'utiliser.

Il me semble que cela n'a pas toujours était le cas. Il y quelques mois, j'avais besoin de monter les dépendances dont j'avais besoin. Je suppose qu'une mise à jour de Hugo a changé ce comportement sur la disponibilité du répertoire `node_modules` dans la résolution de chemin.

[Source](https://gohugo.io/hugo-pipes/js/#include-dependencies-in-packagejson--node_modules)
