# laptop-setup
Ansible project for automatically installing software on a Linux host (Ubuntu)

The idea for this project is to complete automate the installation of all useful software and their associated packages. In general the software will be development oriented including various programming languages.

It should also install several IDEs and DEVops tools for a full dev experience.

In order to run the playbook the ssh key should be added to the ansible server:
ssh-keyscan -H <ip-address> >> ~/.ssh/known_hosts 
  
To allow for all software to be installed run the playbook using the -K option to become sudo root eg:
ansible-playbook software-installer.yml -K

Then enter the sudo password when prompted.
