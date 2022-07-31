# minecraft-starter

Un projet starter pour serveur minecraft encapsulé dans docker, par ce qu'il y en a marre de tout configurer à la main.

Ce projet se base sur le repo https://github.com/itzg/docker-minecraft-server.
Pour toute autre information de paramétrage, merci de consulter ce merveilleux projet!

## Premier Lancement: Guidelines

1. Cloner le projet à l'emplacement voulu
2. Configurer le nom du monde et le dossier `/data` si souhaité
3. Renseigner ou désactiver la whitelist
4. Lancer le serveur

## Lancer le serveur

// TODO

## Configuration de Jeu

### Whitelist / Ops

- Whitelist: https://github.com/itzg/docker-minecraft-server#whitelist-players
- Ops: https://github.com/itzg/docker-minecraft-server#opadministrator-players

### Difficulté

https://github.com/itzg/docker-minecraft-server#difficulty

### PVP

https://github.com/itzg/docker-minecraft-server#pvp-mode

## Configuration Technique

Toutes les propriétés sont à modifier directement dans le fichier `docker-compose.yml`

### Choisir la version de minecraft

Pour choisir la version, attribuer la propriété `VERSION` d'une version spécifique (`"1.7.9"` par exemple), ou `"LATEST"` pour récupérer la version la plus à jour.

https://github.com/itzg/docker-minecraft-server#versions

### Définir le dossier de données

Pour définir le dossier de données qui sera utilisé par le serveur, modifier l'entrée pointant vers le répertoire `/data` de la propriété `volumes`.

Plus d'informations sur l'emplacement des données:

- Structure: https://github.com/itzg/docker-minecraft-server#data-directory
- Choisir l'emplacement des données sur la machine hôte: https://github.com/itzg/docker-minecraft-server#attaching-data-directory-to-host-filesystem

### Autopause

La configuration est prévue pour mettre en pause le serveur automatiquement lorsque personne n'interragit avec durant un certain temps. Cette durée est configurable, en secondes.

https://github.com/itzg/docker-minecraft-server#autopause

### Utilisation de la ram

La configuration est prévue pour gérer une quantité restreinte de RAM. Il est possible de l'augmenter via les propriétés d'environnement.

https://github.com/itzg/docker-minecraft-server#memory-limit
