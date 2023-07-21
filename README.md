0. Création d'une clé SSH et ajout sur le serveur
```sh
ssh-keygen -t ed25519
ssh-copy-id user@host
```

1. Mise à jour des paquets
```sh
sudo apt update
sudo apt upgrade
```

2. Installation d'Ansible
```sh
sudo apt install software-properties-common ansible
```

3. Vérification de l'installation
```sh
ansible --version
# ansible 2.10.8
```

4. Clone du repo
```sh
git clone https://github.com/Lindwen/configuration-via-ansible.git
cd configuration-via-ansible
```

4. Exécution du playbook
```sh
ansible-playbook -i inventory/example-inventory.ini -u your_user playbooks/install-docker.yml -vv
```
