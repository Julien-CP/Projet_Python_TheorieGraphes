# Projet de Recherche Opérationnelle

Projet réalisé dans le cadre du cours *Théorie des graphes* — L3 Mathématiques à EFREI Paris.

## Présentation

Ce projet implémente un programme complet d'ordonnancement basé sur la théorie des graphes. À partir de tableaux de contraintes décrivant des tâches avec durées et dépendances, le programme construit un graphe, détecte les erreurs (circuits, arcs négatifs), puis calcule et affiche :

- le **calendrier au plus tôt**,
- le **calendrier au plus tard**,
- les **marges**,
- les **chemins critiques** (chemins les plus longs),
- ainsi que les **rangs** des sommets.

Le graphe est également représenté sous forme **matricielle** et **visuelle** (fichier HTML généré avec PyVis).

## Membres du projet

- Julien CHAN PENG  
- Adrien ASSOUAD  
- Thibault BIAL  
- Alexandre MUNIER  
- Catherine NGANGO KOLOKO

## Fonctionnalités

1. **Lecture de fichiers de contraintes**  
   - Lecture d’un fichier `.txt` décrivant les tâches, durées et dépendances.
   - Construction automatique des tâches fictives `α (0)` et `ω (N+1)`.

2. **Construction du graphe**  
   - Création d’un graphe orienté à partir des contraintes.
   - Affichage visuel et matriciel du graphe.

3. **Vérifications préalables**  
   - Détection d’**arcs à valeur négative**.
   - Détection de **circuits** à l’aide d’un algorithme de parcours en profondeur.

4. **Analyse d’ordonnancement**  
   - Calcul des **rangs** (grâce à un parcours en largeur).
   - Calcul des **dates au plus tôt** et **au plus tard**.
   - Calcul des **marges** et **chemins critiques**.

5. **Traces d’exécution automatiques**  
   - Génération automatique des fichiers `.txt` de trace pour chaque tableau testé.
   - Possibilité de tester une table à la fois ou l’ensemble des 14 tables fournies.

6. **Visualisation**  
   - Graphe interactif généré en HTML via PyVis.
   - Tableaux formatés avec BeautifulTable pour une meilleure lisibilité.

## Exécution du programme principal

### Lancer le programme :

```bash
python E5_main.py
