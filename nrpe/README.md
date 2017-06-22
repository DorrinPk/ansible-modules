## nagios plugin to deploy NRPE to the server for monitoring


* to deploy this module to your server, add your server to the host list : `/nrpe/hosts`
* Make sure you can ssh into the server and the server has python on it
* run : `ansible-playbook -i /nrpe/hosts /nrpe/tasks/main.yml -K`

This script works for Ubuntu and Amazon AMI. 
