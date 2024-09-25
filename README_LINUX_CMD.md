# Commandes de base Linux

- `pwd` : Affiche le chemin du répertoire courant.
- `ls` : Liste les fichiers et répertoires dans le répertoire courant.
- `ls -l` : Liste les fichiers avec des détails supplémentaires (permissions, taille, date).
- `ls -a` : Liste tous les fichiers, y compris les fichiers cachés (commençant par un `.`).
- `cd /chemin/vers/repertoire` : Se déplace vers un répertoire spécifique.
- `cd ..` : Revient au répertoire parent.
- `mkdir nom_dossier` : Crée un nouveau répertoire.
- `rmdir nom_dossier` : Supprime un répertoire vide.
- `rm fichier` : Supprime un fichier.
- `rm -r dossier` : Supprime un dossier et son contenu récursivement.
- `cp source destination` : Copie un fichier ou un répertoire.
- `mv source destination` : Déplace ou renomme un fichier ou un répertoire.
- `cat fichier` : Affiche le contenu d'un fichier.
- `less fichier` : Permet de visualiser le contenu d’un fichier page par page.
- `head fichier` : Affiche les premières lignes d’un fichier.
- `tail fichier` : Affiche les dernières lignes d’un fichier.
- `touch fichier` : Crée un fichier vide ou met à jour l'horodatage d'un fichier.
- `echo "texte" > fichier` : Écrit du texte dans un fichier.
- `echo "texte" >> fichier` : Ajoute du texte à la fin d’un fichier.
- `chmod 755 fichier` : Modifie les permissions d’un fichier ou d’un répertoire.
- `chown utilisateur:fichier` : Change le propriétaire d’un fichier ou d’un répertoire.
- `find /chemin -name fichier` : Recherche un fichier par nom dans un répertoire.
- `grep "texte" fichier` : Recherche du texte dans un fichier.
- `ps aux` : Affiche la liste des processus en cours.
- `top` : Affiche en temps réel les processus et leur utilisation des ressources.
- `kill PID` : Termine un processus en utilisant son identifiant (PID).
- `df -h` : Affiche l’espace disque disponible dans un format lisible par l'humain.
- `du -sh` : Affiche la taille d’un répertoire.
- `free -h` : Affiche l'utilisation de la mémoire.
- `ifconfig` : Affiche la configuration réseau.
- `ping adresse_ip` : Envoie des paquets à une adresse IP pour tester la connectivité.
- `wget url` : Télécharge un fichier depuis une URL.
- `curl url` : Transfère des données depuis ou vers un serveur via une URL.

## Gestion des utilisateurs

- `useradd utilisateur` : Ajoute un nouvel utilisateur.
- `passwd utilisateur` : Modifie le mot de passe d’un utilisateur.
- `usermod -aG groupe utilisateur` : Ajoute un utilisateur à un groupe.
- `userdel utilisateur` : Supprime un utilisateur.
- `whoami` : Affiche le nom de l’utilisateur connecté.
- `sudo commande` : Exécute une commande avec des privilèges administratifs.

## Gestion des paquets (Ubuntu/Debian)

- `apt update` : Met à jour la liste des paquets disponibles.
- `apt upgrade` : Met à jour les paquets installés.
- `apt install nom_paquet` : Installe un paquet.
- `apt remove nom_paquet` : Supprime un paquet installé.
- `apt search nom_paquet` : Recherche un paquet dans les dépôts.

## Archive et compression

- `tar -cvf archive.tar dossier/` : Crée une archive tar d’un dossier.
- `tar -xvf archive.tar` : Extrait une archive tar.
- `tar -czvf archive.tar.gz dossier/` : Crée une archive compressée en gzip.
- `tar -xzvf archive.tar.gz` : Extrait une archive compressée en gzip.
- `zip -r archive.zip dossier/` : Crée une archive zip d’un dossier.
- `unzip archive.zip` : Extrait une archive zip.

## Informations sur le système

- `uname -a` : Affiche des informations sur le système.
- `hostname` : Affiche ou modifie le nom de l’hôte.
- `uptime` : Affiche le temps écoulé depuis le dernier démarrage.
- `dmesg` : Affiche les messages du noyau.
- `history` : Affiche l’historique des commandes.

## Redirection et piping

- `commande > fichier` : Redirige la sortie standard vers un fichier (écrase le contenu).
- `commande >> fichier` : Redirige la sortie standard vers un fichier (ajoute au contenu).
- `commande 2> fichier` : Redirige les erreurs standard vers un fichier.
- `commande1 | commande2` : Envoie la sortie de la première commande comme entrée à la deuxième (piping).

## Autres commandes utiles

- `alias nom='commande'` : Crée un alias pour une commande.
- `nano fichier` : Ouvre un fichier pour l'éditer dans l'éditeur Nano.
- `man commande` : Affiche le manuel d’une commande.
- `exit` : Ferme le terminal ou une session SSH.
