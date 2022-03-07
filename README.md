# aci-ansible
This repository will contain Ansible playbooks for Cisco ACI.

To run any of the playbooks:

ansible-playbook register_leaf.yml -i inventory

Inventory file: contains credentials and hosts
vars files: contains variables the playbooks will use

-register_leaf.yml

This playbook will register 2 leafs (either vpc or standalone), add rack location, OOB addresses, leaf profile, leaf interface profile and VPC protection group (if VPC peer).

If only registering 1 leaf node. Leave either EVEN or ODD variables empty (example: even_id: )

Modify register_leaf_vars.yml with your data. If registering more than 2 leafs. Start a new pair with -type:  
