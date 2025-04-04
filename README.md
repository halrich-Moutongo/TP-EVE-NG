# TP-EVE# TP EVE-NG : Interconnexion de deux LANs et accès Internet

Ce dépôt contient la configuration EVE-NG pour un TP visant à interconnecter deux réseaux locaux (LAN A et LAN B) et à permettre aux machines de ces réseaux d'accéder à Internet.

## Topologie

Une représentation visuelle de la topologie est disponible dans le dossier `Topologie/`.

## Objectifs

* Configurer l'adressage IP sur les différents périphériques.
    1- soit dynamiquement via le protocole DHCP sur le routeur(Optionnel mais recommandé)
    2- soit statiquement en saisant les IP et en configurant sur le routeur un NAT(Network address translation) via l'interface routeur connecté à internet
* Configurer le routage entre les deux LANs via le routeur central.
* Configurer une route par défaut sur le routeur central pour permettre l'accès à Internet (simulé).
* Vérifier la connectivité entre les machines des deux LANs.
* Vérifier l'accès à Internet depuis les machines des LANs.

## Configurations

Les fichiers de configuration pour chaque périphérique sont disponibles dans le dossier `Configurations/`.

* **Routeur_Central/** : Configurations du routeur central assurant l'interconnexion et l'accès Internet.
* **Switch_LAN_A/** : Configuration de base du switch du LAN A.
* **Switch_LAN_B/** : Configuration de base du switch du LAN B.
* **PC_LAN_A/** : Configuration IP du PC du LAN A.
* **PC_LAN_B/** : Configuration IP du PC du LAN B.

## Instructions

1. Importer le fichier de topologie EVE-NG (si vous l'avez exporté) ou recréer la topologie en vous basant sur l'image `Topologie/Topologie.png`.
2. Copier le contenu des fichiers de configuration (`startup-config.txt`) dans la configuration de démarrage de chaque périphérique correspondant dans EVE-NG.
3. Démarrer les périphériques.
4. Vérifier la connectivité en utilisant les commandes `ping` depuis les PCs.
5. Vérifier l'accès à Internet (simulé) depuis les PCs.

## Notes

* Ce TP suppose une configuration de base des switches (VLAN par défaut). Des configurations VLAN plus avancées pourraient être ajoutées.
* L'accès à Internet est simulé par un "cloud" EVE-NG connecté au routeur central avec une configuration permettant le routage par défaut.
* Les fichiers `running-config.txt` peuvent être ajoutés après avoir démarré les périphériques et sauvegardé leur configuration en cours.

## Auteur

halrich-Moutongo/TP-EVE-NG 
