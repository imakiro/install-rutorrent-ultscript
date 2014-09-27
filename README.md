# Rtorrent/rutorrent/munin/seedbox-manager install script
# Original script from exrat => https://bitbucket.org/exrat/install-rutorrent
# I (imakiro) translated it and extended it, this is a WIP version, please do know what you do if you use it.

## French first, English goes next [here][english]


# Script d'installation ruTorrent / Nginx v 1.3

* Nécessite Debian 7.x - 32/64 bits & un serveur fraîchement installé
* Multi-utilisateurs

* Inclus VsFTPd (ftp & ftps sur le port 21), Fail2ban (avec conf nginx, ftp & ssh) & Proxy php
* Seedbox-Manager, Auteurs: Magicalex, Hydrog3n et Backtoback

Tiré du tutoriel de Magicalex pour mondedie.fr disponible ici:

[Installer ruTorrent sur Debian {nginx & php-fpm}](http://mondedie.fr/viewtopic.php?id=5302)

[Aide, support & plus si affinités à la même adresse !](http://mondedie.fr/)

**Auteur :** Ex_Rat

Merci Aliochka & Meister pour les conf de munin et VsFTPd

à Albaret pour le coup de main sur la gestion d'users et

Jedediah pour avoir joué avec le html/css du thème

## Installation:
```
apt-get update && apt-get upgrade -y
apt-get install git-core -y

cd /tmp
git clone https://bitbucket.org/exrat/install-rutorrent
cd install-rutorrent
chmod a+x scriptmondediefr.sh && ./scriptmondediefr.sh
```

Pour gérer vos utilisateurs ultérieurement, il vous suffit de relancer le script

#### Inspiration:
- [hexodark](https://github.com/gaaara/)


## (english) English version:

# Install script for ruTorrent on Nginx v 1.3
* Multi-User capable
* Needs a clean new install of Debian 7 wheezy (be it 64 or 32 bits)
* FTP powered by VsFTPD (with FTP and FTPS on port 21)
* Fail2ban configured on nginx, FTP and ssh.
* Php proxy to access internet through your server
* Seedbox Manager to help you with users.

The original script was extracted from a tutorial of Magikalex on a french website named mondédié.fr, and was created by Ex_Rat, helped by Aliochka & Meister (Munin and VsFTPD config files), Albaret (for user management), Jedediah (for web manager theming), Hydrog3n & Backtoback (seedbox manager) : 
[Installer ruTorrent sur Debian {nginx & php-fpm}](http://mondedie.fr/viewtopic.php?id=5302)

