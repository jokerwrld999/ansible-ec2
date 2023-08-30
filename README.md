# Ansible Template Playbook

This Ansible template provides a base for provisioning Linux systems with
pre-updated distros and necessary tweaks. It streamlines the process of adding
desired software and bootstrapping your servers.

## Pre-commit Commands

```
pre-commit install
pre-commit run -a
```

## Dynamic Inventory

```
ansible-inventory -i ./inventory/inventory_aws_ec2.yaml --graph
ansible-inventory -i ./inventory/inventory_aws_ec2.yaml --list
```

## Export Env Variables

```
export CUSTOM_USER=
export REGISTRY_URL=
export CONTAINER_NAME=
export DOCKER_IMAGE=
export PUBLISHED_PORTS=
export DOCKER_USERNAME=
export DOCKER_PASS=
```

## Run Ansible Playbooks

```
ansible-galaxy collection install -r requirements.yml
ansible-playbook local.yml
```
