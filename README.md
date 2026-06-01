# 🦾 SO-ARM101 : Développement d'un Préhenseur Souple (Soft Gripper)

![Bannière du projet ou photo de ton préhenseur](lien_vers_une_image_ici.jpg)

*Ce dépôt a été créé dans le cadre d'un stage de recherche chez [Nom du labo / Polytech / Entreprise], encadré par [Nom de ton maître de stage].*

---

## 📖 Introduction

Ce projet vise à étendre les capacités du bras robotique open-source **SO-ARM101** en lui ajoutant un effecteur terminal (préhenseur) de type "Soft Robotics". 
Contrairement aux pinces rigides traditionnelles, un préhenseur souple permet de manipuler des objets fragiles, de formes complexes ou inconnues, en s'adaptant naturellement à leur géométrie (compliance).

📝 **[Lire le rapport de recherche complet (PDF)](docs/Rapport_Recherche_TonNom.pdf)**

## 🎯 Objectifs du Projet

1. **Étude et conception :** Modélisation d'un préhenseur souple (CAO sous Autodesk Fusion).
2. **Fabrication :** Impression 3D utilisant des matériaux flexibles (ex: TPU 95A ou silicone) et des structures rigides (PLA/PETG) pour l'interface avec le SO-ARM101.
3. **Contrôle :** Intégration logicielle de l'actionnement du préhenseur.
4. **Validation :** Tests de préhension sur divers objets (fragiles, asymétriques) et analyse des performances.

## 📂 Arborescence du dépôt

```text
📦 SO-ARM101-SoftGripper
 ┣ 📂 CAD/             # Fichiers sources (Fusion 360, .STEP)
 ┣ 📂 STL/             # Fichiers prêts à imprimer (.STL / .3MF)
 ┣ 📂 docs/            # Compte-rendu de recherche, documentation et schémas
 ┣ 📂 src/             # Code source pour le contrôle (Python, C++...)
 ┗ 📜 README.md        # Ce fichier