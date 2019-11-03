# Ansible Rails

## Supported Platform

- Ubuntu 16
- Ubuntu 18

## Using it in your project

- clone the repo
- move the `ansible` directory to your project's root directory
- create a deploy user
  - Follow this guide to setup a deploy user and ssh http://climber2002.github.io/blog/2015/02/09/deploy-rails-application-on-ubuntu-14-dot-04-part-2/
- run `ansible-playbook -i hosts site.yml --extra-vars "ansible_become_pass=<deploy-user-password>"`
- Define your variables in site.yml. Once you’ve defined variables, you can use them in your playbooks using the Jinja2 templating system
## Incorrect  Su password 

If you get `incorrect su password error`, change `become_method: su` to `become_method: sudo`
