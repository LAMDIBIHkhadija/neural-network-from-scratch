# Réseau de Neurones pour la Classification du Dataset MNIST

Ce projet implémente un réseau de neurones à partir de zéro pour la classification des chiffres manuscrits du dataset MNIST. Plusieurs techniques d'optimisation sont explorées, notamment la descente de gradient classique, le momentum, Adagrad, et la Propagande Stochastique Approximative (PSA).

## Description du Projet

L'objectif de ce projet est de construire un réseau de neurones simple et d'implémenter manuellement les mécanismes d'apprentissage et d'optimisation. Les étapes incluent :  
1. Chargement et prétraitement des données.  
2. Construction d'un réseau de neurones à deux couches.  
3. Entraînement et évaluation du modèle.  
4. Exploration de diverses techniques d'optimisation.  

## Structure du Projet

### Prétraitement des Données
- Chargement du dataset MNIST via `scikit-learn`.  
- Normalisation des images pour des valeurs entre 0 et 1.  
- Transformation des labels en vecteurs one-hot.  

### Modèle
- Une **couche cachée** avec une activation `tanh`.  
- Une **couche de sortie** avec l'activation `softmax`.  
- Fonction de coût : **Entropie Croisée**.  

### Optimisations
1. **Descente de Gradient Classique**.  
2. **Momentum** : Accélération de la convergence en utilisant la vitesse.  
3. **Adagrad** : Ajustement dynamique des taux d'apprentissage.  
4. **Propagande Stochastique Approximative (PSA)** : Technique innovante permettant une convergence rapide en combinant des propriétés des méthodes stochastiques et des approximations des gradients.  

### Entraînement
- **Propagation Avant** : Calcul des prédictions.  
- **Rétropropagation** : Calcul des gradients pour mettre à jour les poids.  
- Suivi de la perte et de la précision à chaque époque.  

### Évaluation
- Calcul de la précision du modèle sur le jeu de test.

## Résultats

- **Descente de Gradient Classique** : Convergence lente mais fiable.  
- **Momentum** : Meilleure convergence grâce à une accélération.  
- **Adagrad** : Bonne performance pour les données clairsemées.  
- **PSA** : Convergence rapide et résultats compétitifs par rapport aux autres méthodes.  


## Auteur

Ce projet a été réalisé dans un but pédagogique pour explorer les bases des réseaux de neurones et des algorithmes d'optimisation.
