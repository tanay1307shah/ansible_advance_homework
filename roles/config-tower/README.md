Role Name
=========

This role configures tower instances with different templates and CICD workflow as well as setup up inventories and deploy's all the architecture for three tier app.

Requirements
------------

It requires, tower to be deployed as well openstack workstation to be configured correctly, before execution.

Role Variables
--------------
|Vairables| Description|
|----------------|----------------------|
|tower_guid| Ansible Tower Homework GUID|
|osp_guid| Openstack for ansible GUID|
|opentlc_login| Login ID for Opentlc|
|opentlc_repo| Opentlc login password|
|github_repo| The github repo url for this repo|
|param_repo_base| The repo base for scripts|
|region| region name, eg: us-eat-1|
|EMAIL| email for tagging|
|path_to_opentlc_key|private ssh key to login into opentlc|


Dependencies
------------

No dependencies required for this role.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      gather_facts: false  #optional, remove for faster execution
      become: yes 
      roles:
        - config-tower

License
-------

BSD

Author Information
------------------

Tanay Shah \
contact: tanshah@redhat.com
