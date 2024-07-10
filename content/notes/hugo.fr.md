---
title: Hugo
date: 2024-03-08T15:47:28.529Z
---
# Hugo

## Disponibilité de node_modules dans Hugo

[Hugo](https://gohugo.io) s'appuie sur [esbuild](https://esbuild.github.io) pour bundler les assets et celui-ci utilise automatiquement `node_modules` comme dossier de résolution. Il est donc pas nécessaire de [monter](https://gohugo.io/hugo-modules/configuration/#module-configuration-mounts) une dépendance pour l'importer et l'utiliser en JavaScript.

[Source](https://gohugo.io/hugo-pipes/js/#include-dependencies-in-packagejson--node_modules)

Mais _'tention hein_, vous pourriez toujours avoir besoin de monter un dossier de `node_modules` pour, par exemple, manipuler une ressource.

## Hugo i18n Redirection automatique des langues

- https://nanmu.me/en/posts/2020/hugo-i18n-automatic-language-redirection/

## Installer une version spécifique de Hugo avec Brew

1. Télécharger le [fichier hugo.rb](https://github.com/Homebrew/homebrew-core/blob/master/Formula/h/hugo.rb) de la version souhaitée sur le dépot de homebrew-core
2. `brew unlink hugo`
3. `brew install hugo.rb`
