📖 English version available: [README.md](README.md)

# DOFConfigTool Mise à jour automatique et sauvegarde

## Description

Le script **DOFConfigTool Mise à jour automatique et sauvegarde** vous permet de gérer automatiquement et rapidement la mise à jour du fichier de configuration de **DOFConfigTool**, utilisé pour contrôler les LED et les jouets dans les machines de flipper virtuel.  
Il télécharge et remplace vos fichiers de configuration depuis votre compte **DofConfigTool** tout en créant une sauvegarde avant de procéder à toute modification.

> *Script basé sur le programme DOF Configs Ini Pull (v4.0) de [configtool.vpuniverse.com](https://configtool.vpuniverse.com).*

---

## Fonctionnalités

- **Téléchargement du fichier manquant**  
  Lors du premier lancement, le script vérifie si le fichier essentiel `_ledcontrol_pull.vbs_` est présent dans le répertoire.  
  ➜ S'il manque, il sera **téléchargé automatiquement** depuis le serveur.

- **Sauvegarde et compression**  
  Avant la mise à jour, le script crée une **sauvegarde complète** du dossier `\CONFIG\` et **le compresse dans une archive ZIP**.  
  ➜ Un fichier de sauvegarde est créé **à chaque mise à jour**.

- **Mise à jour automatique**  
  Une fois la sauvegarde terminée, le script met automatiquement à jour le fichier **DOFConfigTool**, en remplaçant l'ancienne version par la dernière version disponible.

- **Gestion du dossier de sauvegarde**  
  Vous pouvez désormais **configurer et gérer jusqu'à 5 sauvegardes** *(ce nombre est ajustable selon vos besoins)* pour le dossier `Backup`.

- **Suppression automatique des anciennes sauvegardes**  
  ➜ Lorsque le nombre de sauvegardes dépasse la limite configurée, **les sauvegardes les plus anciennes sont automatiquement supprimées**.

---

## Installation

1. **Téléchargez** le fichier `DofConfigTool-AutoUpdate.cmd` et placez-le **à la racine du dossier `DirectOutput`**.
2. **Exécutez-le** et **suivez les instructions à l'écran**.
3. **Modifiez** le fichier dans un éditeur de texte et remplissez les champs suivants :

   Dans le fichier `DofConfigTool-AutoUpdate.cmd`, vous trouverez des espaces réservés pour les champs requis. Remplacez-les par vos données réelles.

---

## Exemple

**Avant :**

~~~ini
SET LCP_APIKEY=###
SET LCP_DIRECTOUTPUTCONFIGPATH=###
~~~

**Après :**

~~~ini
SET LCP_APIKEY=8JIx1LBoDR5Z64mv3zKqI8YJW3BOoLuD
SET LCP_DIRECTOUTPUTCONFIGPATH=C:\DirectOutput\Config\
~~~

4. **Enregistrez** le fichier après avoir ajouté les informations nécessaires.
5. **Redémarrez** `DofConfigTool-AutoUpdate.cmd`.

---

## Utilisation

1. **Exécutez** le script `DofConfigTool-AutoUpdate.cmd`.
2. Lors du **premier lancement**, le script vérifie si le fichier `_ledcontrol_pull.vbs_` est présent dans le répertoire.  
   - S'il manque, il sera **téléchargé automatiquement**.
3. Une fois que les **champs sont correctement remplis**, **redémarrez le script** pour effectuer la mise à jour automatique.
4. Le script crée **une sauvegarde complète** de votre configuration **avant de procéder à la mise à jour** de **DOFConfigTool**.

---

## Remarques

- Le script nécessite **une connexion Internet** pour télécharger les fichiers nécessaires.
- Assurez-vous que **le chemin vers votre dossier de configuration DOF est correct** afin d'éviter des erreurs.
- Si le script échoue à télécharger ou à mettre à jour vos fichiers de configuration, **la mise à jour ne sera pas effectuée**.
