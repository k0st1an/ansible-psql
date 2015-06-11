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


License
-------

MIT

Author Information
------------------

GitHub: https://github.com/k0st1an

Author: Konstantin Kruglov

Contact: kruglovk@gmain.com
