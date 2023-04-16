joenyland.samba
=========================

[![CI](https://github.com/JoeNyland/ansible-samba-role/actions/workflows/ci.yml/badge.svg)](https://github.com/JoeNyland/ansible-samba-role/actions/workflows/ci.yml)

Installs and configures Samba.

Requirements
------------

None.

Role Variables
--------------

### `samba_shares`

A hash of shares to export.

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: server
  roles:
    - role: joenyland.samba
      vars:
        samba_shares:
          tank:
            path: /tank
            valid_users: john
            read_only: false
```

License
-------

MIT

Author Information
------------------

⌨️ with ❤️ by [Joe Nyland](https://joe.nyland.io)
