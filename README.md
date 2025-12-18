# Backoffice Web App

## Description

Cette application est un **Backoffice simple** pour gérer les entités scolaires (Étudiants, Enseignants, Cours, Salles, Notes/Examens) via un tableau de bord interactif et un système de login sécurisé avec redirection vers le dashboard.

L'application est développée uniquement en **HTML5**, **CSS3** et **JavaScript natif**, sans frameworks externes.

---

## Structure du projet

- `index.html` - Page de connexion (Login)
- `dashboard.html` - Tableau de bord (Dashboard)
- `README.md` - Documentation du projet

---

## Login Page

### Fonctionnalités

- Formulaire avec nom d'utilisateur et mot de passe
- Vérification côté client : seul l'utilisateur `admin / admin` est accepté
- Redirection vers le dashboard en cas de succès
- Message d'alerte en cas d'identifiants incorrects

### Design

- Carte centrée sur l'écran
- Gradient en background
- Inputs arrondis avec effet focus
- Bouton de connexion avec animation au survol

---

## Dashboard

### Fonctionnalités principales

#### Dashboard (Accueil)

- Affichage de cartes statistiques : nombre d'étudiants, enseignants, cours, salles

#### Gestion des entités

- **Étudiants** : liste avec ID, nom, prénom, classe, bouton "Voir"
- **Enseignants** : liste avec ID, nom, prénom, matière, bouton "Voir"
- **Cours** : liste des cours avec ID, intitulé, matière, enseignant, classe
- **Salles** : liste des salles avec ID, nom et capacité
- **Notes / Examens** : section pour la gestion future

#### Détails

- Affichage d'un rapport détaillé pour chaque entité sélectionnée

#### Déconnexion

- Bouton pour terminer la session et revenir à la page de login

### Design

- Sidebar fixe avec menu de navigation
- Contenu responsive
- Cartes statistiques avec ombre et arrondi
- Tables stylisées avec couleur et boutons interactifs

---

## Fonctionnement

1. Ouvrir la page de login dans un navigateur
2. Saisir le login :
   - **Nom d'utilisateur** : `admin`
   - **Mot de passe** : `admin`
3. Cliquer sur **Login** → redirection vers le dashboard
4. Naviguer entre les sections via le menu à gauche
5. Cliquer sur **Déconnexion** pour retourner à la page de login

