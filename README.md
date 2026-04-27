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

![tp5](content/other/tp5-tuto.gif)

Tout d'abord pour publier ce répertoire sur GitHub Pages, suivez ces étapes :

1. **Forker le répertoire**
   - Cliquez sur **Fork** en haut à droite pour créer votre propre copie sur votre compte GitHub.

2. **Activer les workflows**
   - Allez dans l’onglet **Actions** de votre répertoire forké.
   - Cliquez sur **"I understand my workflows, go ahead and enable them"** pour activer les workflows.

3. **Activer GitHub Pages**
   - Ouvrez les **Paramètres** (`Settings`) de votre répertoire forké.
   - Dans la section **Pages**, sélectionnez **GitHub Actions** comme source de déploiement.

4. **Publier et vérifier le site**
   - Effectuez une modification et **commit** dans le répertoire.
   - Le workflow GitHub Actions générera et publiera automatiquement le site.
   - L’URL du site sera indiquée dans la section **Pages** des paramètres.

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
