# Système d'alarme avec un Raspberry Pi

Des projets proches du projet **Domotique avec commandes vocales et Tkinter sur des Raspberry Pi**: <a href="https://github.com/ugolabo/domotique_commandes_vocales">bouton droit vers repo</a>

1. [Projet, v1](#projet-v1-avec-bouton)
2. [Projet, v2](#projet-v2-avec-console-pygame)

## Projet, v1: avec bouton

**Objectif:** maitriser les fondements des nanoordinateurs (Raspberry Pi), des OS Linux (Raspbian, mais aussi Ubuntu, les CLI) et de montages, du langage Python embarqué, de concepts comme les rappels haut et bas, les fils d'exécution (*thread*), des évènements sur le système (boutons), de la gestion du temps, du protocole SMTP pour les courriels et plus afin de construire des projets simples en IoT et de pouvoir collaborer avec des spécialistes de ces domaines dans des projets avancés.

Montage:

1. Un contact représentant une porte ou une fenêtre
   - Lorsque le fil est branché, le circuit est fermé et l'état du contact est actif
   - Lorsque le fil est débranché, le circuit est ouvert et l'état du contact est inactif
2. Un bouton
   - pour armer ou désarmer le système: état armé ou désarmé
3. Une DEL rouge allumée; système en état armé
4. Une DEL jaune clignotante; système en état d'alerte

Schéma Fritzing global avec un Raspberry Pi 3 (le projet a été fait avec un RPi4)

<img src="img/diagramme_fritzing.jpg" alt="">

| Schéma bouton | Schéma contact  | Schéma DEL  |
|:---|:---|:---|
| <img src="img/schema_bouton.jpg" alt="" width="200"> | <img src="img/schema_contact.jpg" alt="" width="200">  | <img src="img/schema_dels.jpg" alt="" width="200">  |

Concrètement, le contact pourrait être un interrupteur reed (ou alors un détecteur de mouvement ou de proximité)

|   |   |    |
|:---|:---|:---|
| <img src="img/reed_switch1.jpg" alt="" width="200"> | <img src="img/reed_switch2.jpg" alt="" width="200">  | <img src="img/reed_switch3.jpg" alt="" width="200">  |

Diagramme d'états

<img src="img/diagramme_etat.jpg" alt="">

## Projet, v2: avec console Pygame

**Objectif:** poursuivre avec la programmation embarquée et s'initier à la programmation orientée objet en Python pour gérer les états et les changements d’état, la journalisation (*logging*), la conception d'interfaces graphiques (avec Pygame), la gestion de plus d'évènements sur le système (clavier, souris), la récupération de données du web avec un *API* (OWM), l'importation de données de fichiers YAML, l'architecture de paquets et la configuration des fichiers et dossiers Python avec des fichiers comme __init__.py et main.py ou une ligne d'instruction comme  `__name__ == "__main__":` et plus.

| Clavier | Armer, désarmer  |
|:---|:---|
| <img src="img/console1.gif" alt="" width="250">  | <img src="img/console2.gif" alt="" width="250"> |
| **Tenter d'armer, armer**  | **Déclencher, désarmer ou alerte** |
| <img src="img/console3.gif" alt="" width="250">  | <img src="img/console4.gif" alt="" width="250"> |
