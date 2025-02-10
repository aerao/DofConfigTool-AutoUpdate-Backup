Version française disponible ici : [README.md](README.md)

# DOFConfigTool Auto-Update & Backup

## Description

The **DOFConfigTool Auto-Update & Backup** script allows you to automatically and quickly manage the update of the **DOFConfigTool** configuration file, used for controlling LEDs and TOYS in virtual pinball machines.  
It downloads and replaces your configuration files from your **DofConfigTool** account while creating a backup before making any changes.

> *Script based on the DOF Configs Ini Pull Program (v4.0) from [configtool.vpuniverse.com](https://configtool.vpuniverse.com).*

---

## Features

- **Missing File Download**  
  When launched for the first time, the script checks if the essential `_ledcontrol_pull.vbs_` file is present in the directory.  
  ➜ If missing, it will be **automatically downloaded** from the server.  

- **Backup and Compression**  
  Before updating, the script creates a **full backup** of the `\CONFIG\` folder and **compresses it into a ZIP archive**.  
  ➜ A backup file is created for **each update**.  

- **Automatic Update**  
  Once the backup is completed, the script automatically updates the **DOFConfigTool** file, replacing the old version with the latest available version.  

- **Backup Folder Management**  
  You can now **configure and manage up to 5 backups** *(this number is adjustable based on your needs)* for the `Backup` folder.  

- **Automatic Deletion of Old Backups**  
  ➜ When the number of backups exceeds the configured limit, **the oldest backups are automatically deleted**.  

---

## Installation

1. **Download** the `DofConfigTool-AutoUpdate.cmd` file and place it **in the root of the `DirectOutput` folder**.  
2. **Run it** and **follow the on-screen instructions**.  
3. **Edit the file** in a text editor and fill in the following fields:  

   ```ini
   LCP_APIKEY=Your DOFConfigTool API key (example: F29oyY4loj3L53IUtF38xq613FA)
   LCP_DIRECTOUTPUTCONFIGPATH=Your DOF configuration folder path (example: C:\DirectOutput\Config\)
4. **Save** the file after adding the necessary information.  
5. **Restart** `DofConfigTool-AutoUpdate.cmd`.  

---

## Usage

1. **Run** the `DofConfigTool-AutoUpdate.cmd` script.  
2. During the **first launch**, the script checks if the `_ledcontrol_pull.vbs_` file is present in the directory.  
   - If **missing**, it will be **automatically downloaded**.  
3. Once the **fields are correctly filled**, **restart the script** to perform the automatic update.  
4. The script creates **a full backup** of your configuration **before proceeding with the update** of **DOFConfigTool**.  

---

## Notes

- The script requires **an internet connection** to download the necessary files.  
- Make sure **the path to your DOF configuration folder is correct** to avoid errors.  
- If the script fails to download or update your configuration files, **the update will not proceed**.  

