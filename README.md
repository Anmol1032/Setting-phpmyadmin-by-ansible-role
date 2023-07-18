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
```yaml
---
- hosts: localhost
    roles:
    - role: Setting-phpmyadmin-by-ansible-role
      nginx_port: 80
      debian_name: Anmol1032
      server_name: Anmol
      phpmyadmin_location: phpmyadmin
      root: /var/www/
```

License
-------
BSD
