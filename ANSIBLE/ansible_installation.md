### Installing Ansible on Control Node
___________________________________________________________________________________________________

Installing Ansible on a Ubuntu Machine

Pre-requicites for installing Ansible on a Ubuntu Machine is to install Python package
- sudo apt update
- sudo apt install software-properties-common
- sudo add-apt-repository --yes --update ppa:ansible/ansible
- sudo apt install ansible


### Updating the Inventroy file in Contorl Node before installing pre-req Python and Ansible

- SSH into the Control node with the Key Pair of the EC2 Instance
- Copy the Key Pair with ssh to the /etc/.ssh
- chmod 600 MY_PEM.pem id_rsa
- Then install ansible and python on control node 
