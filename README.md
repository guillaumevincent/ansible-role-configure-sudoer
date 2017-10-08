# ansible-role-sudoer

 * create sudoer
 * add public keys for sudoer 

## Role Variables

 * sudoer (default: `admin`)
 * sudoer_public_keys (default: `['~/.ssh/id_rsa.pub']`)

## Example Playbook

    - hosts: all
      roles:
         - { role: guillaumevincent.configure-sudoer, sudoer: 'admin', sudoer_public_keys: ['~/.ssh/id_rsa.pub'] }

## License

MIT
