# Ansible-vSphere-MassServerShutdown
Ansible-Playbook for shutting down multiple vm's in vSphere ( Vmware ).


## Prerequisites

You will have to set up a vault with the name 'vault.yml' before running the actual playbook, where you will store the 'vsphere_username' and 'vsphere password'.
Also, create the hosts inventory. Alongside the 'ansible_host' parameter, add the 'vcenter' parameter that will be used in the vmware-guest module, in case the vm's will be located in different vcenters. In case you have only one vcenter, you can hardcode the vcenter name in the playbook.

The playbook offers the option to schedule a shutdown operation in vSphere.

## How to run the playbook?

Run the following command:

ansible-playbook -i hosts playbook.yml --ask-vault-pass
