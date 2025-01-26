### DOFConfigTool Auto-Update & Backup

**Description**
Le script DOFConfigTool Auto-Update & Backup permet de gérer automatiquement la mise à jour du fichier de configuration **DOFConfigTool** utilisé pour le contrôle des LEDS et des TOYS dans les flippers virtuels. Il télécharge et remplace vos fichiers de configuration à partir de votre compte du site DofConfigTool, tout en effectuant une sauvegarde avant toute modification.

**Fonctionnalités**
 - **Téléchargement du fichier manquant** : Lors du premier lancement, le script vérifie si le fichier essentiel _ledcontrol_pull.vbs_ est présent dans le répertoire. Si ce fichier est manquant, il sera téléchargé automatiquement depuis le serveur.
 - **Sauvegarde et compression** : Avant toute mise à jour, le script effectue une sauvegarde complète du dossier \CONFIG\ et le compresse en archive ZIP. Un fichier de sauvegarde est créé pour chaque mise à jour.
 - **Mise à jour automatique** : Une fois la sauvegarde effectuée, le script met à jour automatiquement le fichier DOFConfigTool, en remplaçant l'ancienne version par la dernière version disponible.

**Installation**
1. Téléchargez le fichier DofConfigTool-AutoUpdate.cmd et mettez le à la racine du dossier DirectOutput
2. Ouvrez le fichier dans un éditeur de texte et remplissez les champs suivants :
 -  LCP_APIKEY : Votre clé API DOFConfigTool.  (exemple, F29oyY4loj3L53IUtF38xq613FA ).
 -  LCP_DIRECTOUTPUTCONFIGPATH : Le chemin de votre dossier de configuration DOF (exemple, C:\DirectOutput\Config\).
3. Enregistrez le fichier après avoir ajouté les informations nécessaires.

**Utilisation**
1.  Exécutez le script DofConfigTool-AutoUpdate.cmd.
2.  Lors du premier lancement, le script vérifie si le fichier ledcontrol_pull.vbs est présent dans le répertoire du script. Si ce fichier est manquant, il sera téléchargé automatiquement.
3.  Une fois les champs renseignés correctement dans le fichier, relancez le script pour effectuer la mise à jour automatique.
4.  Le script effectue une sauvegarde complète de votre configuration avant de procéder à la mise à jour de **DOFConfigTool**.

**Notes**
- Le script nécessite une connexion Internet pour télécharger les fichiers nécessaires.
- Veuillez vous assurer que le chemin de votre dossier de configuration DOF est correct pour éviter toute erreur.
- Si le script échoue à télécharger ou mettre à jour un fichier, la mise à jour ne s'effectuera pas.
