# active-directory

Active Directory - Présentation et Analyse
Table des matières
Description
Documentation
Installation
Utilisation
Cas pratiques
Contact
Description
Active Directory est une solution de gestion des identités et des accès développée par Microsoft. Il permet d'organiser, sécuriser et administrer les ressources d'un réseau informatique de manière centralisée. Ce projet vise à fournir une analyse approfondie de son fonctionnement, de ses avantages et de ses limites.

Installation
Prérequis
Un serveur ou une machine compatible avec Active Directory (Windows Server requis)
Une image ISO de Windows Server avec les fonctionnalités AD DS (Active Directory Domain Services)
Accès Internet pour télécharger les mises à jour
Étapes d'installation
Étape 1 : Préparer l'environnement
Installer Windows Server sur le matériel ou une machine virtuelle
Configurer une adresse IP fixe
Renommer la machine pour correspondre aux conventions de nommage
Étape 2 : Installer le rôle Active Directory
Ouvrir le Gestionnaire de serveur
Ajoutez un rôle et sélectionnez "Services AD DS"
Suivre l'assistant d'installation et redémarrer la machine
Étape 3 : Promouvoir le serveur en contrôleur de domaine
Lancer l'outil "Configuration de l'Assistant Active Directory"
Sélectionnez "Ajouter une nouvelle forêt" ou rejoindre un domaine existant
Configurer les paramètres de domaine (nom, mot de passe DSRM, etc.)
Redémarrer pour finaliser l'installation
Utilisation
Active Directory permet : ✅ L'authentification et l'autorisation des utilisateurs ✅ La gestion centralisée des stratégies de groupe (GPO) ✅ Le contrôle d'accès aux ressources réseau ✅ L'intégration avec des services Cloud comme Azure AD

Cas pratiques
Exemple : Gestion des accès dans une entreprise
Un administrateur système utilise Active Directory pour :

Créer et gérer les comptes utilisateurs et groupes
Appliquer des stratégies de sécurité via GPO
Automatiser le déploiement d'applications via AD
Surveiller et auditer l'activité réseau
Résultat : Une infrastructure sécurisée et simplifiée pour la gestion des accès et des ressources.
