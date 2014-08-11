Keynote about playbooks
=======================

### Install Ansible
```
install pip: wget https://bootstrap.pypa.io/get-pip.py
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
