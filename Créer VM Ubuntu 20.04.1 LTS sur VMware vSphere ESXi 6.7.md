# **Créer VM Ubuntu 20.04.1 LTS sur VMware vSphere ESXi 6.7**

Cette documentation sert de support d'installation pour créer une VM d'Ubuntu Serveur sur un serveur ESXi via une console web (sans vCenter Server)



## Introduction

Installation testée sur un PC Dell Optiplex 7020 (Intel Core i5, 16Go RAM, 256Go SSD) avec VMware ESXi 6.7.0.update03 (DELL) 



## Ubuntu Server ISO

Télécharger l'ISO [Ubuntu Server 20.04.1 LTS](https://ubuntu.com/download/server), il sera par la suite intégré dans le stockage d'ESXi



## Intégrer l'ISO Ubuntu Server sur le stockage ESXi

Se connecter sur la console web d'ESXi

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_01_vmwareConsole.png)

Etendre **Stockage** puis cliquer sur **datastore**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_02_datastore.png)

Cliquer sur **Navigateur de banque de données**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_03_navigateurbdd.png)

1. Cliquer sur **Charger**
2. Sélectionner l'ISO téléchargé plus tôt
3. Cliquer sur **Ouvrir**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_04_explorateurWin.png)

Patienter durant l'intégration puis cliquer sur **Fermer**

L'ISO est maintenant intégré sur le stockage du serveur ESXi



## Création de la VM

Cliquer sur **Hôte** puis **Créer/Enregistrer une VM**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_06_creationVM1.png)

L'installeur s'ouvre

1. Cliquer sur **Créer une machine virtuelle**
2. Puis cliquer sur **Suivant**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_07_creationVM2.png)

1. Nommer la VM
2. Sélectionner **Linux** pour **Famille de systèmes d'exploitation invités**
3. Sélectionner **Ubuntu Linux (64-bit)** pour **Version du SE invité**
4. Puis cliquer sur **Suivant**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_08_creationVM3.png)

Sélectionner **datastore1**, c'est le disque sur lequel sera stocké la VM puis cliquer sur **Suivant**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_09_creationVM4.png)

Dans **Lecteur de CD/DVD 1**, sélectionner **Fichier ISO banque de données** puis cliquer sur **Parcourir**…

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_10_creationVM5.png)

Sélectionner l'ISO, puis cliquer  sur **Sélectionner**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_11_creationVM6.png)

Modifier les paramètres (CPU, Mémoire, Disque dur 1, etc.) puis cliquer sur **Suivant**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_12_creationVM7.png)

La VM est désormais prête, vérifier que les informations à l'écran sont correctes puis cliquer sur **Terminer**



## Installer le système d'exploitation

La VM étant prête, l'OS est prêt à être installé

1. Cliquer sur **Machines Virtuelles**
2. Cliquer sur le nom de la VM

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_13_installos.png)

Cliquer sur **Mettre sous tension**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_14_sousTension.png)

Cliquer sur **Console** puis **Ouvrir une console dans une nouvelle fenêtre**.

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_15_console.png)

L'installeur devrait apparaître dans un autre onglet 

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_16_installeur.png)

Suivre la [procédure d'installation]("https://github.com/Arkedrille/Infrastructure-Maison-Ark/Installer Ubuntu 20.04.1 Serveur LTS.md"). Une fois finie, on devra retirer l'ISO et installer VMware tools.



## Déconnecter l'ISO Ubuntu

Il faut déconnecter l'ISO Ubuntu pour éviter des erreurs en cas de future migration (par exemple)

Cliquer sur **Modifier** puis sélectionner **Périphérique hôte** sur **Lecteur de CD/DVD 1** puis cliquer sur **Enregistrer**

![](https://github.com/Arkedrille/Infrastructure-Maison-Ark/blob/master/assets/images-Cr%C3%A9er%20VM%20Ubuntu%2020.04.1%20LTS%20sur%20VMware%20vSphere%20ESXi%206.7/img_17_deconnecterISO.png)



## VMware tools

VMware devrait être installé sur Ubuntu 20.04.1 LTS. Si non, exécuter cette commande:

```
apt install open-vm-tools -y
```



**Ecrit par: [Tony Mackay](https://tonymackay.net/)**

**Traduit et mis à jour en pour Ubuntu 20.04.1 LTS par: [Karl Zawisla](https://github.com/Arkedrille/)**
