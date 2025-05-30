# 🧠 Active Directory - Présentation et Analyse

## 📚 Table des matières

- [Description](#description)
- [Installation](#installation)
  - [Prérequis](#prérequis)
  - [Étapes d'installation](#étapes-dinstallation)
- [Utilisation](#utilisation)
- [Cas pratiques](#cas-pratiques)
- [Contact](#contact)

---

## 📖 Description

**Active Directory** est une solution de gestion des identités et des accès développée par **Microsoft**.  
Elle permet d'organiser, sécuriser et administrer les ressources d'un réseau informatique de manière **centralisée**.

🎯 **Objectif du projet** : Fournir une analyse approfondie du fonctionnement d'Active Directory, de ses avantages et de ses limites.

---

## 💿 Installation

### 🔧 Prérequis

- Un serveur ou une machine compatible avec **Active Directory** (Windows Server requis)
- Une **image ISO** de Windows Server avec les fonctionnalités **AD DS (Active Directory Domain Services)**
- Accès Internet pour télécharger les mises à jour

### ⚙️ Étapes d'installation

#### ✅ Étape 1 : Préparer l'environnement

- Installer **Windows Server** sur le matériel ou une machine virtuelle
- Configurer une **adresse IP fixe**
- Renommer la machine selon les conventions de nommage

#### ✅ Étape 2 : Installer le rôle Active Directory

- Ouvrir le **Gestionnaire de serveur**
- Ajouter un rôle et sélectionner **"Services AD DS"**
- Suivre l'assistant d'installation
- **Redémarrer** la machine

#### ✅ Étape 3 : Promouvoir le serveur en contrôleur de domaine

- Lancer **l’Assistant de configuration d'Active Directory**
- Choisir :
  - "Ajouter une nouvelle forêt"  
  _ou_
  - Rejoindre un domaine existant
- Configurer :
  - Le **nom de domaine**
  - Le **mot de passe DSRM**
- **Redémarrer** pour finaliser l’installation

---

## 🛠️ Utilisation

Active Directory permet :

- ✅ L'**authentification** et l’**autorisation** des utilisateurs
- ✅ La **gestion centralisée** des stratégies de groupe (**GPO**)
- ✅ Le **contrôle d’accès** aux ressources réseau
- ✅ L’**intégration** avec des services Cloud comme **Azure AD**

---

## 💼 Cas pratiques

### 🎯 Exemple : Gestion des accès dans une entreprise

Un administrateur système utilise **Active Directory** pour :

- Créer et gérer des **comptes utilisateurs** et **groupes**
- Appliquer des **stratégies de sécurité** via **GPO**
- Automatiser le **déploiement d’applications**
- Surveiller et **auditer l’activité réseau**

✅ **Résultat** : Une **infrastructure sécurisée** et **simplifiée** pour la gestion des accès et des ressources.

---
