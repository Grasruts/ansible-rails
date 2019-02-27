# Ansible Rails

## Supported Platform

- Ubuntu 16
- Ubuntu 18

## Using it in your project

- clone the repo
- move the `ansible` directory to your project's root directory
- run `ansible-playbook -i hosts site.yml --extra-vars "ansible_become_pass=<deploy-user-password>"`
