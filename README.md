# Ansible Role: Openssl Root CA

Configure Root CA via openssl

## Requirements

Role requires
 - pexpect module

## Role Variables

All role variables are listed in default/main.yml.

## Dependencies

- pexpect module

## Example Playbook

    - hosts: localhost
      connection: local
      vars_files:
        - vars/main.yml
      roles:
        - { role: ansible-role-openssl-ca }

*Inside `vars/main.yml`*:

    root_ca_dir: /etc/pki/root_ca/
    root_private_key_pass: very-secure-password


## License

MIT / BSD
