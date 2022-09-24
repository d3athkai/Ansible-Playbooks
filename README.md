![GitHub](https://img.shields.io/badge/license-GPL--3.0-orange?style=plastic) ![GitHub](https://img.shields.io/badge/Python-2.7+-green?style=plastic) ![GitHub](https://img.shields.io/badge/Ansible-2.9+-blue?style=plastic) 

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
  
