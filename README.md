# Simulation numérique d’équations hyperboliques – Loi de conservation scalaire

## Description
Ce projet est dédié à la **résolution numérique des équations hyperboliques de conservation** en 1D, via des **méthodes de volumes finis**.  
L’objectif principal est d’implémenter, comparer et analyser différents schémas numériques pour capturer des phénomènes physiques fondamentaux : **ondes de choc, ondes de détente et régularisation**.

Ce travail combine **rigueur mathématique**, **implémentation algorithmique** et **analyse numérique avancée**.

---

## Objectifs
- Implémenter des **schémas de volumes finis** pour des équations de conservation.  
- Étudier le **problème de Riemann** pour différentes conditions initiales.  
- Comparer trois méthodes numériques :
  - **Godunov** : précis mais coûteux (résolution du problème de Riemann).  
  - **Rusanov** : plus diffusif mais simple.  
  - **Roe** : compromis entre précision et complexité.  
- Évaluer les **effets des conditions aux limites** (Neumann, périodiques).  
- Observer l’évolution de solutions régulières et discontinues dans le temps.  

---

##  Méthodologie
1. **Discrétisation en volumes finis**  
   - Schéma explicite basé sur le flux numérique aux interfaces.  
   - Respect de la condition CFL pour garantir stabilité et convergence.  

2. **Flux numériques étudiés**  
   - Godunov : flux basé sur la solution exacte locale du problème de Riemann.  
   - Rusanov : schéma central avec viscosité numérique.  
   - Roe : linéarisation locale pour capturer les discontinuités.  

3. **Cas étudiés**  
   - Conditions initiales discontinues (problèmes de Riemann).  
   - Cas de Burgers (flux convexe et concave).  
   - Cas non linéaire avec flux cubique.  
   - Condition initiale régulière (sinusoïdale).  

---

## Résultats
- **Ondes de détente** et **ondes de choc** sont correctement capturées par les trois méthodes.  
- Les différences principales :  
  - Godunov → fidèle à la solution exacte.  
  - Rusanov → plus diffusif (lissage des discontinuités).  
  - Roe → très bon compromis, mais instable pour certaines fortes discontinuités.  
- Les solutions régulières (sinusoïdales) se dégradent au-delà d’un certain temps, conformément à la théorie.  

---

## Compétences développées
- Simulation numérique d’**équations aux dérivées partielles hyperboliques**.  
- Implémentation de **schémas de volumes finis**.  
- Analyse de stabilité (condition CFL) et validation par comparaison théorique.  
- Programmation scientifique en **Python / MATLAB / Jupyter Notebook**.  
- Visualisation et interprétation de solutions numériques.  

---

## Organisation du projet
- `TP1_système_hyperbolique_2024_2025.pdf` → Rapport détaillé avec explications et validations.  
- `notebooks/` → Implémentations Python (Jupyter) des schémas numériques.  
- `figures/` → Comparaisons visuelles des solutions exactes et numériques.  
- `README.md` → Présentation du projet.  

---

## Perspectives
- Extension à des **systèmes hyperboliques couplés** (équations d’Euler pour les fluides).  
- Étude en **2D** pour la modélisation des ondes et écoulements.  
- Implémentation de **schémas TVD (Total Variation Diminishing)** pour limiter les oscillations spurious.  
- Comparaison avec des solveurs open-source (Clawpack, PyClaw, FEniCS).  

---

## Conclusion:
- Il démontre la capacité à **modéliser et résoudre des PDE complexes**.  
- Il prouve des compétences solides en **analyse numérique et méthodes de volumes finis**.  
- Il met en avant la **programmation scientifique** et la rigueur dans la validation des résultats.  
- Il reflète des aptitudes transférables à l’**ingénierie numérique**, à la **simulation physique** et à la **data science avancée**.
- --
## Auteur
**Bréhima Samaké**  
Janvier 2025  


