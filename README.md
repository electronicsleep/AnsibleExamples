# Ansible Examples

#MacOS

brew install ansible

#Debian

apt-get install ansible

sudo vim /etc/ansible/hosts

ansible default -m ping -u ubuntu

ansible default -a "w" -u ubuntu

ansible default -a "ps -ef" -u ubuntu

ansible default -a "netstat -ta" -u ubuntu

# Get Facts

ansible default -m setup -u ubuntu

# Simple Playbooks (one file)

ansible-playbook check-user-load.yml -u ubuntu

# Run Role Playbooks (roles directory)

ansible-playbook check-lamp.yml -u ubuntu

ansible-playbook check-os.yml -u ubuntu

ansible-playbook update-os.yml -u ubuntu

ansible-playbook build-os.yml -u ubuntu

ansible-playbook build-nagios-client.yml -u ubuntu

# Resources

https://www.ansible.com

http://docs.ansible.com
