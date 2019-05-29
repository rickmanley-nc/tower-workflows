# Ansible Tower Workflows

This repo will be a collection of different workflows to meet Standard Operating Procedures that administrators, developers, and operations teams encounter. These Ansible playbooks will then be chained together into what Ansible Tower classifies as Workflows.

## Workflow 1
- Deploy RHEL VM (golden image/template)
- Patch VM (register, update, reboot)
- Configure RHEL VM (ldap, open firewall ports)
- Install application (postgresql, add firewall ports... or possibly use https://github.com/rickmanley-nc/snapshot)
- Snapshot RHEL VM

## Workflow 2
- Update application
- Snapshot VM
