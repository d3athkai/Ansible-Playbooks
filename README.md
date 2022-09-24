![GitHub](https://img.shields.io/badge/license-GPL--3.0-orange?style=plastic) ![GitHub](https://img.shields.io/badge/Python-2.7+-green?style=plastic) ![GitHub](https://img.shields.io/badge/Ansible-2.9+-blue?style=plastic) 

# My Ansible Playbooks
A Work-in-Progress (WIP), with more Ansible Playbooks adding regularly.  
  
## Ansible Tips and Tricks
Refer to [My Ansible Tips and Tricks](https://gist.github.com/d3athkai/3b1c6becc41d79f45332f238791ceb3d).  
  
## Recommended Ansible Settings
In `/etc/ansible/ansible.cfg`, under `[defaults]`, add:  
`interpreter_python=/usr/bin/python3`
  
## Playbooks
| S/N  | Playbook  | Description  | Usage  |
| ------------- | ------------- | ------------- | ------------- |
| 1 | add-yum-repo.yml  | To add a new Yum Repo for CentOS/Red Hat.<br>It has the option to disable all existing repos in `/etc/yum.repos.d`.  | 1. Update hosts and variables.<br>2. Execute the playbook:<br>`ansible-playbook add-yum-repo.yml`  |
| 2 | ansible-setup-clients.yml  | To setup individual Ansible client so that the Ansible master can communicate with this client.<br>It will create a non-root privilleged user for running Ansible tasks and also plant the ssh public key from the Ansible Master.  | 1. Update hosts and variables.<br>2. Execute the playbook:<br>`ansible-playbook ansible-setup-clients.yml --extra-vars "host=<ip-address>" -u <existing remote user> -k -K`<br>*where:<br>-u is your existing linux user<br>-k is user password<br>-K is your user sudo password*  |
| 3 | detect-family-distribution.yml  | To detect OS Family and Distribution.  | 1. Update hosts.<br>2. Execute the playbook:<br>`ansible-playbook detect-family-distribution.yml`  |
  
