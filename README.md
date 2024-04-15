# FTP-DNS-DHCP-SSH
#Consignes
Objectif

Configurer un environnement réseau virtuel à l'aide de deux
machines virtuelles Debian, en mettant en place un serveur
DHCP et DNS sur la première machine, ainsi qu'un
serveur-client FTP avec SSH sur la seconde machine.

Lire le sujet jusqu’à la fin avant de le commencer !

Étapes à suivre

1. Installation de Debian sans interface graphique :
- Mettez en place deux machines virtuelles Debian sans interface
graphique et dans un réseau virtuel créé par votre logiciel de
virtualisation.

2. Mise à jour des systèmes :
- Vérifiez et appliquez les mises à jour nécessaires sur les deux
machines.


3. Configuration du Serveur DHCP :
- Installez un serveur DHCP sur la première machine.
- Configurez le serveur DHCP pour attribuer des adresses de classe B
aux machines connectées au réseau.
- Assurez-vous que la machine hébergeant le serveur DHCP possède
une adresse IP fixe.

4. Installation du Serveur FTP et SSH :
- Sur la deuxième machine, installez un serveur FTP (proFTPd) et SSH.
- Configurez le serveur FTP avec une seule session de connexion possible.
- Utilisez les identifiants suivants pour le FTP :
- Identifiant : laplateforme
- Mot de passe : Marseille13!
- Utilisez le serveur SSH pour les connexions au FTP en SFTP, renforçant ainsi
la sécurité.

5. Installation du Serveur DNS :
- Installez un serveur DNS sur la première machine.
- Configurez le DNS de sorte que le lien soit "dns.ftp.com", pointant vers
l'adresse IP de la deuxième machine où le serveur FTP est installé.

6. Test de Connexion au Serveur SFTP :
- Une fois toutes les configurations réalisées, tentez de vous connecter au
serveur SFTP de la deuxième machine en utilisant les identifiants fournis
(`laplateforme` et `Marseille13!`).
- Utilisez l'adresse "dns.ftp.com" pour la connexion.

7. Paramètres de Sécurité Additionnels :
- Afin de renforcer la sécurité du serveur SFTP :
- Restreignez l'accès au serveur uniquement avec les identifiants
fournis.
- Configurez le serveur pour fonctionner sur le port 6500.
- Évitez toute connexion anonyme ou invité sur le serveur.
