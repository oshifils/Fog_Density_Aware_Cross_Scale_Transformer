# Fog_Density_Aware_Cross_Scale_Transformer
# EDCST : Enhanced Density-Aware Cross-Scale Transformer for Robust Object Classification under Atmospheric Fog Conditions

Un projet de recherche avancé sur la classification robuste d’objets sous différentes intensités et types de brouillard, basé sur un modèle Transformer multi-échelle avec attention sensible à la densité.

## 🧠 Objectif

Développer un classificateur d'images performant capable de conserver une haute précision même dans des conditions visuelles dégradées par le brouillard.  
Le modèle s’appuie sur :
- Un mécanisme d’attention croisée entre les échelles
- Une stratégie d’optimisation basée sur OneCycleLR
- Cinq types de brouillard (uniforme, gradient, patchy, adaptatif, dense)

## 🚀 Fonctionnalités principales

- Simulations réalistes de brouillard sur CIFAR-10
- Architecture personnalisée à base de Vision Transformers
- Analyse de robustesse par classe (class-wise sensitivity)
- Visualisation des résultats de classification

## 📦 Technologies utilisées

- Python 3.10
- PyTorch
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV
- Jupyter Notebook

## 📁 Structure du projet

```
.
├── Fog_Density_Aware_Cross_Scale_Transformer_5Types_Fog_Optimizing.ipynb
├── data/
│   └── (CIFAR-10 images simulées avec brouillard)
├── models/
│   └── transformer_fdacst.py
├── utils/
│   └── fog_simulation.py
├── requirements.txt
└── README.md
```

## ⚙️ Installation

1. Cloner le dépôt :
```bash
git clone https://github.com/oshifils/Fog_Density_Aware_Cross_Scale_Transformer.git
cd Fog_Density_Aware_Cross_Scale_Transformer
```

2. Créer un environnement virtuel (optionnel mais recommandé) :
```bash
python -m venv venv
source venv/bin/activate  # sous Linux/macOS
venv\Scripts\activate     # sous Windows
```

3. Installer les dépendances :
```bash
pip install -r requirements.txt
```

## 🧪 Lancer le Notebook

Ouvre le notebook dans Jupyter :
```bash
jupyter notebook Fog_Density_Aware_Cross_Scale_Transformer_5Types_Fog_Optimizing.ipynb
```

> ⚠️ Assurez-vous que les images CIFAR-10 modifiées avec brouillard sont bien placées dans `./data`.

## 📊 Résultats obtenus

| Condition             | Accuracy (%) |
|-----------------------|--------------|
| Sans brouillard       | 84.4         |
| Brouillard léger      | 81.3         |
| Brouillard moyen      | 77.5         |
| Brouillard dense      | 74.2         |
| Brouillard extrême    | 70.1         |

- **Robustesse élevée** pour les véhicules et animaux
- **Amélioration de 15.8%** par rapport aux Transformers standards

## 📌 À venir

- Évaluation sur des jeux de données réels (Dashcam, Foggy Cityscapes)
- Extension vers la segmentation sémantique
- Intégration de détection d’anomalies

## 👤 Auteur

- **OSHASHA OSHASHA Fiston**  
Chercheur en intelligence artificielle appliquée et Système distribué  
GitHub : [@oshifils](https://github.com/oshifils)

## 📄 Licence

Ce projet est publié sous licence **MIT**.  
Vous pouvez l'utiliser, le modifier et le redistribuer librement avec attribution.
