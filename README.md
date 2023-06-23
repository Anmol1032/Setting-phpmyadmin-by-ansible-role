Setting-phpmyadmin-by-ansible-role
==================================
This is an ansible role to setup *\*phpmyadmin\** with **LEMP** *(Linux, nginx, mysql, php)*.

Requirements
------------
N/A

Role Variables
--------------
* debian_name: Name of debian.
* server_name: Name of server
* root: Root directory.
* phpmyadmin_location: phpmyadmin path on url.


Dependencies
------------
N/A

Example Playbook
----------------
    - hosts: servers
      roles: 
         - { role: Setting-phpmyadmin-by-ansible-role, debian_name: abc }

License
-------
BSD
