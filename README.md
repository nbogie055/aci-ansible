# aci-ansible
This repository will contain Ansible playbooks for Cisco ACI.

To run any of the playbooks:

ansible-playbook register_leaf.yml -i inventory

Inventory file: contains credentials and hosts
vars files: contains variables the playbooks will use

- register_leaf.yml

1. Modify register_leaf_vars.yml with your data
2. If registering more than 2 leafs. Start a new pair with -type:  