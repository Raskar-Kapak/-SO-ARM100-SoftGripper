# Journal — Semaine 1 (du 01/06 au 05/06)

## ✅ Ce que j'ai fait cette semaine
- Recherche sur l'état de l'art des différentes technologies de préhenseurs souples.
- Modélisation 3D d'un préhenseur à effet Fin Ray (FRE) intégrant une bride de fixation rigide (*Fixed Clamp*), en m'appuyant sur les travaux et résultats de Sheikhsofla et al.
- Prise en main de la bibliothèque open-source LeRobot (Hugging Face) via l'environnement virtuel Miniforge.
- Calibration des axes et prise de contrôle du bras robotique (téléopération au clavier et contrôle direct via des requêtes Python).

## 🧠 Ce que j'ai appris
- Découverte approfondie des mécanismes et des technologies liés aux préhenseurs souples.
- Fonctionnement de l'interface logicielle et de l'API de LeRobot.
- Compréhension de l'architecture logicielle sous Windows (notamment le rôle du dossier `src/`) et du système de parsing des arguments avec la bibliothèque `draccus`.

## 🚧 Difficultés rencontrées
- **Problème :** Crash logiciel systématique (`StopIteration` / déconnexion) au moment d'activer le couple des moteurs.
- **Tentatives :** Création de scripts Python minimaux pour isoler le problème, puis exécution d'une lecture des positions à vide.
- **Statut :** **Résolu**. Après diagnostic, il s'est avéré que le bras utilisé est configuré comme un *Leader* (utilisé uniquement pour lire les valeurs des potentiomètres internes en vue de la téléopération) et non un *Follower* (qui nécessite du couple/tension pour agir physiquement). Demander du couple à ce bras spécifique provoquait donc une erreur logique de sous-tension/plantage.

## 💡 Idées & observations
- L'utilisation de brides de fixation rigides (*Fixed Clamps*) semble être une solution très prometteuse pour augmenter significativement la force de préhension des effecteurs souples.
- **Projet de test :** Création future d'un banc d'essai équipé d'un dynamomètre. Cela permettrait d'évaluer et de comparer objectivement la force de maintien (*grip*) de différentes configurations : préhenseur rigide standard, FRE classique, FRE + *Fixed Clamp*, Silicone, et Silicone + *Fixed Clamp*.

## 📋 Plan pour la semaine prochaine
- [ ] Impression 3D de la V1 du préhenseur souple FRE avec sa bride de fixation rigide.
- [ ] Rédaction de scripts Python autonomes permettant au bras d'exécuter des séquences de mouvements simples (avec le préhenseur actuel, puis avec le FRE gripper une fois monté).

## ❓ Questions pour l'encadrant
-