# Ansible Tower Workflows

This repo will be a collection of different workflows to meet Standard Operating Procedures that administrators, developers, and operations teams encounter. These Ansible playbooks will then be chained together into what Ansible Tower classifies as Workflows.

## Workflow 1 - Deploy From Gold Standard
- Deploy RHEL VM (golden image/template)
- Register
- Configure RHEL VM (ldap, motd, firewall)
- Install application (postgresql, add firewall ports... or possibly use https://github.com/rickmanley-nc/snapshot)
- Snapshot VM

## Workflow 2 - Update VM
- Snapshot VM
- Patch VM (update, reboot)
- Snapshot VM

## Workflow 3 - Update Application
- Snapshot VM
- Update application
- Snapshot VM

## Workflow 4 - Vulnerability Scan
- Reoccurring workflow that runs against all RHEL VMs on a RHV Cluster.
