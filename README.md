# Ansible Setup

Автоматизация установки используемых мной инструментов на Debian 12

## Инструкция

1. Закоментируй строку с репозиторием CD-ROM
```bash
sudo vi /etc/apt/sources.list
```

2. Установи Ansible
```bash
sudo apt update -y
sudo apt install -y git software-properties-common ansible
```

3. Выполни Ansible-playbook
```bash
ansible-pull -U https://github.com/skraio/ansible-setup.git -t basis
```
