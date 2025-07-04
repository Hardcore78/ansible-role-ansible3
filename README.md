# Déploiement WordPress avec Docker & Ansible
sofiane mahi-moussa
Ce projet illustre comment construire un environnement WordPress « from scratch » en combinant :

- **Docker** : conteneurs Ubuntu et Rocky Linux avec SSH et pile LAMP  
- **Docker Compose** : orchestration des services  
- **Ansible** : configuration et déploiement automatisé  

---

## Structure du projet

```text
.
├── docker-compose.yaml       # orchestration des conteneurs
├── inventaire                # inventaire Ansible (SSH hosts)
├── fin                       # playbook Ansible principal
├── ubuntu-ssh/
│   └── Dockerfile            # image Ubuntu 24.04 + SSH
└── rocky-ssh/
    └── Dockerfile            # image Rocky 9 + SSH + LAMP
