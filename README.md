# TP-EVE# TP EVE-NG : Interconnexion de deux LANs et accès Internet

Ce dépôt contient la configuration EVE-NG pour un TP visant à interconnecter deux réseaux locaux (LAN A et LAN B) et à permettre aux machines de ces réseaux d'accéder à Internet.

## Topologie

Une représentation visuelle de la topologie est disponible dans le dossier `Topologie/`.

## Objectifs

* Configurer l'adressage IP sur les différents périphériques.
  
    1- soit dynamiquement via le protocole DHCP sur le routeur(mise en place)
    2- soit statiquement en saisant les IP et en configurant sur le routeur un NAT(Network address translation) via l'interface routeur connecté à internet(pas mise en place)
  
* Configurer le routage entre les deux LANs via le routeur central.
* Vérifier la connectivité entre les machines des deux LANs.
* Vérifier l'accès à Internet depuis les machines des LANs.

## Configurations

Les fichiers de configuration pour chaque périphérique sont disponibles dans le dossier `Configurations/`.

* **Routeur_Central/** : Configurations du routeur central assurant l'interconnexion et l'accès Internet.
* **PC_LAN_A/** : Configuration IP du PC du LAN A.
* **PC_LAN_B/** : Configuration IP du PC du LAN B.

## Instructions

1. Démarrer les périphériques.
2. Vérifier la connectivité en utilisant les commandes `ping` depuis les PCs.
3. Vérifier l'accès à Internet (simulé) depuis les PCs.

## Notes

* L'accès à Internet est simulé par un "cloud" EVE-NG connecté au routeur central.
* Les fichiers `running-config.txt` peuvent être ajoutés après avoir démarré les périphériques et sauvegardé leur configuration en cours.

## Auteur

halrich-Moutongo/TP-EVE-NG 
