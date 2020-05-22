app-tier
=========

This configures the backend service and infrastructe in the Three Tier Application. It installs and sets up Tomcat server and Httpd module for communication. 

Requirements
------------

The requirement is to have the correct repo configured to have the required packages to be installed.


Role Variables
--------------

This roles uses a dynamic inventory, where it uses group vars `[apps]` as servers:

    [app]
    app1
    app2

Also this role uses a special ansible variable 
 
    {{ inventory_hostname }} - Current hostname on which the playbook is working on. i.e. app1 & app2


Dependencies
------------

The role does not have any dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: apps
      roles:
         - name: app-tier
           tag:
             - apps
             - Tomcat
             - httpd

License
-------

BSD

Author Information
------------------

Tanay Shah \
contact: tanshah@redhat.com