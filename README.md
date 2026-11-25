# Statistiques computationnelles pour le Big Data — codes Python

*Statistiques computationnelles pour le Big Data* — méthodes par lots et méthodes de gradient stochastique pour l'inférence bayésienne.

## Contenu

| Fichier | Contenu | Figures produites |
|---|---|---|
| `01_simulations_chapitres_1_a_3.ipynb` | Méthodes par lots (chapitre 1 : Scott, Neiswanger paramétrique, non paramétrique, semi-paramétrique), méthodes de gradient stochastique (chapitre 2 : SGLD, SGHMC) et étude de simulation sur une loi de Student multivariée (chapitre 3) | Figures 3.1 à 3.7 (`Figures/Fig 1.png` … `Fig 7.png`) |
| `02_application_chapitre_4_adult.ipynb` | Régression logistique bayésienne sur le jeu de données Adult (chapitre 4) : MH de référence, recombinaison par lots, SGLD, SGHMC, divergences KL et temps de calcul | Figures 4.1 à 4.5 (`Figures/Fig_4_1.png` … `Fig_4_5.png`) |
| `Figures/` | Figures du mémoire, telles qu'obtenues en exécutant les notebooks | |

## Données

Le notebook du chapitre 4 télécharge automatiquement le jeu de données **Adult** (fichier `adult-all.csv`, 48 842 individus) depuis
<https://raw.githubusercontent.com/jbrownlee/Datasets/master/adult-all.csv>.
Source originale : UCI Machine Learning Repository, <https://archive.ics.uci.edu/dataset/2/adult>.

## Exécution

```bash
pip install -r requirements.txt
jupyter notebook
```

Ouvrir puis exécuter chaque notebook en entier (*Run All*). Les figures sont enregistrées dans le dossier `Figures/`.
Les méthodes étant stochastiques, une nouvelle exécution donne des valeurs numériques légèrement différentes de celles du mémoire, mais des conclusions identiques.
