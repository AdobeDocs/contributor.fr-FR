---
title: Bases de la documentation Git et GitHub
description: Cet article donne un aperçu du référentiel Git et GitHub, ainsi que de la manière dont le contenu est organisé et dont les conventions d’attribution de noms sont utilisées pour la documentation Adobe.
exl-id: 2b2ec764-4201-4bcd-802d-a034d6675793
translation-type: tm+mt
source-git-commit: 1b1678b33059f4bc8f7aff4690f1d775e6aee2d6
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 100%

---

# Bases de la documentation Git et GitHub

## Aperçu

Si vous devez simplement apporter des modifications mineures et uniquement textuelles aux articles, il n’est pas nécessaire de comprendre les détails de cet article. Cet article décrit le workflow permettant d’apporter des modifications majeures, telles que la création d’articles, l’ajout d’images ou la modification continue de la documentation Adobe.

En votre qualité de contributeur au contenu de la documentation Adobe, vous pouvez interagir à l’aide de plusieurs outils et processus. Vous pouvez travailler simultanément avec d’autres contributeurs sur le même projet, éventuellement sur le même contenu, voire au même moment. Toutes ces opérations sont possibles grâce au logiciel Git et GitHub.

Git est un système de contrôle des versions Open Source qui permet la collaboration. Plusieurs contributeurs ainsi peuvent travailler sur des fichiers placés dans des *référentiels*.

GitHub est un service d’hébergement sur le Web pour les référentiels Git, comme ceux utilisés pour stocker les contenus [docs.adobe.com](https://docs.adobe.com). Pour tous les projets, GitHub héberge le référentiel principal, à partir duquel les contributeurs peuvent effectuer des copies pour leur propre travail.

## Git

Git dispose d’un workflow et d’une terminologie de contribution uniques pour prendre en charge son modèle distribué. Par exemple, aucun verrouillage de fichier n’est normalement associé aux opérations de passage en caisse/d’arrivée. Git permet de résoudre les modifications à un niveau encore plus détaillé, en comparant les fichiers octet par octet.

Git utilise également une structure à niveaux pour stocker et gérer le contenu d’un projet :

- *Référentiel* : également appelé *repo*. Il s’agit de la plus grande unité de stockage. Un référentiel contient une ou plusieurs branches.
- *Branche* : tous les référentiels contiennent une branche par défaut (généralement appelée « principale ») et une ou plusieurs branches devant être fusionnées à nouveau dans la branche principale. La branche principale sert de version et de source à partir desquelles le contenu est publié. Il s’agit du parent à partir desquelles toutes les autres branches du référentiel sont créées.

Les contributeurs interagissent avec Git pour mettre à jour et manipuler des référentiels tant au niveau local qu’au niveau de GitHub :

- localement par l’intermédiaire d’outils tels que GitHub Desktop ;
- via [www.github.com](https://www.github.com), qui intègre Git pour gérer la réconciliation des contributions qui retournent vers le référentiel principal.

## GitHub

Tous les workflows commencent et se terminent au niveau de GitHub, où est stocké le référentiel principal de tout projet de documentation Adobe. Les copies que les contributeurs créent pour leur propre utilisation sont réparties entre plusieurs ordinateurs. Ces copies sont finalement réconciliées dans le référentiel GitHub principal du projet.

### Organisation du répertoire

La branche par défaut/principale d’un projet sert de version actuelle du contenu destiné au projet. Le contenu dans la branche principale (et des embranchements créés à partir de cette dernière) s’aligne sur l’organisation des rubriques de l’article. Les sous-répertoires servent à organiser le contenu et les actifs d’image.

Vous pouvez généralement trouver un répertoire `help` principal sur la racine du référentiel. Le répertoire d’articles contient un ensemble de sous-répertoires. Les articles dans les sous-répertoires sont formatés sous la forme de fichiers Markdown, qui utilisent une extension *.md*.

Dans la racine de ce répertoire, vous trouvez des articles généraux relatifs au produit ou au service global. En général, vous pouvez ensuite trouver d’autres séries de sous-répertoires qui correspondent aux fonctionnalités/services ou aux scénarios communs.

### Répertoire d’actifs

Les répertoires du guide de l’utilisateur contiennent des sous-répertoires `/assets` pour les fichiers image référencés dans un répertoire.

<!--

### Markdown file template

For convenience, the root directory of each repository typically contains a Markdown template file named `template.md`. You can use this template file as a "starter file" if you need to create a new article for submission to the repository. The file contains:

- A **metadata header** at the top of the file, delineated by two, 3-hyphen lines. It contains the various tags used for tracking information related to the article. It also includes SEO optimizations and reporting processes that Adobe uses to evaluate the performance of the content. So the metadata is important!
- Various **examples of using Markdown** to format the elements of an article.
- General **instructions on the use of Markdown extensions**, which you can use for various types of alerts.
- Examples of **embedding video** by using an iframe.
- General **instructions on the use of docs.adobe.com extensions**, which you can use for special controls such as buttons and selectors.

-->

## Requêtes de tirage

Une *requête de tirage* permet à un contributeur de proposer facilement un ensemble de modifications à appliquer à la branche par défaut. Les modifications (également appelées *validations*) sont stockées dans la branche d’un contributeur, de sorte que GitHub puisse tout d’abord modéliser l’impact de leur *fusion* dans la branche par défaut. Une requête de tirage sert également de mécanisme permettent au contributeur de recevoir des commentaires d’un processus de création/validation, le réviseur de requête de tirage, afin de résoudre les problèmes ou questions potentiels avant que les modifications ne soient fusionnées dans la branche par défaut.

Il existe deux manières de contribuer à l’aide d’une requête de tirage, selon la taille des modifications que vous souhaitez proposer. Nous aborderons ce point en détail ultérieurement, dans la section [GitHub workflow](local-repo.md) de ce guide.
