# Commandes de base Linux

- Affiche le chemin du répertoire courant.
  ```bash
  pwd
  ```

- Liste les fichiers et répertoires dans le répertoire courant.
  ```bash
  ls
  ```

- Liste les fichiers avec des détails supplémentaires (permissions, taille, date).
  ```bash
  ls -l
  ```

- Liste tous les fichiers, y compris les fichiers cachés (commençant par un `.`).
  ```bash
  ls -a
  ```

- Se déplace vers un répertoire spécifique.
  ```bash
  cd /chemin/vers/repertoire
  ```

- Revient au répertoire parent.
  ```bash
  cd ..
  ```

- Crée un nouveau répertoire.
  ```bash
  mkdir nom_dossier
  ```

- Supprime un répertoire vide.
  ```bash
  rmdir nom_dossier
  ```

- Supprime un fichier.
  ```bash
  rm fichier
  ```

- Supprime un dossier et son contenu récursivement.
  ```bash
  rm -r dossier
  ```

- Copie un fichier ou un répertoire.
  ```bash
  cp source destination
  ```

- Déplace ou renomme un fichier ou un répertoire.
  ```bash
  mv source destination
  ```

- Affiche le contenu d'un fichier.
  ```bash
  cat fichier
  ```

- Permet de visualiser le contenu d’un fichier page par page.
  ```bash
  less fichier
  ```

- Affiche les premières lignes d’un fichier.
  ```bash
  head fichier
  ```

- Affiche les dernières lignes d’un fichier.
  ```bash
  tail fichier
  ```

- Crée un fichier vide ou met à jour l'horodatage d'un fichier.
  ```bash
  touch fichier
  ```

- Écrit du texte dans un fichier.
  ```bash
  echo "texte" > fichier
  ```

- Ajoute du texte à la fin d’un fichier.
  ```bash
  echo "texte" >> fichier
  ```

- Modifie les permissions d’un fichier ou d’un répertoire.
  ```bash
  chmod 755 fichier
  ```

- Change le propriétaire d’un fichier ou d’un répertoire.
  ```bash
  chown utilisateur:fichier
  ```

- Recherche un fichier par nom dans un répertoire.
  ```bash
  find /chemin -name fichier
  ```

- Recherche du texte dans un fichier.
  ```bash
  grep "texte" fichier
  ```

- Affiche la liste des processus en cours.
  ```bash
  ps aux
  ```

- Affiche en temps réel les processus et leur utilisation des ressources.
  ```bash
  top
  ```

- Termine un processus en utilisant son identifiant (PID).
  ```bash
  kill PID
  ```

- Affiche l’espace disque disponible dans un format lisible par l'humain.
  ```bash
  df -h
  ```

- Affiche la taille d’un répertoire.
  ```bash
  du -sh
  ```

- Affiche l'utilisation de la mémoire.
  ```bash
  free -h
  ```

- Affiche la configuration réseau.
  ```bash
  ifconfig
  ```

- Envoie des paquets à une adresse IP pour tester la connectivité.
  ```bash
  ping adresse_ip
  ```

- Télécharge un fichier depuis une URL.
  ```bash
  wget url
  ```

- Transfère des données depuis ou vers un serveur via une URL.
  ```bash
  curl url
  ```

## Gestion des utilisateurs

- Ajoute un nouvel utilisateur.
  ```bash
  useradd utilisateur
  ```

- Modifie le mot de passe d’un utilisateur.
  ```bash
  passwd utilisateur
  ```

- Ajoute un utilisateur à un groupe.
  ```bash
  usermod -aG groupe utilisateur
  ```

- Supprime un utilisateur.
  ```bash
  userdel utilisateur
  ```

- Affiche le nom de l’utilisateur connecté.
  ```bash
  whoami
  ```

- Exécute une commande avec des privilèges administratifs.
  ```bash
  sudo commande
  ```

## Gestion des paquets (Ubuntu/Debian)

- Met à jour la liste des paquets disponibles.
  ```bash
  apt update
  ```

- Met à jour les paquets installés.
  ```bash
  apt upgrade
  ```

- Installe un paquet.
  ```bash
  apt install nom_paquet
  ```

- Supprime un paquet installé.
  ```bash
  apt remove nom_paquet
  ```

- Recherche un paquet dans les dépôts.
  ```bash
  apt search nom_paquet
  ```

## Archive et compression

- Crée une archive tar d’un dossier.
  ```bash
  tar -cvf archive.tar dossier/
  ```

- Extrait une archive tar.
  ```bash
  tar -xvf archive.tar
  ```

- Crée une archive compressée en gzip.
  ```bash
  tar -czvf archive.tar.gz dossier/
  ```

- Extrait une archive compressée en gzip.
  ```bash
  tar -xzvf archive.tar.gz
  ```

- Crée une archive zip d’un dossier.
  ```bash
  zip -r archive.zip dossier/
  ```

- Extrait une archive zip.
  ```bash
  unzip archive.zip
  ```

## Informations sur le système

- Affiche des informations sur le système.
  ```bash
  uname -a
  ```

- Affiche ou modifie le nom de l’hôte.
  ```bash
  hostname
  ```

- Affiche le temps écoulé depuis le dernier démarrage.
  ```bash
  uptime
  ```

- Affiche les messages du noyau.
  ```bash
  dmesg
  ```

- Affiche l’historique des commandes.
  ```bash
  history
  ```

## Redirection et piping

- Redirige la sortie standard vers un fichier (écrase le contenu).
  ```bash
  commande > fichier
  ```

- Redirige la sortie standard vers un fichier (ajoute au contenu).
  ```bash
  commande >> fichier
  ```

- Redirige les erreurs standard vers un fichier.
  ```bash
  commande 2> fichier
  ```

- Envoie la sortie de la première commande comme entrée à la deuxième (piping).
  ```bash
  commande1 | commande2
  ```

## Autres commandes utiles

- Crée un alias pour une commande.
  ```bash
  alias nom='commande'
  ```

- Ouvre un fichier pour l'éditer dans l'éditeur Nano.
  ```bash
  nano fichier
  ```

- Affiche le manuel d’une commande.
  ```bash
  man commande
  ```

- Ferme le terminal ou une session SSH.
  ```bash
  exit
  ```
