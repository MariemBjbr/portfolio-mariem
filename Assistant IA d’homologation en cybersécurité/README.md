Assistant IA d’homologation en cybersécurité (Hydro-Québec)
🎯 Contexte

Ce projet s’inscrit dans le cadre du projet intégrateur final (INF8970 / INF8980 / INF8985) en collaboration avec Hydro-Québec.
Objectif : développer un assistant IA basé sur un LLM et une approche RAG (Retrieval Augmented Generation) pour aider les intégrateurs de systèmes à analyser les guides d’installation et à identifier les failles de sécurité dans les environnements TO (Technologies Opérationnelles).

🏗️ Choix de l’architecture

Nous avons adopté une architecture hexagonale car :

Elle est modulaire : chaque fonctionnalité peut être développée indépendamment.

Elle facilite l’ajout de nouvelles capacités sans impacter le reste du code.

Elle correspond aux bonnes pratiques de conception logicielle pour des projets collaboratifs.

🧩 Architecture simplifiée (version actuelle)
           ┌──────────────────┐
           │  Ports / Adapters│  ← (sources externes : JSON, MITRE, guides, API)
           └─────────┬────────┘
                     │
             ┌───────▼────────┐
             │  Core (RAG+LLM)│  ← (analyse croisée, génération de recommandations)
             └───────┬────────┘
                     │
           ┌─────────▼─────────┐
           │   Interface UI    │  ← (chatbot, affichage des résultats)
           └───────────────────┘

📅 Statut du projet

📌 Projet en cours

📆 Remise finale prévue : 5 décembre 2025

✅ Étape actuelle : mise en place du cœur (RAG + LLM) et intégration des premiers adaptateurs.

👩‍💻 Contribuer

Chaque membre peut développer son module indépendamment (ex. ingestion JSON, indexation, UI…) sans toucher au code des autres.
Merci de respecter l’architecture hexagonale pour garantir l’évolutivité et la modularité.
