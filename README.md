Setting-phpmyadmin-by-ansible-role
==================================
This is an ansible role to setup *\*phpmyadmin\** with **LEMP** *(Linux, nginx, mysql, php)*.

Requirements
------------
N/A

Role Variables
--------------


| variable name | work | default |
| ------------- | --- | --- |
| debian_name   | Name of debian | html |
| server_name   | Name of server | _ |
| root          | Root directory | /var/www |
| nginx_port    | Port for nginx | 80 |
| disable_default | Disable the default nginx site | true |
| phpmyadmin_location | phpmyadmin path on url | phpmyadmin |
| user_name | Initial user | phpmyadmin |
| password | Password of initial user | 12345678 |



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
