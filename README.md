# Segmentation d'Images - Deep Learning

Ce projet explore différentes techniques de segmentation d'images en utilisant l'apprentissage profond, notamment avec les architectures U-Net et knowledge distillation.

## 📁 Structure du Projet

```
Deep Learning/
├── PROJET/                          # Projet principal de segmentation
│   ├── notebooks/
│   │   └── camvid_unet_selfdistill.ipynb
│   ├── data/camvid/                # Dataset CamVid
│   │   ├── images/
│   │   └── masks/
│   ├── outputs/
│   │   ├── checkpoints/            # Modèles entraînés
│   │   ├── figures/                # Visualisations
│   │   ├── metrics/                # Métriques d'évaluation
│   │   └── predictions/            # Prédictions du modèle
│   └── requirements.txt
│
├── TP1/                             # Travail pratique 1 - Préparation de données
├── TP2/                             # Travail pratique 2 - Classification
├── TP3/                             # Travail pratique 3
├── TP4/                             # Travail pratique 4 - Détection YOLOv8
│
└── README.md
```

## 🎯 Objectifs

- **Segmentation d'images sémantique** sur le dataset CamVid
- **U-Net baseline** pour la segmentation
- **Knowledge Distillation** pour l'optimisation du modèle
- **Classification binaire et multiclass** sur des données médicales
- **Détection d'objets** avec YOLOv8

## 🚀 Démarrage Rapide

### Prérequis

- Python 3.8+
- GPU recommandé (CUDA)

### Installation

```bash
# Cloner le repository
git clone https://github.com/JadFalaq/Segmentation_Image.git
cd Deep\ Learning

# Créer un environnement virtuel
python -m venv .venv
source .venv/bin/activate  # On Linux/Mac
# ou
.venv\Scripts\activate  # On Windows

# Installer les dépendances
pip install -r PROJET/requirements.txt
```

## 📊 Modèles et Résultats

### PROJET - Segmentation CamVid

#### Checkpoints disponibles:
- `best_unet_baseline.pth` - U-Net baseline
- `best_unet_self_distill.pth` - U-Net avec self-distillation
- `best_unet_self_distill_fixed.pth` - Version corrigée

#### Métriques:
- Voir `outputs/metrics/` pour les résultats complets
- Comparaison: `baseline_vs_self_distill.csv`

## 📈 Travaux Pratiques

### TP1 - Préparation de Données
- Nettoyage et prétraitement des données
- Énumération des cibles
- Gestion des valeurs manquantes

### TP2 - Classification
- Classification binaire (Anomalies bancaires, Maladies)
- Régression (Consommation énergétique)

### TP3-TP4
- Travaux pratiques supplémentaires
- Détection avec YOLOv8 sur radiographies thoraciques

## 🛠️ Technologies Utilisées

- **Framework**: PyTorch
- **Segmentation**: UNet, Self-Distillation
- **Détection**: YOLOv8
- **Traitement**: OpenCV, Pillow
- **Analyse**: Pandas, NumPy, Scikit-learn
- **Visualisation**: Matplotlib, Seaborn

## 📝 Utilisation

Consultez les notebooks Jupyter pour des exemples d'utilisation :
- `PROJET/notebooks/camvid_unet_selfdistill.ipynb`
- `TP1/tp1_notebook.ipynb`
- `TP2/*/multiclass.ipynb`
- `TP4/notebook.ipynb`

## 📄 Licence

Projet personnel - Université

## ✍️ Auteur

**Jad Falaq**
