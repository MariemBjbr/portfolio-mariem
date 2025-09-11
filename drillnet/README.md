# Drill_net_classification – Projet de stage
<img width="1300" height="737" alt="image" src="https://github.com/user-attachments/assets/1d90242f-f55a-4444-874e-3c66e4b6f716" />


Ce projet a été réalisé dans le cadre de mon **stage en apprentissage automatique appliqué à l’imagerie médicale**.  
L’objectif était de développer un modèle de deep learning capable de **détecter automatiquement deux biomarqueurs sur des images OCT** :
- **DRIL** (*Disorganization of Retinal Inner Layers*)  
- **Discontinuités (DISC)* des couches rétiniennes

## Ce que j’ai fait
- Création d’un **pipeline complet** d’entraînement et d’évaluation du modèle.
- Utilisation d’un modèle **CNN (ResNet18)** adapté aux images OCT.
- Mise en place de techniques pour améliorer la robustesse :
  - Optimiseur **AdamW** avec régularisation L2.
  - Scheduler de **warm-up suivi d’un décroissance cosinus** pour le taux d’apprentissage.
  - **Early stopping** basé sur la F1-score de la classe positive.
- Évaluation du modèle sur un jeu de test indépendant.

---

## Résultats obtenus
- **Accuracy (test)** : 0.84  
- **F1-score (classe DRIL/DISC)** : 0.86  
- Bon rappel (0.88) → le modèle détecte bien les cas positifs.  
- Le modèle est donc **valable pour la détection des deux biomarqueurs**.

---

## Impact
Ce travail montre qu’il est possible de développer des outils d’IA qui assistent les médecins dans la détection de biomarqueurs sur OCT.  
Le modèle DrillNet constitue une **preuve de concept** pour un système d’aide au diagnostic en ophtalmologie.
