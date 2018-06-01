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

## bootstrap kubernetes the hard way

Following the instructions from: https://github.com/kelseyhightower/kubernetes-the-hard-way

```
ANSIBLE_CONFIG=./ansible.cfg ansible-playbook -i inventory -u pirate -k k8-hard-way.yml -vv
```
