**Assistant IA d’homologation en cybersécurité (Hydro-Québec)**

  <img width="927" height="507" alt="image" src="https://github.com/user-attachments/assets/bbef6542-2439-4f7c-9bb6-a764b5fe0585" />

🎯 **Contexte**

Ce projet s’inscrit dans le cadre du projet intégrateur final (INF8970 / INF8980 / INF8985) en collaboration avec Hydro-Québec.
Objectif : développer un assistant IA basé sur un LLM et une approche RAG (Retrieval Augmented Generation) pour aider les intégrateurs de systèmes à analyser les guides d’installation et à identifier les failles de sécurité dans les environnements TO (Technologies Opérationnelles).

🏗️ **Choix de l’architecture**

Nous avons adopté une architecture hexagonale car :

Elle est modulaire : chaque fonctionnalité peut être développée indépendamment.

Elle facilite l’ajout de nouvelles capacités sans impacter le reste du code.

Elle correspond aux bonnes pratiques de conception logicielle pour des projets collaboratifs.

🧩 **Architecture simplifiée (version actuelle)**

 <img width="532" height="218" alt="image" src="https://github.com/user-attachments/assets/6a0714e5-cacd-4044-84c1-0449e144f2ae" />
 
 L'architecture hexagonale, aussi connue sous le nom d'architecture à base de ports et d'adaptateurs, est un patron d'architecture logicielle qui vise à isoler la logique métier d'une application de ses détails techniques et de son environnement. En séparant ces deux aspects par des "ports" (interfaces) et des "adaptateurs" (implémentations techniques), l'hexagone permet une plus grande flexibilité, une meilleure testabilité et une maintenance facilitée, rendant le système plus robuste et évolutif. 
 
 **L'hexagone (le noyau métier)**:
 
 Le cœur de l'application, qui contient la logique métier "pure" et est indépendant des technologies. 
 
**Les ports** :

 Les interfaces définies par le noyau métier pour interagir avec l'extérieur. 
 
**Les adaptateurs**:

 Des composants qui font le lien entre l'extérieur (interfaces utilisateur, bases de données, autres systèmes) et les ports de l'hexagone, traduisant les appels et les données. 
 
**Les dépendances inverses**:

Les dépendances vont toujours de l'extérieur vers le centre (l'hexagone). 

**Avantages**

**Faible couplage**: Le noyau métier est indépendant de l'infrastructure, ce qui permet de changer de base de données, d'interface utilisateur ou d'autres services sans affecter la logique métier. 

**Facilité de test**: Le noyau métier peut être testé en isolation grâce à des adaptateurs qui simulent l'environnement technique (mocks), permettant des tests unitaires approfondis. 

**Évolutivité et maintenance**: Il est plus facile d'ajouter de nouvelles fonctionnalités ou de modifier des existantes sans risquer des régressions fonctionnelles. 

**Flexibilité**: L'application peut être pilotée par différents types d'interfaces (utilisateur, tests automatisés, scripts) ou interagir avec divers systèmes externes. 

📅 **Statut du projet**

📌 *Projet en cours*

📆 *Remise finale prévue* : 5 décembre 2025

✅ Étape actuelle : mise en place du cœur (RAG + LLM) et intégration des premiers adaptateurs.


