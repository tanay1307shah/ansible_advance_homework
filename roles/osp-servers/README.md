osp-servers
=========

This role provisions servers on openstack cloud used for three tier app.

Requirements
------------

It requires connection and root access to openstack cloud.

Role Variables
--------------

The role uses the dictonary variable defined in `vars/main.yml`, which is converts into items. Each item represents a server, and falcts related to it.

Dependencies
------------

No other dependecies, required for the role execution.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: workstation
      become: yes
      roles:
        - osp-instance-delete

License
-------

BSD

Author Information
------------------

Tanay Shah \ 
contact: tanshah@redhat.com
