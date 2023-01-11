---
lastModified: 2018-06-28T00:00:00Z
title: Consignes de style de création pour les contributeurs et contributrices externes
description: Découvrez les consignes de création et de rédaction destinées aux contributeurs et contributrices externes d’Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: ht
source-wordcount: '2227'
ht-degree: 100%

---

# Consignes de style de création pour les contributeurs et contributrices externes {#guidelines}

Cette page fournit des consignes éditoriales aux auteurs et autrices externes qui créent ou mettent à jour du contenu existant sur Experience League. Avant de commencer, assurez-vous :

* D’être familiarisé(e) avec la création [Markdown](markdown.md)
* Vérifiez l’orthographe et la grammaire dans vos articles.
* D’utiliser un ton convivial, une présentation cohérente et des phrases simples pour améliorer la traduction automatique
* De suivre les [bonnes pratiques](#writing-tips) et les normes éditoriales de cette page.

## Consignes de style {#style-guidelines}

Gardez ce qui suit à l’esprit lorsque vous rédigez la documentation.

* **Écrivez de manière concise** : ne gaspillez pas de mots. Gardez les phrases courtes et concises. Restez concentré sur votre article. Utilisez un nombre minimum de notes.
* **Concentrez-vous sur le public et l’objectif** : avant de commencer à écrire, déterminez clairement la personnalité du client et la tâche qu’il essaie de réaliser. Rédigez votre article pour aider le client à mener à bien cette tâche.
* **Utilisez des exemples** : donnez des exemples permettant d’expliquer les concepts.
* **Organisez votre contenu** : créez des sections pour diviser les instructions en groupes d’étapes plus faciles à gérer. Utilisez une capture d’écran lorsqu’elle permet d’y voir plus clair.

## Bonnes pratiques d’écriture technique {#writing-tips}

L’écriture technique, notamment pour la documentation logicielle, constitue un domaine spécialisé. Même le romancier ou la romancière le ou la plus prolifique peut avoir des soucis avec l’écriture technique ; non pas parce que le matériel est complexe ou technique, mais parce qu’il est difficile de _simplifier_ des informations techniques complexes. Pour y parvenir, votre contenu doit être structurellement cohérent, analysable, réutilisable et passer par le pipeline de publication sans erreurs de structure et de syntaxe.

Les sections suivantes décrivent les problèmes courants auxquels les nouveaux auteurs et autrices doivent faire attention :

### En-têtes non séparés par du texte (en-têtes doubles) {#double-headings}

Si deux en-têtes ne sont pas séparés par du texte, ajoutez le texte manquant (pour introduire le deuxième en-tête du sujet). Vous pouvez également supprimer l’un des en-têtes. Le deuxième est probablement inutile.

Par exemple, _Présentation_ n’a aucune utilité ici :

![En-têtes doubles](assets/headings-double.png)

* En outre, si votre deuxième en-tête est _Présentation_, il est probablement inutile. Votre H1 et votre premier paragraphe servent de présentation conceptuelle du sujet de l’article.

* De même, à des fins d’optimisation du moteur de recherche (SEO), les en-têtes autonomes comme _Présentation_ et _Introduction_ ne sont pas utiles en soi. Nommez le produit ou la fonction que vous présentez. (Exemple : _Présentation des rapports sur les abandons_.)

### En-têtes de renvois incohérents {#maps}

Utilisez les en-têtes _Informations supplémentaires_ pour les listes de renvois (ou mappages). Exemple :

![Liste de renvois](assets/headings-more-info.png)

**Instructions pour les listes de renvois**

* Utilisez une liste à puces pour les renvois.
* Utilisez l’italique pour les noms officiels des guides ou des noms de page (lorsque vous n’utilisez pas de texte de lien).
* Ne ponctuez pas l’en-tête (ou tout autre en-tête).
* Évitez les nombres dans les en-têtes.

### Correspondance incorrecte entre l’entrée de table des matières, le chemin de navigation et le nom de page {#toc}

Comme nous gérons manuellement le fichier de table des matières, ces incohérences sont des erreurs courantes. Assurez-vous que votre entrée de la table des matières correspond à votre nom de page (H1). Assurez-vous également qu’il correspond étroitement au chemin de navigation.

**Conseils sur les tables des matières et les listes**

* Vous devrez peut-être raccourcir votre entrée de la table des matières, mais elle doit clairement se rapporter au nom et au chemin de navigation de la page.
* Les chemins de navigation sont extraits des métadonnées du titre, de sorte qu’ils peuvent différer (à des fins d’optimisation pour les moteurs de recherche).

### Guillemets au lieu de l’italique {#quotes}

Il est difficile de résister à l’envie d’ajouter des guillemets autour d’un mot ou d’une phrase. Cependant, les guillemets sont destinés à citer des propos et ne sont presque jamais utilisés dans la documentation de produit.

**Conseils sur les guillemets**

* En règle générale, l’italique fonctionne mieux que les guillemets (pour les messages d’erreur, les mots uniques ou étrangers, etc.).
* Pour les éléments d’interface, utilisez les caractères gras et UICONTROL.

### Procédures {#steps}

L’écriture d’une procédure (le type de contenu de la _tâche_) n’est pas un talent avec lequel nous venons au monde. L’élaboration d’une procédure lisible et claire demande de la pratique.

**Conseils pour les étapes**

* Une procédure est une série d’étapes. Une étape est une commande brève, numérotée, composée _d’une seule phrase_.
* Commencez chaque étape par un verbe ou la préposition _Pour_ (pour orienter le lecteur vers l’objectif, comme dans _Pour rester connecté(e), activez **Rester connecté**_). Si une étape a un objectif spécifique dans la procédure globale, mentionnez l’objectif avant l’action.
* Si vous disposez d’informations sur l’étape (un type de contenu appelé _informations sur l’étape_), ajoutez-les après l’étape (avec la même mise en retrait que l’étape) ou après la ressource (une capture d’écran, une vidéo ou une liste de descriptions d’interface).
* Si votre étape comporte deux actions (par exemple, _Sélectionnez-ceci, puis cela_), écrivez-la comme une seule phrase brève.
* Limitez votre tâche à environ sept à dix étapes. Si vous créez plus de dix étapes dans une tâche, vous devrez probablement la diviser en deux tâches. Utilisez votre bon sens.
* Dans la documentation du produit, n’utilisez pas de titres comme étapes. (Exception ci-dessous pour les tutoriels.)
* Pour les tutoriels de plusieurs pages, les titres peuvent être utilisés en tant qu’étapes. Toutefois, ne les numérotez pas. Écrivez plutôt _Étape 1 :_, _Étape 2 :_, et ainsi de suite.

**Exemple de procédure**

Voici une procédure bien structurée pour se connecter à Adobe :

Pour vous connecter à Adobe :

1. Sur `Adobe.com`, sélectionnez **Experience Cloud**.
1. Sélectionnez **Connexion**.
1. Sélectionnez **Compte personnel**.
1. Pour rester connecté(e), sélectionnez **Rester connecté**.
1. Saisissez votre nom d’utilisateur et votre mot de passe.
1. Sélectionnez **Connexion**.

### Listes parallèles {#lists}

L’utilisation d’une construction parallèle pour les listes facilite la lecture et l’analyse. Les listes comprennent une table des matières, des listes à puces (non triées) ou des listes numérotées.

Exemple de table des matières avec entrées parallèles :

![Table des matières parallèle](assets/parallel-toc.png)

La table des matières précédente est un bon exemple, car :

* Les entrées parentes conceptuelles sont des noms ou des groupes nominaux.
* Les procédures (tâches) sont des verbes à la forme active (et non des gérondifs).
* Toutes les entrées utilisent la majuscule en début de phrase.

## Métadonnées de titre et de description {#metadata}

Les métadonnées de _titre_ et de _description_ sont importantes pour l’optimisation pour les moteurs de recherche, la découverte de contenu et les scores de qualité du contenu sur Experience League.

Voici des exemples de titres et de descriptions :

**Descriptions des articles de concept**

* _Découvrez les segments dans Adobe Analytics. Obtenez de l’aide sur la configuration du panneau Segmentation dans un espace de travail._
* _Obtenez de l’aide sur l’utilisation de segments dans un rapport Pages vues dans Adobe Analytics._

**Descriptions des articles de procédure/tâche**

* _Découvrez comment créer un segment dans Adobe Analytics._
* _Créez un segment dans Adobe Analytics. Découvrez comment sélectionner, configurer et exécuter un rapport en fonction du segment que vous créez._

Celui que vous utilisez dépend de la taille et de la portée de l’article.

**Titre d’un article de concept**

* _Segments dans les rapports Pages vues_

**Titre d’un article de procédure/tâche**

* _Créer un segment pour un rapport Pages vues_

(N’oubliez pas que la barre verticale et le nom du produit sont automatiquement ajoutés aux titres.)

## Méthodes pour améliorer la clarté (et les scores Acrolinx) {#tips}

Voici quelques moyens simples d’améliorer la conception, la clarté et la lisibilité du contenu. Cela contribue également à améliorer les scores de style Acrolinx et les scores CQI sur ExL.

| Instructions | À propos |
|---|---|
| Utilisez la voix active. | Remplacez la voix passive par la voix active. |
| Utilisez le présent. | **Faible :** *Campaign v8 sortira en juin.* <p>**Fort :** *Campaign v8 sort en juin.*<p>Le présent est toujours plus facile à lire pour les client(e)s. |
| Évitez les adverbes faibles et inutiles. | *Très*, *extrêmement*, *incroyablement*... <p>Les adverbes sont des mots supplémentaires qui n’apportent rien d’important au sens si vous utilisez des verbes, des propositions et des adjectifs forts et précis. |
| Utilisez des verbes forts pour les titres et les [entrées de table des matières](#using-toc). | Exemples :<p>**Faible :** *Création et gestion des caractéristiques*. <p>**Fort :** *Créer et gérer les caractéristiques*. |
| Utilisez la [majuscule](https://docs.microsoft.com/fr-fr/style-guide/capitalization) en début de phrase. | En cas de doute, n’utilisez pas les majuscules. Dans les en-têtes, mettez une majuscule en début de phrase. Mettez une majuscule aux noms propres et au premier mot après deux-points (en anglais). Dans les procédures, conservez les majuscules que vous voyez dans l’interface. |
| Découvrez ces petits conseils pour plus de clarté : | <ul><li>Évitez *Afin de* (cela n’ajoute aucun sens). Tout ce dont vous avez besoin est *pour.*</li><li>Évitez *Se servir de.* Cela peut sembler plus technique, mais ce n’est pas le cas. *Se servir de* signifie *utiliser à bon escient, en particulier quelque chose qui n’était pas prévu dans un but précis mais qui servira*.</li><li>Évitez les points-virgules : utilisez plutôt un point et commencez une nouvelle phrase. Les points-virgules introduisent une complexité inutile.</li><li>Deux-points : utilisez les deux-points pour présenter une liste. Utilisez les deux-points avec parcimonie dans les phrases. Mettez une majuscule au premier mot après deux points dans une phrase (en anglais).</li><li>Utilisez la virgule d’Oxford (trois virgules dans une liste) (en anglais).</li><li>Conservez une longueur de phrase en dessous de 39 mots.</li><li>Navigation : utilisez _aller à_ ou _accéder à_.</li><li>Évitez le texte brut de l’URL (utilisez du texte de lien convivial), sauf si l’affichage du chemin est une information importante.</li></ul> |
| Utiliser un correcteur orthographique dans VSC | Installez la vérification orthographique du code (extension) dans Visual Studio Code. |
| Remplacez _cliquer sur_ par _accéder à_ ou _sélectionner_. | _Cliquez sur_ est un mot spécifique à l’appareil (avec des problèmes d’accessibilité). Il est recommandé de s’en éloigner. Voici quelques suggestions pour le modifier :<ul><li>Navigation : _Accédez à Fichier > Imprimer_.</li><li>Cliquez sur : _Sélectionnez Fichier > Imprimer_ ou _Sélectionnez OK_. </li></ul>Consultez la [description des interactions avec l’interface utilisateur](https://docs.microsoft.com/fr-fr/style-guide/procedures-instructions/describing-interactions-with-ui) pour découvrir le meilleur choix de mots dans diverses situations. |
| Exécuter Acrolinx dans VSC | Acrolinx recherche les problèmes de style et de grammaire. Il vérifie les URL, la terminologie, l’orthographe, etc. Cela vous permet d’améliorer la clarté et la traduction du contenu Experience League. |

{style=&quot;table-layout:auto&quot;}

Bonnes pratiques et ressources supplémentaires :

* [Contenu analysable](https://docs.microsoft.com/fr-fr/style-guide/scannable-content/) : aidez les lecteurs et lectrices à trouver rapidement ce dont ils ont besoin ou à se rendre compte rapidement qu’ils sont pas là où ils devraient être. Écrire de manière à faciliter l’analyse peut être utile.
* **Nombres :** dans le corps de texte, écrivez les nombres entiers de zéro à neuf, et utilisez les chiffres pour 10 et les nombres supérieurs. Consultez [Nombres](https://docs.microsoft.com/fr-fr/style-guide/numbers).
* Écrivez comme vous parlez, projetez de la convivialité, et allez au but rapidement.

Pour plus d’informations, consultez les [10 meilleurs conseils d’écriture](https://docs.microsoft.com/fr-fr/style-guide/top-10-tips-style-voice) dans le [Guide de style Microsoft®](https://docs.microsoft.com/fr-fr/style-guide/welcome/).

## Texte secondaire {#alt-text}

Ajoutez du texte secondaire significatif à vos ressources (images). Prenez en compte le texte secondaire qui correspond :

* À l’objectif que les client(e)s peuvent atteindre (nom de la tâche ou du concept).
* À la fonction ou la page que vous montrez.
* Au nom de l’icône que vous montrez.

Google prend en compte le texte secondaire dans les résultats de l’optimisation du moteur de recherche (SEO).

## Localisation - DNL et UICONTROL {#localization}

Vous n’avez pas à vous soucier de savoir si votre produit est localisé ou des langues utilisées par ExL. Cependant, vous contribuez à améliorer la qualité de la localisation en appliquant les deux balises Markdown suivantes (requises) le cas échéant :

* `DNL`

   DNL signifie _ne pas localiser_ (do not localize). Vous l’utilisez uniquement pour les noms de produits Adobes de marques déposées, qui doivent tous rester en anglais.

   Exemples de syntaxe : `[!DNL Adobe Campaign]` ou `[!DNL Workfront]`.

   La balise DNL ne concerne pas les noms de fichier ou les URL.

* `UICONTROL`

   UICONTROL indique une commande d’interface (par exemple, une option, un champ, un onglet, une page, un groupe d’options ou un nom de fonction sur l’interface utilisateur).

   Exemple de syntaxe : `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`.

>[!IMPORTANT]
>
>Vous devez appliquer ces balises avant de localiser votre contenu.

### Utiliser Adobe dans les noms de produits {#product-names}

Pour l’identité d’entreprise, nous incluons généralement _Adobe_ dans la première référence d’un produit au niveau du guide. Pour des raisons d’espace, vous pouvez ne pas mettre Adobe dans un en-tête, mais la première référence dans la copie du corps devra inclure le nom complet. Pour certains produits, tels que _Adobe Audition_ et _Adobe Premiere Pro_, il faut utiliser Adobe comme première référence ou comme référence la plus importante dans chaque élément, car il fait partie du nom légal de la marque.

## Premiers paragraphes {#firstparas}

Votre premier paragraphe doit définir le sujet et décrire ce que le lecteur ou la lectrice apprend en lisant l’article.

Exemple de premier paragraphe (concept) :

_Les audiences sont des collections de visiteurs et visiteuses (une liste d’identifiants visiteur). Les services d’audience d’Adobe gèrent la conversion des données du visiteur en segmentation d’audience. Ainsi, la création et la gestion des audiences sont similaires à la création et à l’utilisation de segments, avec la possibilité de partager les segments d’audience dans Experience Cloud._

Exemple de premier paragraphe (tâche) :

_Créez une source d’attributs du ou de la client(e) (fichiers CSV et FIN) et téléchargez les données. Vous pouvez activer la source de données lorsque vous êtes prêt. Une fois que la source de données est active, partagez les données d’attributs avec Analytics et Target._

### Conseils d’optimisation du moteur de recherche (SEO) pour les premiers paragraphes {#seo}

* Incluez des termes de recherche dans les premiers paragraphes.
* Employez des termes utilisés par les lecteurs et lectrices.
* Incluez des synonymes et, si nécessaire, les versions antérieures des termes. Par exemple, « Le service Experience Cloud ID (ECID), précédemment connu sous le nom d’_identifiant visiteur_ ou sous forme d’acronymes comme MID, MCVID, fournit un identifiant universel et permanent qui identifie les visiteurs et visiteuses. »
* Incluez les termes d’optimisation du moteur de recherche (SEO) dans les liens.
* Évitez de placer des termes essentiels dans des tableaux complexes. Les tableaux complexes ne génèrent pas de résultats de recherche fiables. Le texte dans les images ne fait pas l’objet de recherches. Les légendes font l’objet de recherches.

## Majuscules {#capitalization}

* Le style d’Adobe est d’utiliser la majuscule en début de phrase pour tous les titres, en-têtes, sous-titres et éléments de navigation de page.
* Tous les mots sont en minuscules, à l’exception du premier mot et des noms propres, tels que les noms de marques, de solutions et de services.
* Conservez les majuscules dans les noms de produits des outils, options, éléments de menu, boîtes de dialogue et champs.

## Table des matières {#using-toc}

`TOC.md` est votre table des matières. Chaque guide doit en avoir une.

**Instructions éditoriales pour une table des matières**

* Majuscules : utilisez toujours les règles de majuscules de phrase pour chaque entrée (sauf pour les acronymes). Mettez uniquement en majuscules les noms de produits ou les éléments d’interface officiels (pages, onglets, champs, options, etc.). Conservez les majuscules des termes de l’interface utilisateur lorsque vous y faites référence.
* Forme de verbe et parallélisme : utilisez l’impératif et évitez le participe présent (gérondif). Les tables des matières sont des listes. Faites donc en sorte qu’elles soient parallèles le plus souvent possible. Il existe des exceptions qu’il est parfois impossible d’éviter. Pour les pages conceptuelles, utilisez des noms et des groupes nominaux. Pour les tâches, utilisez des verbes.

**Instructions de syntaxe**

* Un en-tête de section (parent) dans la table des matières ne peut pas être un lien ; il ne comporte pas de page avec du contenu. Il doit contenir une ancre de lien telle que `{#processing-rules}`.
* Vous devez utiliser la syntaxe appropriée pour les en-têtes de section de table des matières (par exemple, `+ Processing rules {#processing-rules}`) et des liens d’article de la table des matières (par exemple, `+ [Article name](article.md)`).
* Les entrées d’article de la table des matières peuvent être une version abrégée du titre de l’article. Respectez les normes de rédaction des présentations, des concepts et des tâches dans ce document.
* Évitez d’ajouter le même fichier plusieurs fois à une table des matières (ou à plusieurs tables des matières). Cela provoque un comportement irrégulier.
* Si votre référentiel contient plusieurs guides d’utilisation, les répertoires de vos guides d’utilisation doivent se trouver au même niveau, tels que les sous-répertoires dans le répertoire `help`. Chaque répertoire du guide d’utilisation doit comporter un fichier de table des matières. N’imbriquez pas les guides d’utilisation.

## Gras et italique {#bold}

* Utilisez du texte en gras uniquement pour les éléments d’interface que vous sélectionnez dans une procédure (et avec UICONTROL).
* Utilisez l’italique pour mettre l’accent sur un mot ou si le mot prête à confusion sans l’italique. Par exemple, un mot étranger, ou lorsque vous décrivez un mot ou définissez un terme.
