# network_cli_demo
Simple demo playbooks to demonstrate the network_cli connection type with Ansible, to accompany blog post.

## Pre-2.5 Playbook

```
ansible-playbook -i hosts-2.4.ini playbook-2.4.yml
```

## Partial refactor for Ansible 2.5

```
ansible-playbook -i hosts-2.4.ini -u cisco -k -e ansible_network_os=ios playbook-2.5-refactor.yml
```

## Refactored for Ansible 2.5

```
ansible-playbook -i hosts.ini -u cisco -k playbook-2.5-final.yml
```