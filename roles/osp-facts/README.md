osp-facts
=========

This role fetchs openstack server details and builds an in memory inventory using `add_host` module for other application execution.


Requirements
------------

No specific requirements need except the connection setup to a openstack connection machine.

Role Variables
--------------

-The role does not use external variables, but fecths the data from openstack cloud and store it in `{{ results }}` variable.

Dependencies
------------

Openstack cloud needs to be provisoned and setup for this role.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

Tanay Shah \
contact: tanshah@redhat.com
