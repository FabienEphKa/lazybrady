<p align="center"><img src="logo-lazybrady.png" width="112" alt="Logo LazyBrady, un paresseux dans une loupe"></p>

<h1 align="center">LazyBrady</h1>

<p align="center"><strong>Une app macOS pour chercher des offres et suivre ses candidatures en France.</strong></p>

<p align="center">Projet personnel · En développement depuis le 3 novembre 2026 · Version actuelle 0.7.134</p>

LazyBrady est née d’un besoin personnel : retrouver au même endroit les offres qui correspondent à mes critères, les candidatures envoyées et les réponses reçues.

J’ai souvent la flemme, d’où le *Lazy*. J’ai ajouté *Brady* en clin d’œil à *Bradypus*, le genre des paresseux à trois doigts. Comme quoi, la flemme peut aussi donner naissance à une app.

## Ce que fait LazyBrady

- **Recherche d’offres** selon les critères définis dans l’app, notamment le métier, la zone géographique, le type de contrat et la date de publication.
- **Préparation des candidatures** à partir du profil et du CV, avec un modèle d’IA qui tourne sur le Mac. Sur les parcours pris en charge, l’app peut aussi remplir le formulaire et envoyer la candidature.
- **Suivi des démarches** avec les candidatures enregistrées, les confirmations des plateformes et les dossiers à vérifier. Quand une étape demande une intervention, le passage peut reprendre au point enregistré.
- **Tri des accusés Gmail** pour mettre à la corbeille les notifications automatiques identifiées. Les échanges utiles, comme les propositions d’entretien ou les demandes de pièces, restent disponibles.

## Pourquoi j’ai développé ma propre extension Chrome

Dans mes premiers essais avec Playwright, Chrome revenait régulièrement au premier plan. Ça interrompait ma navigation et me gênait même quand je travaillais dans une autre application.

Je me suis inspiré de l’extension Chrome de ChatGPT et de sa façon de travailler sur des onglets sans les afficher. J’ai développé ma propre extension, à laquelle LazyBrady se connecte. Elle pilote les groupes d’onglets de travail de LazyBrady en arrière-plan, pendant que je continue à utiliser mes onglets habituels ou d’autres applications. Si une étape demande mon intervention, l’app peut me prévenir.

## Gmail, en arrière-plan

Après une première autorisation Google, LazyBrady peut vérifier le courrier à intervalles réguliers via **l’API Gmail**. La vérification passe par l’app et peut continuer quand sa fenêtre est fermée, tant que LazyBrady tourne dans la barre des menus et que le Mac reste éveillé.

Le tri automatique attend la fin du passage de recherche. Il met à la corbeille les accusés automatiques qu’il peut rattacher à une candidature confirmée. Les réponses des recruteurs, les propositions d’entretien, les demandes de documents et les messages incertains restent dans Gmail. Une vérification manuelle est aussi disponible.

## Sites d’emploi configurés

| Plateforme | Parcours actuel |
| --- | --- |
| **France Travail** | Recherche via l’API, puis consultation et candidature dans Chrome quand le parcours le permet. |
| **LinkedIn** | Recherche et candidatures simplifiées. |
| **Indeed** | Recherche et traitement des formulaires de candidature intégrés à Indeed. |
| **Apec** | Recherche et traitement des candidatures proposées directement sur l’Apec. |

Les parcours évoluent avec les plateformes. Les formulaires incomplets et les vérifications demandées par les sites peuvent nécessiter une intervention.

## Visite de l’app

| Écran | À quoi il sert |
| --- | --- |
| **Vue d’ensemble** | Lancer ou reprendre une recherche, voir les sources actives et retrouver les compteurs de candidatures. |
| **Sources & comptes** | Choisir les sites à parcourir, leur ordre et les réglages propres à chacun. |
| **Offres** | Lire les annonces examinées et consulter le résultat du tri, avec le motif de chaque décision. |
| **Candidatures** | Consulter le suivi, les enregistrements des plateformes et les dossiers qui restent à vérifier. |
| **Mes consignes** | Définir les métiers recherchés, la zone, la période, les contrats et les exclusions. |
| **Mon profil** | Importer le CV et un export LinkedIn, puis consulter les faits utilisés pour préparer les réponses. |
| **Modèles locaux** | Configurer le moteur d’IA qui tourne sur le Mac. |
| **Courrier** | Relier Gmail, régler la fréquence des vérifications et consulter les décisions de tri. |
| **Version portable** | Préparer une copie de l’app et de ses données à déplacer ensemble. |
| **Chrome autonome** | Vérifier la liaison avec l’extension, piloter les passages et gérer les alertes. |
| **Journal** | Retrouver les opérations effectuées et les étapes qui ont demandé une intervention. |

## Aperçu

![Vue d’ensemble de LazyBrady avec des données fictives](vue-ensemble.jpg)

<details>
<summary>Voir l’écran Courrier</summary>

![Vérification Gmail en arrière-plan avec un compte de démonstration masqué](courrier.jpg)

</details>

<details>
<summary>Voir Chrome autonome et le moteur d’IA local</summary>

![LazyBrady, travail en arrière-plan dans Chrome et notifications](chrome-autonome.jpg)

![LazyBrady, configuration du moteur d’IA local](moteur-local.jpg)

</details>

Les vues d’ensemble et Courrier utilisent des données de démonstration. Le nom du modèle local est masqué dans sa capture.

## État du projet

**LazyBrady est en développement et je l’utilise d’abord pour ma propre recherche d’emploi.** Cette page présente le projet. L’application, l’extension Chrome et le code source sont privés à ce stade.

Mon objectif est de rendre LazyBrady accessible au public **en France uniquement**, une fois les parcours suffisamment fiables pour une utilisation au-delà de mon propre profil. La date et les modalités de cette ouverture restent à définir.
