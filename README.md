install ansible with brew install ansible

playbook yaml is the main function 
inventory contains raspberry pi and ip address
group vars are overwriting variables 

group vars overwrite role default variables in multiple environments 

group vars are defined in inventory and can be overwritten specifically for each 
environment. The prod variables are in the prod inventory

and finally we got roles: contain task, defaults and templates 
they are the step by step process 
there is a main task in the role and that is what's usually being run 

basic command:
ansible-playbook playbook.yml

create inventories/all.yml
add ansible_user and ansible_host 

add host list with pi as value in playbook (first play)
add role and host in playbook

create roles and punk role inside. inside the punk role create a default directory and a tasks directory. Inside the tasks directory is hte main.yml

ssh-copy-id pi@id-address 
adds key to terminal so we can programmatically ssh into pi
ansible-vault can help getting around using a key passphrase and having a programmatic access 

become -> use elevated priviliges 

install python3 via apt-get module in role task 

