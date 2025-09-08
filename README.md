# Travail Pratique 1: 420-SN1-RE Automne 2025

TP01: Analyse biomécanique

## Objectifs
− Comprendre et appliquer les opérations arithmétiques (chapitre 1)  
− Comprendre et appliquer les fonctions d’affichage (chapitre 1)  
− Utiliser des fonctions de bibliothèques importées (chapitre 2)  

## Pondération
10 % de la note finale.
Le travail comprend trois parties valant chacune 10 points, pour un total de 30 points.


## Durée estimée
Entre 2 et 4 heures au total

## Équipes
Travail à faire en équipe de 2 ou 3 personnes. Aucun travail individuel n’est accepté. **Un travail solo ne sera pas  
corrigé et se verra attribuer la note de 0.**

## Remise
Le travail doit être remis via GitHub Classroom; le=s remises par LÉA ne sont pas acceptées. La date de remise sera  
communiquée par LÉA et sera aussi inscrite dans Github Classroom.

À noter que l'utilisation de Git permet de faire des remises partielles au fur et à mesure de l'avancement du travail.

# Travail à faire
## Contexte
En physiothérapie, l’analyse biomécanique permet d’évaluer les forces, les angles et les vitesses impliqués dans les  
mouvements du corps humain. Ce TP simule un test de flexion-extension du genou, utilisé pour mesurer la performance  
musculaire et la récupération après effort.

## Partie 1: Simulation du mouvement (10 points)
### Prérequis
- Créer un environnement virtuel Python (si ce n'est pas déjà fait)
  - Suivre les instructions dans la section **Optionnel, mais recommandé: Configurer un environnement virtuel** du README.MD du dépôt [420-SN1-RE-A25](https://github.com/plducharme/420-SN1-RE-A25)
  - Votre code doit être dans le fichier `simulation.py` qui vous est fourni dans le dépôt.
  - Inscrire le nom des membres de l'équipe, no de DA et nom d'utilisateur github dans l'espace prévu à cet effet dans le fichier `simulation.py`.
### Objectifs
On cherche à calculer et afficher:
- l'amplitude du mouvement de flexion-extension du genou.
  - L'amplitude est la différence entre l'angle maximal et l'angle minimal atteint pendant le mouvement.
- La vitesse angulaire moyenne du mouvement.
  - La vitesse angulaire moyenne est calculée en divisant l'amplitude par le temps total du mouvement.
- Le travail mécanique effectué pendant le mouvement.
  - Le travail mécanique est calculé en multipliant la force appliquée par la distance parcourue.
    - La distance parcourue peut être approximée en utilisant l'amplitude du mouvement et la longueur du segment de la jambe.

### Variables à générer
- `angle_initial`: 
  - angle initial du genou en degrés
  - float aléatoire entre 0 et 20
  - doit être arrondi à deux décimales
- `angle_maximal_atteint`: 
  - angle maximal atteint pendant le mouvement en degrés
  - float aléatoire entre 90 et 130
  - doit être arrondi à deux décimales
- `temps_execution`: 
  - temps total du mouvement en secondes
  - float aléatoire entre 1.5 et 3.5
  - doit être arrondi à une décimale
- `force_maximale_appliquee`: 
  - force maximale appliquée pendant le mouvement en Newtons
  - float aléatoire entre 150 et 400
  - doit être arrondi à trois décimales

### Autres variables
- `longueur_segment_jambe`:
    - longueur du segment de la jambe en mètres
    - constante fictive de 0.45

