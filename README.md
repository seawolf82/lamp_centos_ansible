# lamp_centos_ansible


This script install on centos7 apache with mariadb and php5.4 


To install  stack lamp on centos7 run:

ansible-playbook -i hosts site.yaml

To uninstall stack lamp on centos7 run:

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
