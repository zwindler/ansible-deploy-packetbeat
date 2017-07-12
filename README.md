# ansible-deploy-packetbeat
Ansible role to install packetbeat for network metric collection

# Installation

```bash
cd /etc/ansible/roles
git clone https://github.com/zwindler/ansible-deploy-packetbeat
```

# Usage 

For quick usage, you can just copy the sample playbook

```bash
cd /etc/ansible
cp roles/ansible-deploy-packetbeat/sample-playbook.yml deploy_packetbeat.yml
cat deploy_packetbeat.yml
---
- name: Install packetbeat
  hosts: localhost
  vars:
    - elk_server: localhost
    - deploy_dashboard: false
  roles:
    - { role: ansible-deploy-packetbeat }
```
