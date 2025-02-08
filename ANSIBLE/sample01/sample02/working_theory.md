#### Testing Ansible installation and worker nodes from Ansible control node

--> create 3 ubuntu/any os EC2 instances 
--> Make one instance as a Ansible - Control Node
--> other two instances remain as Worker nodes 
--> In the control node, install ansible, python gets installed as pre-req, open a file using sudo command
--> sudo nano /etc/ansible/hosts and enter the inventory details of the worker nodes/ server details with ip address
--> to check whether the worker node ip addresses are added correctly, use the ping command to check 
--> "ansilbe server -m ping"
--> copy the key pair from local machine to ec2 instance using scp command and change the usermode for the file ex: sudo chmod 400 "file_name_of_the_key_pair"
--- then create a YAML file on the control node ex: update_servers.yaml, for updating the servers/ worker nodes remotely.
--- once the update_servers.yaml file is created, you can run the yaml file using command
--- "ansible-playbook -i /etc/ansible/hosts update_servers.yaml"