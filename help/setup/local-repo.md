---
title: Configuration locale du référentiel Git
seo-title: Configuration locale du référentiel Git pour la documentation Adobe
description: Cet article vous sert de guide lorsque vous créez votre référentiel Git local et contribuez à la documentation Adobe, notamment en ce qui concerne le processus de duplication et de clonage.
seo-description: Cet article vous sert de guide lorsque vous créez votre référentiel Git local et contribuez à la documentation Adobe, notamment en ce qui concerne le processus de duplication et de clonage.
translation-type: ht
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---

# Configuration locale du référentiel Git pour la documentation

Cet article décrit les étapes de configuration d’un référentiel Git sur votre ordinateur local, dans le but de contribuer à la documentation Adobe. Les contributeurs peuvent utiliser un référentiel cloné localement pour ajouter de nouveaux articles, effectuer des modifications majeures sur des articles existants ou modifier les illustrations.

> [!IMPORTANT]
> Si vous apportez uniquement des modifications mineures à un article, il n’est *pas* nécessaire de suivre les étapes décrites dans cet article. Vous pouvez simplement cliquer sur l’icône Edit et effectuer les modifications textuelles dans votre navigateur.

## Aperçu

Pour contribuer à la documentation Adobe, vous pouvez dupliquer le référentiel approprié dans votre compte GitHub afin de disposer des autorisations de lecture/écriture. Vous pouvez ensuite créer et modifier des fichiers Markdown en local en clonant le référentiel de documentation correspondant. Ensuite, vous utilisez des requêtes de tirage pour fusionner (soumettre) les modifications dans le référentiel partagé central en lecture seule.

* Déterminer le référentiel approprié
* Dupliquer le référentiel de votre compte GitHub
* Choisir un dossier local pour les fichiers clonés
* Cloner le référentiel sur votre ordinateur local
* Configurer la valeur distante en amont

## Déterminer le référentiel

Vous dupliquez le référentiel approprié de votre compte GitHub afin de disposer des autorisations de lecture/écriture pour y stocker vos modifications proposées. [!UICONTROL Adobe Experience Cloud] la documentation se trouve dans plusieurs référentiels différents sur [github.com](https://www.github.com/adobedocs).

1. Si vous n’êtes pas sûr du référentiel à utiliser, consultez l’article à l’aide de votre navigateur Web. Sélectionnez le lien **Edit** (icône en forme de crayon) dans l’angle supérieur droit de l’article. (Si vous ne voyez pas de lien Edit, ce contenu n’est pas encore disponible dans GitHub.)

Pour contribuer à la documentation Adobe, vous pouvez créer et modifier des fichiers Markdown en local en clonant le référentiel de documentation correspondant. Ensuite, vous utilisez des requêtes de tirage pour fusionner les modifications dans le référentiel partagé central en lecture seule.

<!---
![GitHub Triangle](/assets/git-and-github-initial-setup.png)

If you're new to GitHub, watch the following video for a conceptual overview of the forking and cloning process:

>[!VIDEO https://channel9.msdn.com/Blogs/CoolMoose/Git-Repository-Setup/player]
-->

## Dupliquer le référentiel

À l’aide du référentiel approprié, créez un double du référentiel dans votre compte GitHub à l’aide du site Web GitHub.

Un double personnel est requis, car tous les référentiels de documentation principaux fournissent un accès en lecture seule, ce qui signifie que vous ne pouvez pas apporter directement des modifications au contenu des référentiels. Pour apporter des modifications, vous devez envoyer une requête de tirage depuis votre double dans le référentiel principal. Pour simplifier ce processus, vous devez d’abord disposer de votre propre copie du référentiel, dans laquelle vous disposez d’un accès en écriture. Un *double* GitHub a cette finalité.

1. Accédez à la page GitHub du référentiel principal et cliquez sur le bouton **Fork** dans l’angle supérieur droit.

   ![Fork GitHub](assets/fork-simple.png)

1. Si vous y êtes invité, sélectionnez la miniature de votre compte GitHub comme destination de la création du double. Cette invite crée une copie du référentiel dans votre compte GitHub, appelée double.

1. Choisissez un nom de dossier facile à mémoriser et à saisir.

   Certains référentiels peuvent être volumineux. Choisissez un emplacement disposant d’un espace disque disponible.

   > [!NOTE]
   > Évitez de choisir un chemin d’accès au dossier local imbriqué dans un autre emplacement de dossier de référentiel Git. Bien qu’il soit acceptable de stocker les dossiers clonés Git les uns à côté des autres, l’imbrication de dossiers Git les uns dans les autres provoque des erreurs au niveau du suivi des fichiers.

## Créer un clone local du référentiel

En créant un clone du référentiel dupliqué, vous téléchargez une copie des fichiers sur votre ordinateur. Lorsque vous êtes prêt, vous pouvez transférer des modifications depuis votre disque local vers le référentiel pour lequel une activité Branchement a été créée sur le serveur. Vous pouvez ensuite envoyer une requête de tirage pour fusionner les modifications en amont vers le référentiel principal.

Ces étapes supposent que vous utilisez GitHub Desktop. Si vous utilisez un autre client, effectuez les ajustements appropriés.

1. Cliquez sur **Clone or download**, puis sélectionnez **Open in Desktop** pour extraire une copie du référentiel (votre double) vers votre ordinateur sur le répertoire actuel.

  ![Cloner le référentiel](assets/clone-pulldown.png)

1. Utilisez GitHub Desktop pour que les fichiers locaux restent synchronisés avec le référentiel forké.

Pour plus d’informations, reportez-vous à la page [Documentation GitHub Desktop](https://help.github.com/desktop/).
