Gitlab-setadmin
===============

Ansible playbook to give administrator privileges to any number of pre-existing gitlab accounts.

Prerequisites
-------------

- The target gitlab installation needs to use postgresql as the backend and the default gitlabhq_production database.

### The inventory file
This playbook targets all machines so it is **highly advised** to create a custom inventory file for this playbook and run as:

    $ ansible-playbook -i inventory gitlab.yml 

The required accounts are specified as a YAML list on the one existing task.
