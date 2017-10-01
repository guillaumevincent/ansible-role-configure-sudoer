Configure sudoer
================

 * create sudoer
 * add public keys for sudoer 

Role Variables
--------------

 * sudoer (default: admin)
 * sudoer_public_keys (default: ['~/.ssh/id_rsa.pub'])

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: guillaumevincent.configure-ssh, sudoer: 'admin', sudoer_public_keys: ['~/.ssh/id_rsa.pub'] }

License
-------

MIT
