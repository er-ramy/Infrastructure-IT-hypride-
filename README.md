# 🛡️ Architecture, Automatisation et Déploiement Cloud d'une Infrastructure Sécurisée (De V1.0 à DevOps)

## 📌 À propos de ce projet
Élève ingénieur en **Systèmes, Réseaux et Cloud**, je conçois ce projet dans le cadre de mon **développement continu**. Ce dépôt documente la création d'un environnement serveur virtualisé (Debian), conçu pour simuler une infrastructure de production robuste. 

Cette **Version 1.0** se concentre sur la configuration manuelle et la compréhension profonde des couches système, réseau et cryptographique.

📄 **[👉 Consultez le Portfolio Technique complet avec les Preuves de Concept (PoC) en PDF ici](./Portfolio_Technique_Debian_Server.pdf)**

## 🛠️ Stack Technique (V1.0)
* **OS :** Debian Linux (Server)
* **Web & BDD :** Apache 2, MariaDB, PHP (Stack LAMP)
* **Réseau :** TCP/IP, OpenVPN, WireGuard, NAT, Port Forwarding
* **Sécurité :** OpenSSL (RSA, X.509), SSH Key-based Auth, UFW

## ⚙️ Architecture et Implémentation (Preuves de Concept)
*Note : Le détail complet de l'audit et les captures d'écran des terminaux sont documentés dans le rapport PDF ci-dessus.*

### 1. Sécurisation et Cryptographie (Hardening)
Désactivation de l'authentification par mot de passe pour le compte Root. L'accès est sécurisé de bout en bout via un échange de paires de clés asymétriques RSA.

### 2. Déploiement Web (VirtualHosts & SSL/TLS)
Hébergement compartimenté via VirtualHosts. Sécurité des flux garantie par la cryptographie TLS/SSL (Certificats X.509 OpenSSL auto-signés) sur le port 443, avec résolution DNS locale.

### 3. Ingénierie Réseau et Tunnels VPN
Audit réseau (`ss -tulpn`) et configuration d'interfaces virtuelles pour le tunneling chiffré via **OpenVPN** (UDP 1194) et **WireGuard** (UDP 51820).

### 4. Supervision des Services
Audit régulier de la consommation des ressources (RAM, CPU, Processus) via des outils interactifs (`htop`) pour garantir la stabilité et la légèreté de l'architecture.

## 🗺️ Roadmap Technique (L'évolution du projet)
Ce laboratoire virtuel est conçu pour évoluer de manière itérative vers les standards de l'industrie :
* ⏳ **V2.0 (Automatisation Native) :** Intégration de scripts **Bash** pour l'automatisation de l'administration système et des sauvegardes (Backups).
* ⏳ **V3.0 (IaC & SDN) :** Automatisation avancée et idempotente avec **Python** et **Ansible**.
* ⏳ **V4.0 (Cloud & DevOps) :** Transition vers des architectures Cloud, CI/CD, et conteneurisation.

---
*Projet réalisé par ER-RAMY MAROUANE.*
