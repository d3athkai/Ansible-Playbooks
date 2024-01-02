[![GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-BE0000?style=plastic)](#)  
[![Red Hat](https://img.shields.io/badge/Red%20Hat-E5141F?style=plastic)](#) [![Rocky Linux](https://img.shields.io/badge/RockyLinux-07BA82?style=plastic)](#) [![Ubuntu+](https://img.shields.io/badge/Ubuntu-DD4814?style=plastic)](#) [![Raspberry Pi OS](https://img.shields.io/badge/Raspberry--Pi--OS-C51A4A?style=plastic)](#)  
[![Ansible](https://img.shields.io/badge/Ansible-131211?style=plastic)](#) [![Python 3](https://img.shields.io/badge/Python-3-3673A5?style=plastic)](#)  

# My Ansible Playbooks
A Work-in-Progress (WIP), with more Ansible Playbooks adding regularly.  
  
## Ansible Tips and Tricks
Refer to [My Ansible Tips and Tricks](https://gist.github.com/d3athkai/3b1c6becc41d79f45332f238791ceb3d).  
  
## Recommended Ansible Settings
In `/etc/ansible/ansible.cfg`, under `[defaults]`, add: `interpreter_python=/usr/bin/python3`
  
## Playbooks List
| S/N  | Playbook  | Description  |
| ------------- | ------------- | ------------- |
| 1 | add-yum-repo.yml  | To add a new Yum Repo for CentOS, Red Hat and Rocky Linux.<br>It has the option to disable all existing repos in `/etc/yum.repos.d`.  |
| 2 | ansible-setup-clients.yml  | To setup individual Ansible client so that the Ansible master can communicate with this client.<br>It will create a non-root privilleged user for running Ansible tasks and also plant the ssh public key from the Ansible Master.  |
| 3 | detect-family-distribution.yml  | To detect OS Family, Distribution Release & version and Architecture.  |
| 4 | vault_lookup.yaml  | To lookup key-value pairs from HashiCorp Vault.  |
