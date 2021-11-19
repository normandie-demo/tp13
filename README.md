# TP numéro 13

## Objectif:

Stocker un secret dans un fichier Ansible Vault

## Besoin:

- Créer un fichier vault *mysql.yaml* contenant les mots de passe root *old_pass* et *new_pass*
- Créer un Playbook *rotate.yaml* tel que:
  - S’exécute sur les hosts *back*
  - Charge le contenu *mysql.yaml*
  - Exécute le changement du password root mariadb en assurant de ne pas logguer la commande 
  - Exécuter le Playbook en mode Verbose en demandant le mot de passe du fichier Vault


> La commande pour initialiser le mot de passe root est: `/usr/bin/mysqladmin -u root password '<mot de passe>'`
