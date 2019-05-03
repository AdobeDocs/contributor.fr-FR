---
title: Guide du contributeur pour la documentation d’Adobe
seo-title: Présentation du guide du contributeur pour la documentation technique d'Adobe
  Experience Cloud
description: Ce guide explique comment apporter votre contribution sous la forme de
  suggestions et d’ajouts sur le site de documentation Adobe.
seo-description: Ce guide explique comment contribuer à la documentation technique
  [!UICONTROL Adobe Experience Cloud].
translation-type: tm+mt
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---


# Présentation du guide du contributeur pour Adobe Documentation

## Documentation de collaboration

Durant 2019, tous les contenus techniques et d'activation d'Adobe Experience Cloud passent à une nouvelle plateforme, reposant sur les principes Open Source, utilisant les solutions Github, Markdown et Adobe Experience Cloud, notamment Adobe Experience Manager, Analytics, Launch et Target.

Ce modèle Open Source améliore la qualité du contenu et la communication entre les clients, les équipes de documentation et les équipes de produits. Sur chaque page, vous pouvez désormais évaluer l'utilité du contenu, les problèmes de consignation et même contribuer à des suggestions de contenu sous la forme de requêtes Extraire (prs). Les équipes de documentation Adobe surveillent quotidiennement les contributions et les problèmes et effectuent des mises à jour, des ajustements et des ajustements, le cas échéant.

## Utilisation de la documentation collaborative

En tant qu'utilisateur de ce matériel, quel que soit le type employé, partenaire, client ou même client potentiel, vous avez le choix de contribuer à cette documentation de plusieurs manières simples ;

* evaluer l'utilité de la page
* enregistrer un problème sur une page spécifique
* même envoyer un quick edits jusqu'à la création d'articles entiers, avec des ressources et des exemples de code

Ce guide décrit tout ce que vous devez savoir pour interagir avec ce jeu de matériaux et y contribuer.

<!--
> [!IMPORTANT]
> All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Apporter des modifications rapides aux documents existants

Apporter des modifications rapides est un bon moyen de corriger de petites erreurs et omissions dans des documents. Si un article affiche un bouton de modification comme illustré ci-dessous, vous pouvez effectuer une correction rapide par vous-même. Lorsque vous modifiez le document, vous envoyez une requête de tirage pour nous soumettre la correction/suggestion, que nous pouvons ensuite refuser, approuver et publier.

1. Signez le [contrat de licence du contributeur (CLA)](http://opensource.adobe.com/cla.html) si vous le souhaitez.

   Il suffit d'envoyer une seule fois un CLA Adobe.
1. Cliquez sur ** dans la colonne de droite pour accéder au fichier source Markdown sur GitHub.`Edit this page`**
1. Cliquez sur l'icône représentant un crayon pour modifier l'article.

   > [!NOTE]
   > Si l’icône en forme de crayon est grisée, vous devez vous connecter à votre compte GitHub ou créer un compte.

   ![Emplacement de l’icône en forme de crayon](assets/edit-icon.png)

1. Apportez vos modifications dans l’éditeur Web. Vous pouvez cliquer sur l’onglet **Preview changes** pour vérifier la mise en forme de votre modification.
1. Une fois que vous avez apporté vos modifications, faites défiler l’écran jusqu’au bas de la page. Saisissez un titre et une description pour votre requête de tirage, puis cliquez sur **Propose file change**, comme le montre la figure suivante :

   ![votre suggestion de modification](assets/submit-pull-request.png)

   >[!NOTE] Si vous recevez un message d'erreur de validation sur la signature d'un contrat de licence de contributeur (CLA), cliquez **sur Détails** pour ouvrir le contrat de licence. Signez l'accord, le cas échéant. Fermez et ouvrez ensuite la demande d'extraction, puis continuez.

C’est aussi simple que cela. Merci ! Les membres de l’équipe de documentation vont examiner et fusionner votre requête de tirage.

## Consigner un problème

Une autre manière simple de nous informer d’un problème lié à un élément de contenu consiste à consigner un problème.

1. Si vous constatez un problème lié à un élément de contenu, cliquez sur le lien `Log an Issue` dans l’angle inférieur droit d’une page. Voir la figure ci-dessous :

   ![](assets/git_log_issue.png)

   > [!NOTE]
   > Vous devez vous connecter à votre compte GitHub ou créer un compte pour consigner un problème.

   En cliquant sur ce lien, vous pouvez consigner un ticket rapide chez nous, à l’aide de l’interface GitHub Issues.

1. L’URL de la page contenant le problème va automatiquement s’afficher le champ de description. Renseignez le titre, rédigez une brève description du problème, puis cliquez sur *Submit new issue*.

   ![](assets/git_issue_example.png)

L'envoi d'un problème avertit directement l'équipe de contenu de cette page qui pourra agir. Une fois le contenu mis à jour, nous vous informerons dans l’interface GitHub Issues. Ensuite, vous serez averti par courrier électronique une fois la mise à jour ou la fermeture effectuée.

## Comprendre les autorisations GitHub

L’interface utilisateur de modification de GitHub s’adapte aux autorisations de votre référentiel. Les images précédentes sont exactes pour les contributeurs qui ne disposent pas d’autorisations d’écriture dans le référentiel cible. GitHub crée automatiquement un double du référentiel cible dans votre compte. Si vous disposez d’un accès en écriture au référentiel cible, GitHub crée une branche dans le référentiel cible.

Adobe utilise des requêtes de tirage pour toutes les modifications, même dans le cas de contributeurs disposant d’un accès en écriture. La plupart des référentiels disposent d’une protection pour la branche `master`, de sorte que les mises à jour doivent être soumises en tant que requêtes de tirage.

L’expérience d’édition intégrée au navigateur est préférable pour les modifications mineures ou occasionnelles. Si vous effectuez des contributions de grande ampleur ou utilisez des fonctionnalités Git avancées, nous vous recommandons de [dupliquer le référentiel et de travailler localement](setup/full-workflow.md).

## Fournir des commentaires

Avec une solution aussi vaste que celle d’Adobe, la documentation est toujours une œuvre inachevée. Si vous détectez des erreurs, consignez un problème, si vous avez des suggestions sur le matériel, partagez-les avec nous. Indiquez les informations que vous recherchez. Dites-nous si vous ne trouvez pas ce dont vous avez besoin ou, si vous avez rencontré des difficultés pour mener à bien votre tâche, faites-nous savoir comment nous pouvons vous aider à assimiler nos solutions.

L’équipe en charge de la documentation collaborative et tous les auteurs et producteurs de contenu d’[!UICONTROL Adobe Experience Cloud] vous adressent leurs remerciements.