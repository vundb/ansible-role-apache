Ansible Role Apache
======================================

Ansible role to install and configure apache on gentoo instances.

Supported Distributions
-----------------------

- Gentoo

Role Variables
--------------

- `apache_services`:
Array with services to be restarted on configuration changes.

- `apache_user`:
System user name for apache daemon. Default value is `apache`.

- `apache_group`:
System user group for apache daemon. Default value is `apache`.

- `apache_port`:
Default port to listen on.

- `apache_opts`:
Apache options to be used for configuration files. Available values are
`["PHP", "PASSENGER"]`.

Dependencies
------------

None.

Example Playbook
----------------
```
- hosts: all
  roles:
    - role: vundb-apache
      apache_opts: ["PHP"]
```

License
-------

MIT

Author Information
------------------

- You can find more roles in my GitHub channel [vundb](https://github.com/vundb)
- Follow me on Twitter [@vundb](https://twitter.com/vundb)
