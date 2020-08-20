---
lastModified: 2018-06-28T00:00:00Z
title: Utilisation de Markdown pour la rédaction de documentation
seo-title: Utilisation de Markdown pour la rédaction de documentation Adobe
description: cet article fournit les concepts de base et les informations de référence relatives au langage Markdown utilisé pour la rédaction d’articles.
seo-description: cet article fournit les concepts de base et les informations de référence relatives au langage Markdown utilisé pour la rédaction d’articles relatifs à la documentation Adobe.
translation-type: tm+mt
source-git-commit: 27ba164070996d192c84493d83232484d2badb28
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 100%

---


# Utilisation de Markdown pour la rédaction de documentation technique

Les articles de documentation technique d’Adobe sont rédigés dans un langage de marquage léger appelé [Markdown](https://daringfireball.net/projects/markdown/), qui est à la fois facile à lire et à apprendre.

À mesure que nous stockons le contenu de documents Adobe dans GitHub, il peut utiliser une version de Markdown appelée [GitHub Flavored Markdown (GFM)](https://help.github.com/categories/writing-on-github/), qui offre des fonctionnalités supplémentaires pour les besoins de formatage courants. De plus, Adobe a élargi le champ d’application de Markdown afin de prendre en charge certaines fonctionnalités d’aide, telles que les notes, les conseils et les vidéos intégrées.

## Concepts de base de Markdown

### Titres

Pour créer un titre, utilisez un signe dièse (#) en début de ligne :

```
   # This is level 1 (article title)
   ## This is level 2
   ### This is level 3
   #### This is level 4
   ##### This is level 5
```

### Texte de base

Un paragraphe ne nécessite pas de syntaxe spéciale dans Markdown.

Pour mettre le texte en **gras**, entourez-le de deux astérisques. Pour mettre le texte en *italique*, entourez-le d’astérisques uniques :

```markdown
    This text is **bold**.
    This text is *italic*.
    This text is both ***bold and italic***.
```

<!--
To format superscript (H<sub>2</sub>O) and subscript (e=mc<sup>2</sup>) text:

```markdown
This is subscript H<sub>2</sub>O and superscript e=mc<sup>2</sup>.
```
-->

Pour ignorer les caractères de formatage Markdown, utilisez \ avant le caractère :

```markdown
This is not \*italicized\* type.
```

### Listes numérotées et listes à puces

Pour créer des listes numérotées, commencez une ligne par `1.` ou `1)`, mais n’utilisez pas les deux formats dans la même liste. Il n’est pas nécessaire de spécifier les nombres. GitHub le fait pour vous.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Contenu affiché :

1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.

<!-- markdownlint-disable MD037 -->
Pour créer des listes à puces, commencez une ligne par \* ou - ou +, mais ne mélangez pas les formats dans la même liste. (Ne mélangez pas les formats de puces, tels que \* et \+, dans le même document.)
<!-- markdownlint-disable MD037 -->

```markdown
* First item in an unordered list.
* Another item.
* Here we go again.
```

Contenu affiché :

* First item in an unordered list.
* Another item.
* Here we go again.

Vous pouvez également intégrer des listes dans d’autres listes et ajouter du contenu entre les éléments de la liste.

```markdown
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this: 

   | Hello | World |
   |---|---|
   | How | are you? |  
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.
```

Contenu affiché :

1. Set up your table and code blocks.
1. Perform this step.

   ![écran](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this:

   | Hello | World |
   |---|---|
   | How | are you? |
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.

### Tableaux

Les tableaux ne font pas partie de la spécification Markdown de base, mais Adobe les prend en charge dans une certaine mesure. Markdown ne prend pas en charge les listes à lignes multiples dans les cellules. Il est recommandé d’éviter d’utiliser plusieurs lignes dans les tableaux. Vous pouvez créer des tableaux à l’aide de la barre verticale (|) pour délimiter les colonnes et les lignes. Les traits d’union créent l’en-tête de chaque colonne, tandis que les barres verticales séparent chaque colonne. Insérez une ligne vierge avant votre tableau afin qu’il soit rendu correctement.

```markdown
| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Contenu affiché :

| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |

Les tableaux simples fonctionnent correctement dans Markdown. Toutefois, les tableaux contenant plusieurs paragraphes ou listes dans une cellule sont difficiles à utiliser. Pour ce type de contenu, nous recommandons d’utiliser un autre format, comme des titres et du texte.

Pour plus d’informations sur la création de tableaux, voir :

* [Organisation des informations de GitHub avec des tableaux](https://help.github.com/articles/organizing-information-with-tables/)
* L’application Web [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
* [Convertir les tableaux HTML en Markdown](https://jmalarcon.github.io/markdowntables/)

### Liens

La syntaxe Markdown d’un lien inséré se compose de la partie `[link text]`, qui est le texte qui sera affiché sous forme d’hyperlien, suivie de la partie `(file-name.md)`, qui est l’URL ou le nom de fichier lié à :

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com)
```

Contenu affiché :

[Adobe](https://www.adobe.com)

Pour les liens vers des articles (références croisées) dans le référentiel, utilisez des liens relatifs. Vous pouvez utiliser tous les opérandes de liens relatifs, tels que./ (répertoire actuel), ../ (retour d’un répertoire) et ../../ (retour de deux répertoires).

```markdown
See [Overview example article](../../overview.md)
```

Pour plus d’informations sur les liens, consultez l’article [Liens](linking.md) de ce guide pour en savoir plus sur la syntaxe.

### Images

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Contenu affiché :

![Logo Adobee](assets/no-localize/adobe_standard_logo.png "Texte de l’info-bulle")

### Blocs de code

Markdown prend en charge le placement de blocs inséré dans une phrase et en tant que bloc « clôturé » séparé entre des phrases. Pour plus d’informations, reportez-vous [à l’assistance native de Markdown pour les blocs de code.](https://daringfireball.net/projects/markdown/syntax#precode)

Utilisez des apostrophes ouvrantes ( \` ) pour créer des styles de code intégrés au sein d’un paragraphe. Pour créer un bloc de code spécifique sur plusieurs lignes, ajoutez trois apostrophes ouvrantes (\`\`\`) avant et après le bloc de code (appelé bloc de code « clôturé » dans Markdown et simplement composant « bloc de code » dans AEM). Pour les blocs de code clôturés, ajoutez la langue de code après le premier jeu d’apostrophes ouvrantes afin que Markdown mette correctement en évidence la syntaxe du code. Example : \`\`\`javascript

Exemples :

```markdown
This is `inline code` within a paragraph of text.
```

Contenu affiché :

This is `inline code` within a paragraph of text.

Il s’agit d’un bloc de code clôturé :

```markdown
\```javascript
function test() {
 console.log("notice the blank line before this function?");
\```
```

Contenu affiché :

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

### Listes de définitions

Une liste de définitions est une extension Markdown qui prend en charge le composant Liste de définitions dans AEM. Une liste de définitions se compose d’un terme et de sa définition.

<!--

```markdown
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

Displayed:

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
--->

#### Remarques et commentaires

Les commentaires (remarques) n’apparaissent pas dans les articles d’aide destinés au public. Toutefois, les commentaires apparaissent dans les fichiers Markdown destinés au public que les utilisateurs peuvent consulter et modifier.

## Extensions Markdown personnalisées

Les articles Adobe utilisent Markdown standard pour la plupart des mises en forme d’articles, tels que les paragraphes, les liens, les listes et les en-têtes. Pour une mise en forme plus riche, les articles peuvent utiliser des fonctions Markdown étendues telles que :

* Blocs de notes
* Vidéos intégrées
* Ne pas localiser
* Propriétés du composant, comme l’attribution d’un ID d’en-tête différent à un en-tête

Utilisez le guillemet anglais Markdown (>) au début de chaque ligne pour associer un composant étendu, comme une note. Si vous devez utiliser des sous-composants dans des composants, ajoutez un niveau supplémentaire de guillemets (>  >) pour cette section de sous-composant. Par exemple, une NOTE dans une section DONOTLOCALIZE doit commencer par >    >.

Certains éléments de Markdown courants, tels que les en-têtes et les blocs de code, incluent des propriétés étendues. Si vous devez modifier les propriétés par défaut, ajoutez les paramètres entre crochets français /{ /} après le composant. Les propriétés étendues sont décrites en contexte.

### Blocs de notes

Vous pouvez choisir parmi quatre types de blocs de notes afin d’attirer l’attention sur un contenu spécifique :

* `[!NOTE]`
* `[!CAUTION]`
* `[!TIP]`
* `[!IMPORTANT]`

En général, les blocs de notes doivent être utilisés avec parcimonie, car ils peuvent être perturbateurs. Bien qu’ils prennent également en charge les blocs de code, les images, les listes et les liens, faites en sorte que les blocs de notes restent simples et directs.


```markdown
>[!NOTE]
>
>This is a standard NOTE block.
```

Contenu affiché :

>[!NOTE]
>
>This is a standard NOTE block.

```markdown
>[!TIP]
>
>This is a standard tip.
```

Contenu affiché :

>[!TIP]
>
>This is a standard tip.

### Vidéos

Les vidéos intégrées ne sont pas rendues nativement dans Markdown, mais vous pouvez utiliser cette extension Markdown.

```markdown
>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)
```

Contenu affiché :

>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)

### More Like This

Le composant « More Like This » dans AEM s’affiche à la fin d’un article. Il affiche les liens connexes. Lorsque l’article est rendu, il peut être formaté comme les en-têtes de niveau 2 (# #) sans être ajouté à la mini-table des matières.

```markdown
>[!MORELIKETHIS]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html)
```

Contenu affiché :

>[!MORELIKETHIS]
>* [Article 1](https://helpx.adobe.com/fr/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/fr/support/audience-manager.html)


### DNL - Do Not Localize - et UICONTROL

Dans certains cas, nous devons signaler certaines sections de contenu d’un article comme étant en anglais uniquement.
Les mots, phrases et autres éléments doivent être déclarés dans nos systèmes de traduction et permettent de gérer un lexique contrôlé.

Pour les mots ou expressions qui ne doivent pas être localisés, utilisez l’extension `[!DNL]` pour entourer le mot ou la section.

Pour les éléments de l’interface utilisateur et des menus d’une solution, nous utilisons l’extension ``.

**Exemple :**

In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.

**Source :**

```markdown
In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.
```

**Exemple**

Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.

**Source :**

```markdown
Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.
```

## Pièges et résolution de problèmes

### Texte alternatif

Le texte alternatif qui contient des tirets bas ne sera pas rendu correctement. Par exemple, au lieu d’utiliser :

```markdown
![Settings_Step_2](/assets/settings_step_2.png)
```

Nous conseillons d’utiliser des tirets (-) plutôt que des tirets bas (_) dans les noms de fichier.

```markdown
![Settings-Step-2](/assets/settings-step-2.png)
```

### Apostrophes et guillemets

Si vous copiez du texte dans un éditeur Markdown, il peut contenir des apostrophes ou des guillemets « intelligentes » (courbes). Ils doivent être codés ou remplacés par des apostrophes ou des guillemets de base. Sinon, vous obtenez des caractères bizarres tels que celui-ci lorsque le fichier est publié : Itâ€™s.

Voici les encodages des versions « intelligentes » de ces signes de ponctuation :

* Guillemet gauche (ouvrant) : `&#8220;`
* Guillemet droit (fermant) : `&#8221;`
* Guillemet ou apostrophe simple droit (fermant) : `&#8217;`
* Guillemet ou apostrophe simple gauche (ouvrant) (rarement utilisé) : `&#8216;`

### Chevrons

Si vous utilisez des chevrons dans le texte (et non dans le code) de votre fichier (par exemple, pour désigner un caractère générique), vous devez encoder les chevrons manuellement. Sinon, Markdown pense qu’il s’agit d’une balise HTML.

Par exemple, encodez `<script name>` comme `&lt;script name&gt;`

### Esperluettes dans les titres

Les esperluettes (&amp;) ne sont pas autorisées dans les titres. Utilisez plutôt « et » ou l’encodage `&amp;`.

## Voir également

### Ressources Markdown

* [Présentation de Markdown](https://daringfireball.net/projects/markdown/syntax)
* [Concepts de base de GitHub Markdown](https://help.github.com/articles/markdown-basics/)
