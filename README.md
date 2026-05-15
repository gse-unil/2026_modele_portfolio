# [Modèle de Portfolio](https://github.com/gse-unil/2026_modele_portfolio)

Ce [repértoire](https://github.com/gse-unil/2026_modele_portfolio) fournit un modèle de portfolio prêt à l’emploi pour les étudiant·e·s.

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

## I. Configurer le portfolio

On va faire la configuration sur GitHub pages, mais si vous préférez ne pas avoir un répertoire GitHub public, vous pouvez directement passer à la section [Optionnel : utiliser GitLab pour un portfolio plus privé](#optionnel--utiliser-gitlab-pour-un-portfolio-plus-privé).

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

## II. Renseigner les données

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

## Optionnel : utiliser GitLab pour un portfolio plus privé

Si vous préférez ne pas avoir un répertoire GitHub public, vous pouvez dupliquer le modèle de portfolio sur GitLab et restreindre l’accès au répertoire ainsi qu’au site web aux seules personnes invitées.

### 1. Créer un compte GitLab

Créer un compte sur : <https://gitlab.com>

### 2. Dupliquer le modèle de portfolio sur GitLab

1. Dans GitLab, cliquer sur **New project**
2. Sélectionner **Import project**
3. Choisir **Repository by URL**
4. Coller l’URL du répertoire : `https://github.com/gse-unil/2026_modele_portfolio.git`
5. Choisir un nom de projet (par exemple : `portfolio`)
6. Définir la visibilité du répertoire sur : `Private`
7. Cliquer sur **Create project**

### 3. Restreindre l’accès au site web

Pour que seules les personnes autorisées puissent accéder au portfolio :

1. Aller dans **Settings → General**
2. Ouvrir **Visibility, project features, permissions**
3. Vérifier que la visibilité du projet est définie sur : `Private`
4. Dans la section **Pages**, choisir : `Only project members`

### 4. Ajouter les enseignant·e·s au projet

Pour permettre aux enseignant·e·s d’accéder au portfolio :

1. Aller dans **Manage → Members**
2. Cliquer sur **Invite members**
3. Ajouter les identifiants GitLab ou adresses email fournis par les enseignant·e·s
4. Attribuer le rôle : `Reporter`

### 5. Continuer ensuite comme indiqué dans [II. Renseigner les données](#ii.-renseigner-les-données)
