---
lastModified: '2018-06-28'
title: Utilisation de liens dans la documentation
seo-title: Utilisation de liens dans la documentation Adobe Git/Markdown
description: Cet article fournit des conseils sur la création de liens vers les contenus et les images.
seo-description: Cet article fournit des conseils sur la création de liens vers les contensu et les images pour la documentation Adobe.
translation-type: ht
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---


# Utilisation de liens dans la documentation

Cet article décrit l’utilisation d’hyperliens dans les pages de documentation. Les liens sont faciles à ajouter dans Markdown avec quelques conventions variables. Les liens orientent les utilisateurs vers le contenu d’une même page, désignent d’autres pages adjacentes ou des sites et des URL externes.

> [!IMPORTANT]
> Tous les liens doivent être sécurisés (`https` plutôt que `http`) chaque fois que l’objectif le permet (comme dans le cas de la grande majorité des liens).

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

<!--
## Bob's link test

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> File Type </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>A comma-separated values file (such as one created in Excel). This is the file that contains the customer attribute data. See [Link TEST](/help/setup/full-workflow.md) </p> <p> <b>Naming requirements:</b> Ensure that file name extensions do not contain white spaces. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Required) The <span class="filepath"> .fin </span> file tells the system that you are finished uploading data. The name of the <span class="filepath"> .fin </span> file must match the name of the <span class="filepath"> .csv </span> file. </p> <p>Adobe recommends creating an empty text file with a <span class="filepath"> .fin </span> extension. An empty file saves space and upload time. </p> <p> <p>Note:  Renaming a <span class="filepath"> .fin </span> file is not allowed after it is uploaded. The <span class="filepath"> .fin </span> file must be uploaded separately and cannot be a renamed, previously uploaded file. </p> </p> <p>After you upload the <span class="filepath"> .fin </span> file in the customer attributes FTP, the system retrieves data quickly (within one minute). This differs from other Adobe FTP-based systems, which pick up data less frequently (around once per hour). </p> <p>The <span class="filepath"> .fin </span> file is not required when using the drag-and-drop upload method. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz </span> or <span class="filepath"> .zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz </span> (gzip) or <span class="filepath"> .zip </span> - for compressed files. A <span class="filepath"> .zip </span> file cannot contain more than one file in the archive. </p> <p> <b>Naming requirements:</b> The name of the <span class="filepath"> .zip </span> or <span class="filepath"> .gz </span> should match the name of the <span class="filepath"> .csv </span>. For example, if your <span class="filepath"> .csv </span> file is <span class="filepath"> crm_small.csv </span>, the <span class="filepath"> .zip </span> file should be <span class="filepath"> crm_small.csv.zip </span>. </p> <p>The .fin file must match the .csv. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
