# vagrant-docker-ansible
Multi-container Vagrantfile with Ansible Provisioner

This can be used as a test environment with multiple Ansible endpoints.

## Use:
Start the environment.  
`vagrant up`

Verify environment status.  
`vagrant status`

View containers via Docker.  
`docker ps -a`  

Access a container.  
`vagrant ssh <container_name>`  
`ssh root@<local_ip or remote_ip> -p <port> -i <private_key>`

Test ansible connectivity.
`ansible all -m ping -i ./.vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory `

Destroy the environment.  
`vagrant destroy -f`
