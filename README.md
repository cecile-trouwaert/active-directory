Active Directory - Gestion pour l'association "Pour les vieux"
Implémentation complète d'AD avec PowerShell, GPO et réplication

# 🏥 Active Directory - Association "Pour les vieux"  

Ce projet démontre la mise en place d'un annuaire Active Directory pour une association gérant 4 établissements médico-sociaux.  

## 🎯 Objectifs  
- Centraliser la gestion des identités (200+ utilisateurs).  
- Appliquer des permissions granulaires (médical, compta, technique).  
- Automatiser via PowerShell et GPO.  

## 🔧 Technologies  
- **Windows Server 2025** (VM)  
- **PowerShell 7+**  
- **GPO** (Stratégies de Groupe)  
- **LDAP** / **Kerberos**  

## 🚀 Déploiement  
1. **Installer AD** :  
   ```powershell
   .\scripts\01_Installation_AD.ps1 -DomainName "pourlesvieux.local"  
Importer les utilisateurs :

powershell
.\scripts\02_Creation_Utilisateurs.ps1 -CsvPath ".\docs\utilisateurs.csv"  
Appliquer les GPO :

powershell
.\scripts\03_GPO_Lecteurs.ps1  
📊 Monitoring (Exemple)
Alerte mots de passe

📚 Documentation
Matrice des permissions

Présentation AD

💡 Bonnes Pratiques
Mots de passe : Forcer le changement au 1er login (Azerty06! par défaut).

Audit : Scripts PowerShell pour détecter les anomalies.

Haute disponibilité : 2 contrôleurs de domaine avec réplication.

👨‍💻 Contributions : Les PR sont les bienvenues !
📜 Licence : MIT - Libre d'utilisation et modification.


---

## 🔗 **Fichiers clés à fournir**  
1. **Scripts PowerShell** :  
   - Exemple pour `01_Installation_AD.ps1` :  
     ```powershell
     # Installer le rôle AD
     Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
     # Promouvoir en contrôleur de domaine
     Install-ADDSForest -DomainName "pourlesvieux.local" -InstallDns:$true -Force:$true
     ```  

2. **Matrice des permissions** (Excel) :  
   - Colonnes : `Dossier | Groupe | Permission | Département`.  

3. **Documentation PDF** :  
   - Résume les sections I à IV de votre demande originale.  

---

## ✅ Validation  
- **Tests** :  
  - Vérifier la réplication entre les 2 DCs avec `repadmin /showrepl`.  
  - Tester les accès aux dossiers partagés (ex : `\\serveur\medical`).   

---

### 🌟 Pourquoi ce projet ?  
- **Professionnel** : Montre votre maîtrise d'AD, PowerShell, et la gestion de projets IT complexes.  
- **Open Source** : Peut être réutilisé par d'autres associations.  


