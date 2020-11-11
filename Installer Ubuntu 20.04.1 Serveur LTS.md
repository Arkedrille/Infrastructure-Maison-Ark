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

![image-20201111131551871](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131551871.png)

Mettre à jour l'installeur si demandé

![image-20201111131620152](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131620152.png)

Modifier la disposition du clavier et variante et sélectionner/valider avec **Terminé**

![image-20201111131715509](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131715509.png)

Sélectionner  le nom du réseaux, préférer une connexion câblée plutôt qu'une connexion WiFi et sélectionner/valider avec **Terminé**

![image-20201111131756067](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131756067.png)

Un proxy peut être renseigné, ne rien remplir et sélectionner/valider avec **Terminé**

![image-20201111131815465](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131815465.png)

Laisser l'archive par défaut et sélectionner/valider avec **Terminé**

![image-20201111131834366](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131834366.png)

Ici, on utilise tout le disque, voir selon les besoins et sélectionner/valider avec **Terminé**

![image-20201111131900731](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131900731.png)

Vérifier si la configuration du stockage est correcte puis sélectionner/valider avec **Terminé**

![image-20201111131917436](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131917436.png)

Valider l'installation sur le disque avec **Continuer**

![image-20201111131934133](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131934133.png)

Configuration de l'user

![image-20201111131950779](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111131950779.png)

Installer OpenSSH server pour pouvoir prendre la main à distance sur le poste via SSH (avec un logiciel comme putty - windows, linux et macOS)et sélectionner/valider avec **Terminé**

![image-20201111132440542](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111132440542.png)

Installer (ou pas) des paquets et sélectionner/valider avec **Terminé**

![image-20201111132510785](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111132510785.png)

Attendre la fin de l'installation et des mises à jour de sécurité 

![image-20201111132536067](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111132536067.png)

et finaliser l'installation en validant avec **Reboot**

![image-20201111135934984](C:\Users\Arkedrille\AppData\Roaming\Typora\typora-user-images\image-20201111135934984.png)

Ne pas oublier de retirer la clé bootable ou disque de démarrage quand l'installeur le demandera et au prochain reboot la distribution sera accessible