ansible-psql
============

Deploy PostgreSQL latest version.

Tested
------

  - Debian Jessie
  - ansible v1.9.1

Synopsis
--------

  - Install PostgreSQL
  - Create super user (optional)


Role Variables
--------------

Content of the `vars/main.yml`:

```yaml
psql_remote_access            : yes
psql_remote_user              : engineer
psql_remote_pass              : SOMEPASSWORD
psql_remote_db                : engineer
psql_remote_host              : 0.0.0.0/0
```

Usage (example)
---------------

Create directories:

  /dir/
     |--roles\
     |      |--psql
     |           |--files of this role
     |--hosts
     |--psql.yml


Contents of the `hosts`:

```
[psql]
a.b.c.d
```

Contents of the `psql.yml`:

```yaml
---
- hosts: psql
  remote_user: root

  roles:
    - psql
```

And launch playbook:

    $ ansible-playbook -i hosts psql.yml



License
-------

MIT

Author Information
------------------

  - Author: Konstantin Kruglov
  - GitHub: https://github.com/k0st1an
  - Contact: kruglovk@gmain.com
