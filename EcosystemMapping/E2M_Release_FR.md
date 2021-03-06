Un modèle pour la cartographie sémantique d'écosystème
==

Tags
-
#EcosystemMapping #SemanticCartography #MapYourEnvironment #EffectuationMethodology #CompetitiveWatch #ProductWatch #MarketWatch #TechnologyWatch #ProductLifecycleManagement 

Introduction
-
Chacun d'entre nous, pour des __raisons diverses et variées__ (e.g. veille concurrentielle, veille produit, étude de marché, veille technologique, démarche entrepreneuriale, développement de produit, ...) sommes à conduit à "cartographier", __plus ou moins formellement__ (et en utilisant des outils __plus ou moins adaptés__), l'environnement dans lequel on évolue actuellement (ou celui dans lequel on souhaite évoluer dans le futur) !

En effet, cartographier son environnement permet d'avoir une vision à la fois globale et précise de celui-ci ...   
... afin de pouvoir mieux agir dessus.

Le modèle E2M (Ecosytem Mapping Model) visent à répondre à ce besoin en proposant :
* Une approche méthodologique
* Un modèle (décliné selon différents formalismes)
* Des propositions d'outils cibles (selon les fonctions requises et l'usage)

Problématique à résoudre
-
Les environnements ont beau être potentiellement __très différents__ d'un cas à l'autre, il s'avère que les questions que l'on se posent à leur propos, mais égalements concepts qui *structurent* ces environnements sont - globalement - toujours les __mêmes__ (ce sont en quelque sorte les *invariants métiers* du domaine de connaissances "ecosystem mapping").

En effet, lorsqu'on cherche à __appréhender un écosystème__, on essaye __essentiellement__ de répondre au __quintuple questionnement__ suivant : 
* QUOI ?
* Fait QUOI ?
* COMMENT ?
* Pour QUOI ?
* Et POURQUOI ?

![Questions](https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/images/Who-DoesWhat-How-ForWhat-Why.png)

Il est évidement possible de se poser d'autres questions très pertinentes à propos de son environnement, toujours est-il que le périmètre de E2M est - pour l'instant - limité à ces 5 questions ;-)

Approche méthodologique
-
L'approche méthodologique permettant de proposer le modèle E2M s'appuie principalement sur le fait de distinguer en chaque chose que l'on doit identifier dans la "carte" (afin de pouvoir la mettre en relation avec d'autres éléments) : 
* d'une part son "intention" (notion qui renvoi à la raison pour laquelle la chose doit être identifiée)
* d'autre part son "extension" (notion qui renvoi à la nature de la chose)

Un article décrivant plus en détail cette approche "Intention VS Extension" est disponible <a href="https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/1_Semantic/ReasonWhyA2-LevelModel_FR.md">ici</a>.

L'expérience montre que globalement, __l'intention est plus importante que l'extension__, et que souvent les modèles sont "pollués" par l'extension des choses (lorsqu'ils sont conçus de manière trop "monolithique"). 

Gérer ces 2 notions de manière "orthogonales" (i.e. "indépendamment", mais en possible connexion) permet de disposer d'un modèle plus compact, plus robuste et plus évolutif, car basé sur 2 modules clefs :
* un module "intensionnel" qui apporte de la généricité et permet d'adresser une grande diversité d'écosystèmes
* un module "extensionnel" qui apporte de la spécificité et qui sert de "racine" à des sous-modules permettant d'adresser des écosystèmes particuliers 

Sémantique Sous-Jacente
-
Un <a href="https://github.com/iPlumb3r/EcosystemMappingModel/tree/master/1_Semantic/Conceptionary">conceptionary</a> permet de decrire les concepts utilisé par E2M   
_(Work in progress ...)_

Le modèle conceptuel simplifié permet de visualer "grosse maille" les relation entres concepts intentionnels et concepts extensionnels :
![TM Ontology](https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/images/ConceptualModel%40E2M_2020-03-04.png)

Fonctionnalités recherchées
-
Réaliser une telle carte nécessite - idéalement - de pouvoir s'appuyer sur 2 modes fonctionels diamétralement opposés, mais totalement complémentaires. Il s'agit des modes suivants :
* Mode "Model-Driven"
* Mode "Model-Discovery" 

Remarque : Le 2nd mode, requiert - là encore idéalement - un mode de réconciliation en complément

Plus d'information sur ces modes fonctionnels <a href="https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/4_Functionalitites/FunctionalModes.md">dans cette page</a>

Ontologies correspondantes
-
Le modèle E2M est décliné pour les 3 formalismes suivants ...   
... et adapté pour certains outils :

<table>
    <thead>
        <tr>
            <th>Ontologie</th>
            <th>Outil</th>
            <th>Mode</th>
            <th>Usage</th>   
            <th>Commentaires</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>OWL</td>
            <td>N'importe que outil "OWL-Compliant"</td>
            <td>En fonction de l'outil</td>
            <td>En fonction de l'outil</td>
            <td>En attente de <a href="http://semapps.org/">SemApps</a></td>
        </tr>
        <tr>
            <td>Topic Maps</td>
            <td>Par exemple pour <a href="https://www.topincs.com/">Topincs</a></td>
            <td>Mode "Model-Driven" uniquement</td>
            <td>Web / Multi-Utilisateur</td>
            <td>Cf <a href="https://www.topincs.com/iPlumb3rSandBox/">"Entangled Bootstrap" Repository (EBR)</a></td>
        </tr>
        <tr>
            <td>KL</td>
            <td>Uniquement pour <a href="http://keeplink.com/">KeepLink</a></td>
            <td>Mode "Model-Driven" et "Model-Discovery" (sans réconsiliation)</td>
            <td>iDevice / Mono-Utilisateur (Mode "Collaboration" à venir)</td>
            <td>En cours de paramétrage du modèle</td>
        </tr>
    </tbody>
</table>

Ci-joint les liens vers les différentes spécification d'ontologies :
* <a href="https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/6_Ontologies/OWL-Ontology.md">OWL Ontology</a>
* <a href="https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/6_Ontologies/TM-Ontology.md">Topic Maps Ontology</a>
* <a href="https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/6_Ontologies/KL-Ontology.md">KeepLink Ontology</a>

Module "Intentionnel" (Simplifié) 
-
![OWL Ontology](https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/images/OWL-Ontology%40E2M-i_Simplified_2020-03-04.png)


Modules "Intentionnel" & "Extensionnel" (Complet)
-
![OWL Ontology](https://github.com/iPlumb3r/EcosystemMappingModel/blob/master/images/OWL-Ontology%40E2M_2020-03-06.png)

Ressources
-
GitHub : <a href="https://github.com/iPlumb3r/EcosystemMappingModel">E2M Repository</a>   
Telegram : <a href="https://t.me/EntangledBootstrap">"Entangled Bootstrap" Repository (EBR) Group"</a> (Projets liés)   
Twitter : <a href="https://twitter.com/iPlumb3r">Semantic Cartography Flux</a>


