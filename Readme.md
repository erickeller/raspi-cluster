# Raspi cluster

## Ansible management

## Getting started

1. update the `inventory` file
1. try the ping module
```
ANSIBLE_CONFIG=./ansible.cfg ansible -m ping -u pirate -k -i inventory all
```

## Update all nodes

```
ANSIBLE_CONFIG=./ansible.cfg ansible-playbook -i inventory -u pirate -k update.yml
```
