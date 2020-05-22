lb-tier
=========

This roles configures and sets up HAproxy for load balancer and it will also serve as a front end for three tier application.

Requirements
------------

THe roles uses a jinja template which iterates over all the app servers to which it can use to balance the application load. This template is used by HAproxy service.


Role Variables
--------------

- No variables used or required.

- Roles executes on group `[frontend]` in the dynamic inventory.

Dependencies
------------

No dependecies for this role.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: frontend
      roles:
         - name: lb-tier
           tags: 
             - frontend
             - loadbalancer

License
-------

BSD

Author Information
------------------

Tanay Shah \
contact: tanshah@redhat.com