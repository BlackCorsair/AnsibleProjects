# User Creation Role
## What does this role do?
This role creates a set of users defined in vars, so they can connect through ssh with a RSA-4096 key. The private key will be saved at **userCreation/tmp/_user_.pem**
## How to use the role?
First you need to modify the **vars** with the users you need. Then you can modify the inventory file or use the provided _/etc/ansible/hosts_ file. An use example with the inventory file:
```
ansible-playbook userCreation.yml -i inventory 
```