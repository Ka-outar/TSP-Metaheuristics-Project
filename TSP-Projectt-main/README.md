# 🌍 Projet M1 : Comparaison de Métaheuristiques pour le TSP

**Université Hassan II de Casablanca - ENSET Mohammedia** **Master :** SDIA (Sciences des Données et Intelligence Artificielle)  
**Module :** Optimisation & Métaheuristiques  
**Encadrant :** Prof. MESTARI  

## 👥 Réalisé par :
* **Timourti Sana**
* **Misbah Kaoutar**
* **Essayouti Atiqa**


---

## 📝 Description du Projet

Ce projet vise à résoudre le célèbre **Problème du Voyageur de Commerce (TSP)** en comparant trois approches d'optimisation :

1. 🏔️ **Hill Climbing (Best Improvement)** : Une méthode de recherche locale simple cherchant le meilleur voisin.
2. 🔄 **Multi-Start Hill Climbing** : Une amélioration du Hill Climbing qui relance la recherche depuis plusieurs points de départ aléatoires pour éviter les optimums locaux.
3. 🔥 **Recuit Simulé (Simulated Annealing)** : Une métaheuristique capable d'échapper aux optimums locaux en acceptant temporairement de moins bonnes solutions.

L'objectif est d'analyser leur performance et leur temps de convergence sur des instances de 20 et 50 villes.

---

## 📊 Résultats Clés (Exemple Instance 50 Villes)

Nos expérimentations montrent que le **Recuit Simulé** et le **Multi-Start** sont nettement supérieurs au Hill Climbing classique pour les grandes instances :

| Algorithme | Meilleur Coût (Distance) | Temps d'exécution |
| :--- | :--- | :--- |
| **Hill Climbing (Best)** | ~ 1495.21 | ~ 0.44s |
| **Multi-Start HC** | *Meilleur que HC* | *Variable* |
| **Recuit Simulé** | **~ 784.40** 🏆 | ~ 0.47s |

> **Analyse :** Le Hill Climbing stagne rapidement dans un optimum local. Le Multi-Start aide à corriger cela en relançant la recherche, tandis que le Recuit Simulé surpasse les autres en explorant l'espace de recherche plus intelligemment.

---

## 📈 Courbes de Convergence

Les graphiques ci-dessous montrent l'évolution de la distance totale au fil des itérations.

### 🔹 Instance A (20 Villes)
![Convergence 20 villes](screenshots/convergence_20.png)

### 🔹 Instance B (50 Villes)
![Convergence 50 villes](screenshots/convergence_50.png)

---

## ⚙️ Installation et Exécution

**1️⃣ Cloner le projet**
```bash
git clone [https://github.com/Ka-outar/TSP-Metaheuristics-Project.git](https://github.com/Ka-outar/TSP-Metaheuristics-Project.git)
cd TSP-Metaheuristics-Project
