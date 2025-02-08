[servers]
server_1 ansible_host= ip_address
server_2 ansible_host= ip_address

[servers:vars]
ansible_ssh_private_key_file=/home/ubuntu/keys/MY_PEM.pem
ansible_user=ubuntu
ansible_python_interpreter=/usr/bin/python3
