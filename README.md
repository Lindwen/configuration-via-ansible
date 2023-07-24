<h1 align="center">Welcome to configuration-via-ansible 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
  <a href="https://twitter.com/Lindw3n" target="_blank">
    <img alt="Twitter: Lindw3n" src="https://img.shields.io/twitter/follow/Lindw3n.svg?style=social" />
  </a>
</p>

> Repo qui contient tout mes playbooks Ansible

## Install

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

## Author

👤 **Lindwen**

* Website: https://lindwen.fr/
* Twitter: [@Lindw3n](https://twitter.com/Lindw3n)
* Github: [@Lindwen](https://github.com/Lindwen)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_