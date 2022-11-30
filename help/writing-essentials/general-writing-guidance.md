---
lastModified: 2018-06-28T00:00:00Z
title: Consignes de style de création pour les contributeurs externes
description: Découvrez les directives de création et de rédaction destinées aux contributeurs externes à Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2227'
ht-degree: 8%

---

# Consignes de style de création pour les contributeurs externes{#guidelines}

Cette page fournit des directives éditoriales aux auteurs externes qui créent du contenu ou mettent à jour du contenu existant sur Experience League. Avant de commencer, assurez-vous que vous :

* Familiarisez-vous avec [Markdown](markdown.md) création
* Vérifiez l’orthographe et la grammaire dans vos articles
* Utiliser un ton convivial, une présentation cohérente et des phrases simples pour améliorer la traduction automatique
* Suivez [bonnes pratiques](#writing-tips) et les normes éditoriales de cette page

## Consignes de style{#style-guidelines}

Gardez ce qui suit à l’esprit lorsque vous rédigez la documentation.

* **Écrivez de manière concise** : ne gaspillez pas de mots. Gardez les phrases courtes et concises. Restez concentré sur votre article. Utilisez un nombre minimum de notes.
* **Concentrez-vous sur le public et l’objectif** : avant de commencer à écrire, déterminez clairement la personnalité du client et la tâche qu’il essaie de réaliser. Rédigez votre article pour aider le client à mener à bien cette tâche.
* **Utilisez des exemples** : donnez des exemples permettant d’expliquer les concepts.
* **Organisez votre contenu** : créez des sections pour diviser les instructions en groupes d’étapes plus faciles à gérer. Utilisez une capture d’écran lorsqu’elle permet d’y voir plus clair.

## Bonnes pratiques d’écriture technique{#writing-tips}

L&#39;écriture technique, notamment pour la documentation logicielle, est une activité spécialisée. Même le romancier le plus prolifique se met à l&#39;aise en essayant d&#39;écrire technique, non pas parce que le matériel est complexe ou technique, mais parce que ce n&#39;est pas facile de faire des informations techniques complexes. _simple_. Pour réussir, votre contenu doit être structurellement cohérent, scannable, réutilisable et transiter par le pipeline de publication sans erreurs de structure et de syntaxe.

Les sections suivantes décrivent les problèmes courants auxquels les nouveaux auteurs doivent faire attention :

### Titres non séparés par du texte (en-têtes doubles){#double-headings}

Si deux en-têtes ne sont pas séparés par du texte, ajoutez le texte manquant (pour introduire le second en-tête de rubrique). Vous pouvez également supprimer l’un des en-têtes. La seconde est probablement inutile.

Par exemple : _Présentation_ n’a aucun but ici :

![En-têtes doubles](assets/headings-double.png)

* En outre, si votre deuxième en-tête se trouve être _Présentation_, c&#39;est probablement inutile. Votre H1 et votre premier paragraphe servent de présentation conceptuelle du sujet de l’article.

* De même, à des fins d’optimisation pour les moteurs de recherche, les en-têtes autonomes comme _Présentation_ et _Introduction_ ne sont pas utiles par elles-mêmes. Nommez le produit ou la fonction que vous introduisez. (Exemple : _Présentation des rapports sur les abandons_)

### En-têtes de références croisées incohérents{#maps}

Utilisation _Informations supplémentaires_ en-têtes pour les listes de références croisées (ou mappages). Exemple :

![Liste de références croisées](assets/headings-more-info.png)

**Conseils pour les listes de références croisées**

* Utilisation d’une liste à puces pour les références croisées
* Utiliser des italiques pour les noms officiels des guides ou des noms de page (lorsque vous n’utilisez pas de texte de lien)
* Ne pas ponctuer l’en-tête (ou tout autre en-tête)
* Éviter les nombres dans les en-têtes

### Correspondance incorrecte entre l’entrée de table des matières, le chemin de navigation et le nom de page{#toc}

Comme nous gérons manuellement le fichier de table des matières, ces incohérences sont des erreurs faciles. Assurez-vous que votre entrée de la table des matières correspond à votre nom de page (H1). Assurez-vous également qu’il correspond étroitement au chemin de navigation.

**Conseils sur les tables des matières et les listes**

* Vous devrez peut-être raccourcir votre entrée de la table des matières, mais elle doit clairement se rapporter au nom et au chemin de navigation de la page.
* Les chemins de navigation sont extraits des métadonnées du titre, de sorte qu’ils peuvent différer (à des fins d’optimisation pour les moteurs de recherche).

### Guillemets au lieu de guillemets en italique{#quotes}

Il est difficile de résister à l&#39;ajout de citations autour d&#39;un mot ou d&#39;une expression. Cependant, les guillemets sont destinés à citer des propos et ne sont presque jamais utilisés dans la documentation du produit.

**Conseils sur les guillemets**

* En règle générale, l’italique fonctionne mieux que les guillemets (pour les messages d’erreur, les mots uniques ou étrangers, etc.).
* Pour les éléments d’interface, utilisez les caractères gras et UICONTROL.

### Procédures{#steps}

Ecriture d&#39;une procédure (le _tâche_ type de contenu) n’est pas un talent avec lequel nous sommes nés. La création d’une procédure lisible et claire est pratique.

**Conseils pour les étapes**

* Une procédure est une série d’étapes. Une étape est courte, numérotée, _phrase simple_ .
* Commencez chaque étape par un verbe ou la fonction _À_ infinitif (pour orienter le lecteur vers l’objectif, comme dans _Pour rester connecté, activez **Rester connecté**_). Si une étape a un objectif spécifique dans la procédure globale, mentionnez l’objectif avant l’action.
* Si vous disposez d’informations sur l’étape (un type de contenu appelé _informations sur l’étape_, ajoutez-la après l’étape (mise en retrait avec l’étape) ou après la ressource (une capture d’écran, une vidéo ou une liste de descriptions d’interface).
* Si votre étape comporte deux actions (par exemple : _Sélectionnez-le, puis_), écrivez-le comme une seule et brève phrase.
* Limitez votre tâche à environ sept à dix étapes. Si vous créez plus de dix étapes dans une tâche, vous devrez probablement la diviser en deux tâches. Utilisez votre meilleur jugement ici.
* Dans la documentation du produit, n’utilisez pas d’en-têtes comme étapes. (Exception ci-dessous pour les tutoriels.)
* Pour les tutoriels de plusieurs pages, les en-têtes peuvent être autorisés en tant qu’étapes. Toutefois, ne les numérotez pas. Écraser plutôt _Étape 1 :_, _Étape 2 :_, etc.

**Exemple de procédure**

Voici une procédure bien structurée de connexion à Adobe :

Pour vous connecter à Adobe :

1. Activé `Adobe.com`, sélectionnez **Experience Cloud**.
1. Sélectionner **Connexion**.
1. Sélectionner **Compte personnel**.
1. Pour rester connecté, sélectionnez **Rester connecté**.
1. Saisissez votre nom et votre mot de passe.
1. Sélectionner **Connexion**.

### Listes parallèles{#lists}

L’utilisation d’une construction parallèle pour les listes facilite la lecture et la numérisation. Les listes comprennent une table des matières (table des matières), des listes à puces (non triées) ou des listes numérotées.

Exemple de table des matières avec entrées parallèles :

![Table des matières parallèle](assets/parallel-toc.png)

La table des matières précédente est un bon exemple car :

* Les entrées parents conceptuelles sont des noms ou des expressions de nom
* Les procédures (tâches) sont des verbes principaux (et non des gerons)
* Toutes les entrées utilisent la majuscule de la phrase

## Métadonnées de titre et de description{#metadata}

_Titre_ et _description_ les métadonnées sont importantes pour l’optimisation pour les moteurs de recherche, la découverte de contenu et les scores de qualité du contenu sur Experience League.

Voici des exemples de titres et de descriptions :

**Descriptions des articles de concept**

* _Découvrez les segments dans Adobe Analytics. Obtenez de l’aide sur la configuration du panneau Segmentation dans un espace de travail._
* _Obtenez de l’aide sur l’utilisation de segments dans un rapport Pages vues dans Adobe Analytics._

**Descriptions des articles de procédure/tâche**

* _Découvrez comment créer un segment dans Adobe Analytics._
* _Créez un segment dans Adobe Analytics. Découvrez comment sélectionner, configurer et exécuter un rapport en fonction du segment que vous créez._

Celui que vous utilisez dépend de la taille et de la portée de l’article.

**Titre d’un article de concept**

* _Segments dans les rapports Pages vues_

**Titre d’un article de procédure/tâche**

* _Création d’un segment pour un rapport Pages vues_

(N’oubliez pas que la barre verticale et le nom du produit sont automatiquement ajoutés aux titres.)

## Méthodes pour améliorer la clarté (et scores Acrolinx){#tips}

Voici quelques moyens simples d’améliorer la conception, la clarté et la lisibilité du contenu. Cela contribue également à améliorer les scores de style Acrolinx et les scores CQI sur ExL.

| Guide | À propos d’ |
|---|---|
| Utiliser la principale voix | Changer la voix passive à la principale voix |
| Utiliser la tension actuelle | **Faible :** *Campaign v8 sortira en juin.* <p>**Strong :** *Versions de Campaign v8 en juin.*<p>Présenter la tension est toujours plus facile à lire pour les clients. |
| Évitez les pubs faibles et inutiles. | *Très*, *extrêmement*, *incroyablement*.... <p>Les publicités sont des mots supplémentaires qui n’ajoutent pas de signification significative si vous utilisez des verbes, des clauses et des adjectifs forts et précis. |
| Utilisez des verbes forts pour les titres et [Entrées de table des matières](#using-toc) | Exemples :<p>**Faible :** *Création et gestion des caractéristiques* <p>**Strong :** *Création et gestion des caractéristiques* |
| Utilisation de la phrase [capitalisation](https://docs.microsoft.com/en-us/style-guide/capitalization) | En cas de doute, ne capitalisez pas. Dans les titres, utilisez une majuscule de type phrase. Capitalisez les noms appropriés et le premier mot après deux points. Dans les procédures, faites correspondre la mise en majuscules que vous voyez dans l’interface. |
| Découvrez ces petits conseils pour plus de clarté | <ul><li>Éviter *Pour* (cela n&#39;ajoute aucun sens). Tout ce dont vous avez besoin *à .*</li><li>Éviter *Utilisez .* Cela peut sembler plus technique, mais ce n&#39;est pas le cas. *Utilisation* signifie *d’utiliser à bon escient, en particulier quelque chose qui n’était pas prévu dans un but précis mais qui servira*.</li><li>Évitez les points-virgules : Utilisez plutôt un point et commencez une nouvelle phrase. Les points-virgules introduisent une complexité inutile.</li><li>Deux-points : Utilisez les deux-points pour présenter une liste. Utilisez les deux-points avec parcimonie dans les phrases. Capitalisez le premier mot après deux points dans une phrase.</li><li>Utilisez la virgule d’Oxford (trois virgules dans une liste).</li><li>Gardez la longueur de la phrase en dessous de 39 mots.</li><li>Navigation : use _accéder à_ ou _accéder à_.</li><li>Évitez le texte brut de l’URL (utilisez du texte de lien convivial), sauf si l’affichage du chemin est une information importante.</li></ul> |
| Utilisation d’un correcteur orthographique dans VSC | Installez la vérification orthographique du code (extension) dans Visual Studio Code. |
| Modifier _click_ to _accéder à_ ou _select_ | _Cliquez sur_ est un mot spécifique à l’appareil (avec des problèmes d’accessibilité), et la tendance est de s’en éloigner. Voici quelques suggestions pour le modifier :<ul><li>Navigation : _Accédez à Fichier > Imprimer_.</li><li>Cliquez sur : _Sélectionnez Fichier > Imprimer_ ou _Sélectionnez OK_. </li></ul>Voir [Description des interactions avec l’interface utilisateur](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) pour plus d’idées sur le meilleur choix de mots dans diverses situations. |
| Exécution d’Acrobat dans VSC | Acrolinx recherche les problèmes de style et de grammaire. Il vérifie les URL, la terminologie, l’orthographe, etc. Cela vous permet d’améliorer votre clarté et d’améliorer la traduction du contenu Experience League. |

{style=&quot;table-layout:auto&quot;}

Autres bonnes pratiques et ressources :

* [Contenu numérisable](https://docs.microsoft.com/en-us/style-guide/scannable-content/): Aidez les lecteurs à trouver rapidement ce dont ils ont besoin, ou à reconnaître aussi rapidement lorsqu&#39;ils ne sont pas là où ils doivent être. L’écriture pour faciliter l’analyse peut aider.
* **Nombres :** Dans le texte du corps, écrivez les nombres entiers de zéro à neuf, et utilisez les nombres pour 10 ou plus. Voir [Nombres](https://docs.microsoft.com/en-us/style-guide/numbers).
* Écrivez comme vous parlez, le projet est convivial, et arrivez au but rapidement.

Voir [10 premiers conseils d’écriture](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) dans le [Guide de style Microsoft®](https://docs.microsoft.com/en-us/style-guide/welcome/) pour plus d’informations.

## Texte secondaire{#alt-text}

Ajoutez du texte secondaire significatif à vos ressources (images). Prenez en compte le texte secondaire qui correspond à :

* L’objectif que les clients peuvent atteindre (nom de la tâche ou du concept)
* Fonction ou page affichée
* Nom de l’icône que vous affichez

Google prend en compte le texte secondaire dans les résultats de l’optimisation pour les moteurs de recherche.

## Localisation - DNL et UICONTROL{#localization}

Vous n’avez pas à vous soucier de savoir si votre produit est localisé ou les langues utilisées par ExL. Cependant, vous contribuez à améliorer la qualité de la localisation en appliquant les deux balises Markdown suivantes (requises) le cas échéant :

* `DNL`

   DNL signifie _ne pas localiser_. Vous l’utilisez uniquement pour les noms de produits Adobes faisant l’objet d’une marque, qui doivent tous rester en anglais.

   Exemples de syntaxe : `[!DNL Adobe Campaign]` ou `[!DNL Workfront]`

   DNL n’est pas prévu pour les noms de fichier ou les URL.

* `UICONTROL`

   UICONTROL indique un contrôle d’interface (par exemple, une option, un champ, un onglet, une page, un groupe d’options ou un nom de fonctionnalité dans l’interface utilisateur).

   Exemple de syntaxe : `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Vous devez appliquer ces balises avant de localiser votre contenu.

### Utilisation de l’Adobe dans les noms de produits{#product-names}

Pour l’identité d’entreprise, nous incluons généralement _Adobe_ dans la première référence d’un produit au niveau du guide. Selon les considérations d’espace, vous pouvez déposer l’Adobe dans un en-tête, mais la première référence dans la copie du corps doit inclure le nom complet. Certains produits, tels que _Adobe Audition_ et _Adobe Premiere Pro_, requiert l’utilisation d’un Adobe sur la première ou la plus importante référence dans chaque élément de garantie, car il fait partie du nom légal de la marque.

## Premiers paragraphes{#firstparas}

Votre premier paragraphe doit définir le sujet et décrire ce que le lecteur apprend de la lecture de l’article.

Exemple de premier paragraphe (concept) :

_Les audiences sont des collections de visiteurs (une liste d’identifiants visiteur). Le service d’audience d’Adobe gère la traduction des données du visiteur en segmentation de l’audience. Ainsi, la création et la gestion des audiences sont similaires à la création et à l’utilisation de segments, avec la possibilité de partager les segments d’audience dans Experience Cloud._

Exemple de premier paragraphe (tâche) :

_Création d’une source d’attributs du client (fichiers CSV et FIN) et transfert des données. Vous pouvez activer la source de données lorsque vous êtes prêt. Une fois que la source de données est active, partagez les données d’attributs avec Analytics et Target._

### Conseils d’optimisation pour les moteurs de recherche pour les premiers paragraphes{#seo}

* Incluez des termes de recherche dans les premiers paragraphes.
* Utilisez des termes utilisés par les lecteurs.
* Incluez des synonymes et, si nécessaire, l’utilisation précédente de termes. Par exemple, &quot;Le service d’ID d’Experience Cloud (ECID), précédemment connu sous le nom de _identifiant visiteur_ ou sous forme d’acronymes comme MID, MCVID, fournit un identifiant universel et permanent qui identifie les visiteurs.&quot;
* Incluez les termes d’optimisation pour les moteurs de recherche dans les liens.
* Évitez de placer des termes essentiels dans des tableaux complexes. Les tableaux complexes ne génèrent pas de résultats de recherche fiables. Le texte dans les images n’est pas une recherche. Les sous-titres sont recherchés.

## Capitalisation{#capitalization}

* Le style d’Adobe utilise la mise en majuscules de style phrase pour tous les titres, titres, sous-titres et éléments de navigation de page.
* Tous les mots sont en minuscules, à l’exception du premier mot et des noms propres, tels que les noms des marques, des solutions et des services.
* Correspondance avec la mise en majuscules dans les noms de produits des outils, options, éléments de menu, boîtes de dialogue et champs.

## Table des matières{#using-toc}

Le `TOC.md` est votre table des matières. Chaque guide doit en avoir un.

**Directives éditoriales pour une table des matières**

* Capitalisation : Utilisez toujours la casse pour chaque entrée (sans les acronymes). Capitalisez uniquement les noms de produits ou les éléments d’interface formels (pages, onglets, champs, options, etc.). Correspondance avec l’interface utilisateur lorsque vous y faites référence.
* Forme verbe et parallélisme : Utilisez des verbes impératifs et évitez les germes. Les tables des matières sont des listes. Par conséquent, la plupart du temps, les listes doivent être parallèles. Il y a des exceptions qu&#39;il est parfois impossible d&#39;éviter. Pour les pages conceptuelles, utilisez des noms et des expressions de nom. Pour les tâches, utilisez des verbes.

**Instructions de syntaxe**

* Un en-tête de section (parent) dans la table des matières ne peut pas être un lien ; il ne comporte pas de page avec du contenu. Elle doit contenir une ancre telle que `{#processing-rules}`.
* Vous devez utiliser la syntaxe appropriée pour les en-têtes de section de table des matières (par exemple, `+ Processing rules {#processing-rules}`) et des liens d’article de la table des matières (par exemple, `+ [Article name](article.md)`).
* Les entrées d’article de la table des matières peuvent être une version abrégée du titre de l’article. Respectez les normes de rédaction des présentations, concepts et tâches de ce document.
* Évitez d’ajouter le même fichier plusieurs fois à une table des matières (ou à plusieurs tables des matières). Cela provoque un comportement bizarre.
* Si votre référentiel contient plusieurs guides de l’utilisateur, les répertoires de vos guides de l’utilisateur doivent se trouver au même niveau, tels que les sous-répertoires dans la variable `help` répertoire . Chaque répertoire du guide de l’utilisateur doit comporter un fichier de table des matières. Aucun guide de l’utilisateur d’imbrication.

## Gras et italique{#bold}

* Utilisez du texte en gras uniquement pour les éléments d’interface sur lesquels vous cliquez dans une procédure (et avec UICONTROL).
* Utilisez l’italique pour mettre l’accent ou lorsqu’un mot est déroutant sans lui. Par exemple, un mot étranger, ou lorsque vous décrivez un mot ou définissez un terme.
