---
title: Workflow de contributions GitHub pour les modifications majeures
description: Découvrez comment apporter des contributions à la documentation Adobe sur Experience League.
exl-id: ad467ad4-abd2-4166-8659-e29c48d268ec
source-git-commit: 90122796acee9214ba96360eb7b5ff5c321a4bd6
workflow-type: ht
source-wordcount: '944'
ht-degree: 100%

---

# Workflow de contributions GitHub pour les modifications majeures

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Aperçu

Ce workflow convient à un contributeur qui doit apporter une modification majeure ou qui sera un contributeur fréquent à un référentiel. Les contributeurs fréquents apportent généralement des modifications continues (à long terme) qui passent par plusieurs cycles de création/validation/évaluation ou s’étendent sur plusieurs jours avant l’approbation et la fusion de la requête de tirage.

### Terminologie

Avant de commencer, examinons quelques-uns des termes Git/GitHub utilisés dans ce workflow.

| Nom | Description |
|-----------|-------------|
| double | Normalement utilisé comme nom, en cas de référence à une copie d’un référentiel GitHub principal. En pratique, un double n’est qu’un autre référentiel. Il est toutefois spécial dans le sens où GitHub conserve une connexion bidirectionnelle avec le référentiel principal/parent. Il est parfois utilisé comme verbe, comme dans « Vous devez d’abord dupliquer le référentiel ». |
| élément distant | Une connexion nommée à un référentiel distant, tel qu’un élément distant « origine » ou « en amont ». Git y fait référence comme des éléments distants, car ils servent à référencer un référentiel hébergé sur un autre ordinateur. Dans ce workflow, un élément distant est toujours un référentiel GitHub. |
| origine | Nom attribué à la connexion entre votre référentiel local et le référentiel à partir duquel elle a été clonée. Dans ce workflow, l’origine représente la connexion à votre double. Elle est parfois utilisée comme Moniker pour le référentiel d’origine lui-même, comme dans « N’oubliez pas d’envoyer vos modifications vers l’origine ». |
| amont | À l’instar de l’élément distant d’origine, l’amont est une connexion nommée à un autre référentiel. Dans ce workflow, l’amont représente la connexion entre votre référentiel local et le référentiel principal, à partir duquel votre double a été créé. Il est parfois utilisé comme Moniker pour le référentiel en amont lui-même, comme dans « N’oubliez pas d’extraire vos modifications depuis l’amont ». |

Si vous ne connaissez pas les concepts Git et GitHub tels qu’un référentiel ou une branche, consultez d’abord l’article [Git and GitHub fundamentals](git-fundamentals.md).

## Workflow

>[!IMPORTANT]
> Si vous ne l’avez pas encore fait, vous devez suivre la procédure de la section [Setup](github-signup.md).

Dans ce workflow, les modifications s’effectuent en suivant un cycle répétitif. À partir du référentiel local de votre appareil, elles refluent vers votre double GitHub, puis vers le référentiel GitHub principal, pour ensuite revenir au référentiel local lorsque vous intégrez les modifications d’autres contributeurs.

### Utilisation du flux GitHub

L’article [Git and GitHub fundamentals](git-fundamentals.md) rappelle qu’un référentiel Git contient une branche principale, ainsi que d’autres branches de travail en cours qui n’ont pas été intégrées à la branche principale. Chaque fois que vous introduisez un ensemble de modifications logiquement liées, il est recommandé de créer une *branche de travail* pour gérer vos modifications tout au long du workflow. Nous l’appelons ici branche de travail, car il s’agit d’un espace de travail permettant d’itérer/affiner les modifications jusqu’à ce qu’elles puissent être intégrées à la branche principale.

L’isolation des modifications liées à une branche spécifique vous permet de contrôler et d’introduire ces modifications indépendamment, en les ciblant à une heure de publication spécifique du cycle de publication. En réalité, en fonction du type de travail que vous réalisez, vous pouvez facilement obtenir plusieurs branches opérationnelles dans votre référentiel. Il n’est pas rare de travailler simultanément sur plusieurs branches, chacune représentant un projet différent.

>[!NOTE]
>
>Il *n’est pas recommandé* d’apporter vos modifications à la branche principale. Imaginez que vous utilisiez la branche principale pour introduire un ensemble de modifications à une publication de fonctionnalité planifiée. Vous avez terminé les modifications et vous attendez avant de les publier. Ensuite, pendant ce temps, une requête urgente vous demandant de corriger quelque chose vous parvient. Vous apportez donc la modification à un fichier dans la branche principale et vous la publiez. Dans cet exemple, vous publiez par inadvertance le correctif *et* les modifications que vous attendiez de publier à une date spécifique.

L’étape suivante consiste à créer une branche opérationnelle dans votre référentiel local afin de tenir compte de vos modifications proposées. Chaque client Git est différent. Vous pouvez donc consulter l’aide relative à votre client préféré. Vous pouvez afficher un aperçu du processus dans le guide GitHub sur [GitHub flow](https://guides.github.com/introduction/flow/).

## Traitement de la requête de tirage

Vous envoyez les modifications proposées en les regroupant dans une nouvelle requête de tirage ajoutée à la file d’attente de requêtes de tirage du référentiel de destination. Une requête de tirage active le modèle de collaboration de GitHub en demandant les modifications de votre branche opérationnelle à extraire et à fusionner dans une autre branche. Dans la plupart des cas, cette branche est la branche par défaut/principale du référentiel principal.

### Validation

Avant que votre requête de tirage ne puisse être fusionnée dans sa branche de destination, il peut être nécessaire de passer par un ou plusieurs processus de validation de requête de tirage. Les processus de validation peuvent varier selon la portée des modifications proposées et les règles du référentiel de destination. Une fois votre requête de tirage envoyée, vous pouvez vous attendre à ce que le contenu soit examiné et, le cas échéant, fusionné dans le référentiel principal.

### Révision et validation

Une fois le traitement des requêtes de tirage terminé, vérifiez les résultats (commentaires sur les requêtes de tirage, URL d’aperçu, etc.) afin de déterminer s’il est nécessaire d’apporter des modifications supplémentaires à ses fichiers avant de valider la fusion. Si un réviseur s’est penché sur votre requête de tirage, il peut également fournir des commentaires en cas de problèmes/questions en suspens avant la fusion.

Lorsque la requête de tirage ne présente pas de problème et est validée, vos modifications sont fusionnées dans la branche parent et la requête de tirage est clôturée.

### Publication

Souvenez-vous que la requête de tirage doit être fusionnée par un réviseur de requête de tirage avant que les modifications ne puissent être incluses dans le prochain cycle de publication planifié. Les requêtes de tirage sont normalement examinées/fusionnées dans l’ordre de la soumission. Si votre requête de tirage nécessite une fusion pour un cycle de publication spécifique, vous devrez préalablement collaborer avec votre réviseur de requête de tirage pour vous assurer que la fusion se produit avant la publication.
