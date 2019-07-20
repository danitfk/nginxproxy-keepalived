NGINXProxy + Keepalived
=========

This playbook install and configure NGINX Reverse proxy with Keepalived. 


Role Variables
--------------

The variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.
Before running the playbook you should adjust variables in `defaults/main.yml`.


Example Playbook
----------------

Here goes an example:


```
---
- hosts: production
  become: yes
  roles:
    - { role: nginxproxy-keepalived }

```

How to Run
-----------
1) Adjust variables in `defaults/main.yml`
2) Prepare a proper inventory file like `inventory/production`
3) Run playbook `ansible-playbook -i nginxproxy-keepalived/inventory/production main.yml`


License
-------

The Unlicense


