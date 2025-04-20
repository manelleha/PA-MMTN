# 📁 data/

Ce dossier contient les données issues du dataset **Dental Annotation** disponible sur [Roboflow](https://universe.roboflow.com/dent-dataset/dental-annotation).

## 📥 Téléchargement

Lien direct :  
👉 [Dental Annotation – Roboflow](https://universe.roboflow.com/dent-dataset/dental-annotation)

Téléchargez le dataset dans un format comme **YOLOv8** ou **COCO JSON**, puis organisez-le comme ci-dessous.

## 📂 Organisation recommandée

```
data/
├── train/
│   ├── images/
│   └── labels/
├── valid/
│   ├── images/
│   └── labels/
├── test/
│   ├── images/
│   └── labels/
├── data.yaml
```

## 🏷️ Classes présentes dans le dataset

Ce dataset contient les 9 classes suivantes :

1. **Abcess** : abcès dentaire
2. **Badly Decayed** : dent très détériorée
3. **Caries** : carie dentaire
4. **Crown** : couronne dentaire
5. **Normal** : dent considérée comme saine
6. **Overhang** : débordement (ex. amalgame mal placé)
7. **Post** : tenon ou pivot radiculaire
8. **RCT** : traitement endodontique (Root Canal Therapy)
9. **Restoration** : restauration dentaire (composite, amalgame…)

Les annotations sont prêtes à l’emploi et disponibles dans les sous-dossiers `labels/`.

## 🧪 Pré-traitement appliqué à chaque image

- Orientation automatique des pixels (avec suppression EXIF)
- Redimensionnement à **640x640 (stretch)**
- Conversion en niveaux de gris (**Grayscale CRT phosphor**)

---

## 🔁 Augmentations de données utilisées

Chaque image source a été augmentée 3 fois avec les transformations suivantes :

- 50% de chance de **flip horizontal**
- 50% de chance de **flip vertical**
- Rotation aléatoire de 90° (aucune / sens horaire / anti-horaire)
- Rotation aléatoire entre **-15° et +15°**


## 📌 Informations complémentaires

- Le fichier `data.yaml` contient les chemins vers les dossiers et la liste des classes.
- Aucun étiquetage manuel supplémentaire n’est nécessaire.

## ⚠️ Remarque

Ce dossier est **exclu du versionnement Git** via `.gitignore`, car il peut contenir de nombreux fichiers volumineux.
