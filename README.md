Keynote about playbooks
=======================

### Install Ansible
```
wget https://bootstrap.pypa.io/get-pip.py
python get-pip.py
sudo pip install ansible
```

### What to do before first run ansible-playbook
```
cd /etc
sudo mkdir ansible
sudo vim hosts
input: localhost ansible_connection=local
```

### Best project struture
```
site.yml
webserver.yml
dbserver.yml
roles/
  common/
    file/
    tmeplates/
    tasks/
    handlers/
    vars/
    meta/
  webconfigure/
    files/
    templates/
    tasks/
    handlers/
    vars/
    meta/
```
##### then as the entrance of the playbooks, could be:
```
---
- hosts: webserver
  roles:
    - common
    - webconfigure
```
