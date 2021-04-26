# Ansible-vSphere-MassServerShutdown
Ansible-Playbook for shutting down multiple vm's in vSphere ( Vmware ).


You will have to set up a vault with the name 'vault.yml' before running the actual playbook, where you will store the 'vsphere_username' and 'vsphere password'.
Also, create the hosts inventory.

##How to run the playbook?

Run the following command:

ansible-playbook -i hosts playbook.yml --ask-vault-pass
