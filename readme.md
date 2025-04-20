# 🦷 Dental AI – Triage Automatique des Radios Dentaires

Ce projet a pour but de créer une **application web alimentée par l'intelligence artificielle** afin d'aider les dentistes à **prioriser les cas urgents** à partir d'images de **radios dentaires**.

---

## 🎯 Objectif

L’application permet de :
- Charger une radio dentaire.
- Prédire automatiquement un **niveau de priorité** (ex : urgent, moyen, faible).
- Aider les professionnels de santé à prendre des décisions rapides et éclairées.

---

## 📁 Structure du projet

```
DENTAL_AI/
├── app/              # Code de l'application web
├── data/             # Données organisées en sous-dossiers
│   ├── train/        # Données d'entraînement
│   ├── validation/   # Données de validation
│   ├── test/         # Données de test
│   └── readme.md     # Explications sur les données
├── models/           # Scripts d'entraînement et architecture des modèles
├── saved/            # Modèles sauvegardés (.pt, .pkl, etc.)
├── requirements.txt  # Bibliothèques Python nécessaires
├── .gitignore        # Fichiers à ignorer dans Git
└── README.md         # Ce fichier 📄
```

---

## 🧠 Dataset

📥 Téléchargement :  
[👉 Lien Google Drive](https://drive.google.com/file/d/10cc7snHCYSq0aN8n8AaGAKvpvy2_JcW6/view)

📂 Organisation des données :
```
data/
├── train/
├── validation/
└── test/
```

Les images doivent être placées dans les dossiers correspondants.  
Si vous avez des fichiers CSV avec les labels, ajoutez-les aussi dans `data/`.

---

## 🛠️ Technologies utilisées

- **Python 3.8+**
- **PyTorch** (ou TensorFlow)
- **OpenCV**
- **Streamlit** (ou Flask) pour l'application web
- **scikit-learn**
- **pandas / numpy / matplotlib**

---

## ⚙️ Installation

1. Clonez le repo :
```bash
git clone https://github.com/manelleha/PA-MMTN.git
cd dental_ai
```

2. Installez les dépendances :
```bash
pip install -r requirements.txt
```

---

## 🚀 Lancer l’application (si Streamlit)

```bash
streamlit run app/app.py
```

L'application s'ouvrira dans votre navigateur à l'adresse :  
[http://localhost:8501](http://localhost:8501)

---

## 🧪 Exemple à venir

- Exemple d’image de radio
- Exemple de prédiction du modèle
- Résultat affiché dans l'application

---

## 🤝 Équipe

- Manelle  
- Noussayba
- Tinhinane
- Monsef

---


