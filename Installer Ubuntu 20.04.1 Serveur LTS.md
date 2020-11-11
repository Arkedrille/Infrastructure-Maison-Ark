# Installer Ubuntu 20.04.1 Serveur LTS

Cette documentation vise à aider à l'installation pas à pas de Ubutnu 20.04.1 Serveur LTS sur une VM (ou support physique)



## Introduction

Cette procédure a été conçue pour compléter la procédure de [création de VM sous VMware ESXi](https://github.com/Arkedrille/Infrastructure-Maison-Ark/Créer VM Ubuntu 20.04.1 LTS sur VMware vSphere ESXi 6.7.md). 



## Ubuntu Server ISO

Télécharger l'ISO [Ubuntu Server 20.04.1 LTS](https://ubuntu.com/download/server)



## Clé bootable (hors VM)

Pour installer Ubuntu Serveur sur un poste physique il faudra utiliser une [clé bootable](https://github.com/Arkedrille/Documentations/Créer).



## Installeur

Une fois que l'OS a démarré, il faut paramétrer l'installeur comme suit :

Sélectionner **Français**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_01_installeur.png)

Mettre à jour l'installeur si demandé

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_02_installeur.png)

Modifier la disposition du clavier et variante et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_03_installeur.png)

Sélectionner  le nom du réseaux, préférer une connexion câblée plutôt qu'une connexion WiFi et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_04_installeur.png)

Un proxy peut être renseigné, ne rien remplir et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_05_installeur.png)

Laisser l'archive par défaut et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_06_installeur.png)

Ici, on utilise tout le disque, voir selon les besoins et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_07_installeur.png)

Vérifier si la configuration du stockage est correcte puis sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_08_installeur.png)

Valider l'installation sur le disque avec **Continuer**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_09_installeur.png)

Configuration de l'user

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_10_installeur.png)

Installer OpenSSH server pour pouvoir prendre la main à distance sur le poste via SSH (avec un logiciel comme putty - windows, linux et macOS)et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_11_installeur.png)

Installer (ou pas) des paquets et sélectionner/valider avec **Terminé**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_12_installeur.png)

Attendre la fin de l'installation et des mises à jour de sécurité 

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_13_installeur.png)

et finaliser l'installation en validant avec **Reboot**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Installer%20Ubuntu%2020.04.1%20Serveur%20LTS/img_14_installeur.png)

Ne pas oublier de retirer la clé bootable ou disque de démarrage quand l'installeur le demandera et au prochain reboot la distribution sera accessible