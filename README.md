# ansible-practise
Where Ansible is installed thats called Control Node:

sudo dnf install ansible -y

Ansible is developed in python 

Connectivity usually has :
-------------------------
protocal : port : username : password : ip

ansible all -i ip -e  ansible_user=  -e ansible_password=
-m ping ;

ansible all -i ip -e  ansible_user=  -e ansible_password=
-b -m dnf -a "name=nginx state=installed"

-b ---become root user
-m ---module
-a ---arguments

ansible all -i ip -e  ansible_user=  -e ansible_password=
-b -m service -a "name=nginx state=started"
======================================
