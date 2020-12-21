Role Name
=========

Hopla.cloud role for ansible to install a simple mariadb.

Requirements
------------

None.

Role Variables
--------------


mysql_packages:
  - mariadb-client
  - mariadb-server
mysql_root_username: root
mysql_root_password:

Dependencies
------------

- hoplacloud.linux_update
- hoplacloud.linux_motd
- hoplacloud.fail2ban
- hoplacloud.postfix
- geerlingguy.mysql


Example Playbook
----------------

    - hosts: localhost
      remote_user: root
      roles:
         - hoplacloud.mariadb

License
-------

GPLv3

Author Information
------------------

Joffrey Skandera for [hopla.cloud](https://hopla.cloud)
