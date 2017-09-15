# mongodb
Ansible Role for MongoDB installation on a single Node

## Supported Platforms
```
rhel 7.2

```
## Using this role in plabook
The playbook to use this role can be used in original playbook by simply creating a requirements.yml file
and referencing the role in your main playbook (e.g. playbook.yml or site.yml )
```
➜  $ tree .
.
├── inventory
│   └── palo-dev
├── playbook.yml
├── requirements.yml
└── roles
    └── README.md

```
```
➜  $ cat requirements.yml 
- name: acuo-compose
  src: https://github.com/pbuditi-ansible-roles/ansible-acuo-compose
  version: master
```
```
➜  $ cat playbook.yml 
---
# test roles

- name: deploy acuo docker compose
  hosts: all
  roles:
    - acuo-compose
➜  $
```
