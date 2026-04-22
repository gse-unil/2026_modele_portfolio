# Modèle de Portfolio

Ce repértoire fournit un modèle de portfolio prêt à l’emploi pour les étudiant·e·s.

L’objectif est simple : vous permettre de créer rapidement un portfolio propre, structuré et personnalisable, sans connaissances avancées en programmation.

## Structure du projet
Voici l’organisation du modèle :
```
├── content
│   ├── apropos.md
│   ├── portfolio.md
│   ├── project.ipynb
│   └── img
│      └── ma_photo.png
```

## Par où commencer ?

### 1. Modifier votre profil

* Fichier : `content/apropos.md`
* C’est la page principale de présentation.

### 2. Ajouter votre photo (optionnel)

* Dossier : `content/img/`
* Remplacez `ma_photo.png` par votre image
* Assurez-vous que le nom correspond!

### 3. Construire votre portfolio

* Fichier : `content/portfolio.md`
* À utiliser les éléments vus lors de la séance de réflexion.

### 4. Ajouter un projet

* Fichier : `content/mon_projet.ipynb`

### [Optionnel] Table des matières du site (MyST / Jupyter Book)

C’est ici que vous contrôlez la navigation globale du site.
* Le fichier important est : `myst.yml`
* Structure de base:
```
toc:
    - file: content/apropos.md
    - file: content/portfolio.md
    - file: content/mon_projet.ipynb
```

* Ajouter une page
  * Si vous créez un fichier :`content/mon_projet.ipynb`
* Ajoutez-le dans myst.yml :

```
toc:
    - file: content/apropos.md
    - file: content/portfolio.md
    - file: content/mon_projet.ipynb
    - file: content/mon_projet_2.ipynb
```
