# Ansible Playbook for Tool Installation
Automate the installation of various tools on a clean machine running Debian 12.

## Usage

1. Remove or Comment Out CD-ROM Repository Line
```bash
sudo nano /etc/apt/sources.list
```

2. Install Ansible 
```bash
sudo apt update -y
sudo apt install -y git software-properties-common ansible
```

3. Execute the Ansible Playbook
```bash
ansible-pull -U https://github.com/skraio/debian12-ansible.git --skip-tags latex
```
