📖 English version available: [README_EN.md](README_EN.md)

# DOFConfigTool Auto-Update & Backup

## 📝 Description

Le script **DOFConfigTool Auto-Update & Backup** permet de gérer automatiquement et rapidement la mise à jour du fichier de configuration **DOFConfigTool**, utilisé pour le contrôle des LEDS et des TOYS dans les flippers virtuels.  
Il télécharge et remplace vos fichiers de configuration à partir de votre compte du site **DofConfigTool**, tout en effectuant une sauvegarde avant toute modification.

> *Script basé sur le DOF Configs Ini Pull Program (v4.0) du site [configtool.vpuniverse.com](https://configtool.vpuniverse.com).*

---

## Fonctionnalités

- **Téléchargement du fichier manquant**  
  Lors du premier lancement, le script vérifie si le fichier essentiel `_ledcontrol_pull.vbs_` est présent dans le répertoire.  
  ➜ S'il est manquant, il sera **téléchargé automatiquement** depuis le serveur.  

- **Sauvegarde et compression**  
  Avant toute mise à jour, le script effectue une **sauvegarde complète** du dossier `\CONFIG\` et le **compresse en archive ZIP**.  
  ➜ Un fichier de sauvegarde est créé pour **chaque mise à jour**.  

- **Mise à jour automatique**  
  Une fois la sauvegarde effectuée, le script met à jour automatiquement le fichier **DOFConfigTool**, en remplaçant l'ancienne version par la dernière version disponible.  

- **Gestion des sauvegardes du dossier Backup**  
  Vous pouvez désormais **configurer et gérer jusqu'à 5 sauvegardes maximum** *(ce chiffre est ajustable selon vos besoins)* pour le dossier `Backup`.  

- **Suppression automatique des anciennes sauvegardes**  
  ➜ Dès que le nombre de sauvegardes dépasse la limite configurée, **les plus anciennes sont automatiquement supprimées**.  

---

## Installation

1. **Téléchargez** le fichier `DofConfigTool-AutoUpdate.cmd` et placez-le **à la racine du dossier `DirectOutput`**.  
2. **Lancez-le** et **suivez les instructions affichées**.  
3. **Modifiez le fichier** dans un éditeur de texte et remplissez les champs suivants :  

   ```ini
   LCP_APIKEY=Votre clé API DOFConfigTool (exemple : F29oyY4loj3L53IUtF38xq613FA)
   LCP_DIRECTOUTPUTCONFIGPATH=Le chemin de votre dossier DOF (exemple : C:\DirectOutput\Config\)
4. **Enregistrez** le fichier après avoir ajouté les informations nécessaires.  
5. **Relancez** `DofConfigTool-AutoUpdate.cmd`.  

---

## Utilisation

1. **Exécutez** le script `DofConfigTool-AutoUpdate.cmd`.  
2. Lors du **premier lancement**, le script vérifie si le fichier `_ledcontrol_pull.vbs_` est présent dans le répertoire.  
   - S'il est **absent**, il sera téléchargé **automatiquement**.  
3. Une fois les **champs renseignés correctement**, **relancez le script** pour effectuer la mise à jour automatique.  
4. Le script effectue **une sauvegarde complète** de votre configuration **avant de procéder à la mise à jour** de **DOFConfigTool**.  

---

## Notes

- Le script nécessite **une connexion Internet** pour télécharger les fichiers nécessaires.  
- Assurez-vous que **le chemin de votre dossier de configuration DOF est correct** pour éviter toute erreur.  
- Si le script échoue à télécharger ou mettre à jour vos fichiers de configuration, **la mise à jour ne s’effectuera pas**.  
