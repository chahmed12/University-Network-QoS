#  Projet Réseau VLAN - Packet Tracer

##  Description
Ce projet illustre une topologie réseau utilisant plusieurs VLANs pour la segmentation. Il simule un réseau avec routage inter-VLAN à l'aide d'un routeur Cisco, un switch, des PCs et des serveurs, le tout configuré dans Cisco Packet Tracer.

---

##  Topologie du réseau

- **1 Routeur Cisco 2901**
- **1 Switch Cisco 2960**
- **3 PCs** répartis dans différents VLANs :
  - PC0 (Académique - VLAN 20)
  - PC1 (Admin - VLAN 30)
  - PC2 (Public - VLAN 40)
- **3 Serveurs dans VLAN 50 (Serveurs)** :
  - Server3 (Kedux)
  - Server4 (Gmail)
  - Server5 (Classroom)

---

##  Fichiers inclus

| Nom du fichier              | Description                                      |
|----------------------------|--------------------------------------------------|
| `README.md`                | Documentation du projet                         |
| `router_config.txt`        | Configuration du routeur Cisco 2901             |
| `switch_config.txt`        | Configuration du switch Cisco 2960              |
| `ip_configurations.txt`    | Adressage IP statique des PCs et serveurs       |
| `vlan_project.pkt`         | Fichier Cisco Packet Tracer (à ajouter)         |

---

##  Plan d’adressage IP

| Appareil   | VLAN | Adresse IP         | Passerelle         |
|------------|------|---------------------|---------------------|
| PC0        | 20   | 192.168.20.10       | 192.168.20.1        |
| PC1        | 30   | 192.168.30.10       | 192.168.30.1        |
| PC2        | 40   | 192.168.4.10        | 192.168.4.1         |
| Server3    | 50   | 192.168.50.10       | 192.168.50.1        |
| Server4    | 50   | 192.168.50.11       | 192.168.50.1        |
| Server5    | 50   | 192.168.50.12       | 192.168.50.1        |

---

##  Configuration CLI

Les configurations complètes se trouvent dans les fichiers suivants :

-  `config-routeur.txt` – Configuration du routeur (sous-interfaces, dot1Q, IP)
-  `config-switch.txt` – VLANs, trunk, ports access, sécurisation
-  `config-pcs.txt` – Commandes IP pour les PCs et serveurs

---

##  Déploiement avec Git & GitHub

1. Initialiser un dépôt Git :
   ```bash
   git init
