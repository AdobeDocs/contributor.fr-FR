---
lastModified: 2018-06-28T00:00:00Z
title: Utilisation de liens dans la documentation
seo-title: Utilisation de liens dans la documentation Adobe Git/Markdown
description: Cet article fournit des conseils sur la création de liens vers les contenus et les images.
seo-description: Cet article fournit des conseils sur la création de liens vers les contensu et les images pour la documentation Adobe.
translation-type: tm+mt
source-git-commit: df6c4152df0c1ee87c9fc4ca22e36a3f13cb620b
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 100%

---


# Utilisation de liens dans la documentation

Cet article décrit l’utilisation d’hyperliens dans les pages de documentation. Les liens sont faciles à ajouter dans Markdown avec quelques conventions variables. Les liens orientent les utilisateurs vers le contenu d’une même page, désignent d’autres pages adjacentes ou des sites et des URL externes.

>[!IMPORTANT]
>Tous les liens doivent être sécurisés (`https` plutôt que `http`) chaque fois que l’objectif le permet (comme dans le cas de la grande majorité des liens).

## Lien vers des URL

Les mots que vous incluez dans le texte du lien doivent être le titre de la page que désigne le lien ou un texte descriptif spécifique.

**Exemples :**

- `For more information, see the [overview article](https://github.com/AdobeDocs/target.en/help/overview.md).`

- `For more details, see [Adobe Legal Concerns](https://www.adobe.com/legal).`

## Lien d’un article vers un autre

Pour créer un lien intégré d’un article vers un autre dans le même référentiel, utilisez la syntaxe de lien suivante :

- Un article dans un répertoire renvoie à un autre article dans le même répertoire :

   `[link text](article-name.md)`

- Un article renvoie à un article dans le répertoire racine à partir d’un sous-répertoire :

   `[link text](../article-name.md)`

- Un article renvoie à un article dans le répertoire racine à partir d’un sous-répertoire secondaire :

   `[link text](../../article-name.md)`

- Un article du répertoire racine renvoie à un article dans un sous-répertoire :

   `[link text](./directory/article-name.md)`

- Un article dans un sous-répertoire renvoie à un article dans un autre sous-répertoire :

   `[link text](../directory/article-name.md)`

- Un article dans un sous-répertoire secondaire renvoie à un article dans un autre sous-répertoire :

   `[link text](../../directory/article-name.md)`

## Lien vers les ancres de lien

Vous ne devez pas créer d’ancres de lien. Elles sont automatiquement générées au moment de la publication pour tous les titres H2. Vous devez simplement créer des liens vers les sections H2 (##).

- Pour créer un lien vers un titre dans le même article :

   `[link](#the-text-of-the-level2-section-separated-by-hyphens)`

   `[Link to anchors](#links-to-anchors)`

- Pour créer un lien vers une ancre de lien dans un autre article du même sous-répertoire :

   `[link text](article-name.md#anchor-name)`

   `[Configure your profile](overview.md#getting-started)`

- Pour créer un lien vers une ancre de lien dans un autre sous-répertoire de service :

   `[link text](../directory/article-name.md#anchor-name)`

   `[Configure your profile](../overview.md#configure-your-profile)`

## Lien vers des images

Les images et les fichiers sont de préférence stockés dans un répertoire `assets` au même niveau que le fichier Markdown qui le désigne.

- Un article renvoie à une image dans le sous-répertoire `assets` :

   `![alt text](assets/image-name.png)`

- Un article renvoie à une image dans le sous-répertoire `assets/no-localize` :

   `![alt text](assets/no-localize/image-name.png)`
