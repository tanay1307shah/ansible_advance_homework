osp-instance-delete
=========
 This role deletes the server instance for three tier app on openstack cloud.

Requirements
------------

The roles requires osp-servers role to be executed before since that provisons the servers, which are to be deleted in this role.

Role Variables
--------------

The role does not require any variables.

Dependencies
------------

It depends on osp-servers role, if that role has succeded then this will succeed and delete the instances.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: workstation
      become: yes
      roles:
        - osp-servers

License
-------
BSD

Author Information
------------------

Tanay Shah \ 
contact: tanshah@redhat.com
