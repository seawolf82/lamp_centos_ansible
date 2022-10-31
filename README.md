# lamp_centos_ansible


This script install on RedHat based Distributions apache with mariadb and php 

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version


To install stack lamp on RedHat based Distributions run:

ansible-playbook -i hosts site.yaml

To uninstall stack lamp on RedHat based Distributions run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
mariadb
apache
php
ntp

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
