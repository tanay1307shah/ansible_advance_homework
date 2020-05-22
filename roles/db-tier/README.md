db-tier
=========

This role deploys and configures the postgres SQL database required for the three tier app. If the databse was previously installed, then just initiallize it or else, install it.

Requirements
------------

Only requirement is correct base repo to have all the packages required.

Role Variables
--------------

- No variables required used for this role.

- Roles uses `[appdbs]` group as hosts


Dependencies
------------

This roles does not have any dependencies

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: appdbs
      roles:
         - name: db-tier
           tags: 
             - postgresSQL
             - dbs

License
-------

BSD

Author Information
------------------

Tanay Shah \
contact: tanshah@redhat.com