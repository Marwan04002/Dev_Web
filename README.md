# Backoffice Web App

## Description

Cette application est un **Backoffice simple** (front-end uniquement) pour gérer des entités scolaires : Étudiants, Enseignants, Modules, Cours, Groupes et Notes. Elle fonctionne entièrement avec **HTML5**, **CSS3** et **JavaScript natif** et stocke les données côté client dans `localStorage`.

---

## Arborescence & Fichiers

- `index.html` - Page de **connexion** (Login)
  - Formulaire simple (utilisateur `admin` / mot de passe `admin`) validé côté client.
  - En cas de succès, redirection vers `dashboard.html`.

- `dashboard.html` - **Tableau de bord** principal
  - Interface avec une **sidebar** de navigation et des sections pour chaque entité.
  - Gestion CRUD basique : **Ajouter**, **Éditer**, **Supprimer** pour chaque entité.
  - Données persistées dans `localStorage` sous la clé `schoolDB`.
  - Entités gérées et champs (exemples) :
    - `students` : `id, nom, prenom, groupe, birth, mat`
    - `teachers` : `id, nom, prenom, mat`
    - `modules` : `id, name, prof`
    - `courses` : `id, titre, prof, module`
    - `groups` : `id, name, capacity`
    - `grades` : `id, groupe, etudiant, note`

- `README.md` - Documentation (ce fichier)

> Remarque : Le projet est volontairement minimal et ne contient pas de back-end. Ouvrir `index.html` dans un navigateur suffit pour l'utiliser.

---

## Fonctionnalités détaillées

- Authentification :
  - Contrôle simple côté client pour la démo (`admin/admin`).

- Dashboard & Navigation :
  - Sidebar fixe pour accéder aux sections : Étudiants, Professeurs, Modules, Cours, Groupes, Notes.
  - Vue table listant les enregistrements pour chaque entité avec actions `Edit` / `Delete`.

- Formulaires :
  - Formulaire d'ajout et d'édition réutilisable.
  - Sélections dépendantes (ex. sélectionner un groupe filtre les étudiants pour les notes).

- Stockage :
  - Toutes les données sont stockées dans `localStorage` sous la clé `schoolDB` au format JSON.
  - Utilisez l'inspecteur du navigateur pour visualiser ou supprimer la clé si besoin (réinitialiser les données).

---

## Utilisation

1. Ouvrir `index.html` dans un navigateur moderne.
2. Se connecter avec : `admin` / `admin`.
3. Ajouter, éditer ou supprimer des enregistrements via le dashboard.
4. Les changements sont automatiquement sauvegardés dans `localStorage`.

---

## Pour aller plus loin

- Ajouter une API back-end pour persister les données côté serveur (ex : Node.js + Express).
- Valider et filtrer les champs côté client (ex : validation de note, capacité numérique positive).
- Ajouter recherches, filtres et pagination pour les tables.
- Export / import JSON pour sauvegarder ou restaurer des jeux de données.

---

## Licence & Crédit

Projet d'exemple éducatif - code libre d'usage pour apprentissage.

---

Si tu veux, je peux :
- ajouter des exemples de données de démo au chargement,
- documenter le format exact attendu dans `localStorage`,
- ou générer un petit script pour réinitialiser la BDD locale.

Indique ce que tu souhaites que j'ajoute ensuite.

