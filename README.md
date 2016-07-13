ansible-psql
============

[![Build Status](https://travis-ci.org/k0st1an/ansible-psql.svg?branch=master)](https://travis-ci.org/k0st1an/ansible-psql) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-k0st1an.psql-blue.svg?style=flat)](https://galaxy.ansible.com/k0st1an/psql/)

Deploy PostgreSQL.


Role Variables
--------------

You can see all variable of role in file `default/main.yml`. Simple example some vars:

    psql_users:
      - name: k0st1an
        pass: 42

    psql_dbs:
      - name: k0st1an
        owner: k0st1an

    psql_user_priv:
      - name: k0st1an
        db: k0st1an
        flags: "LOGIN"

    psql_hba:
      - type: 'local'
        db: 'all'
        user: 'postgres'
        address: ''
        method: 'peer'
      - type: hostssl
        db: k0st1an
        user: k0st1an
        address: localhost
        method: md5

License
-------

MIT

Author Information
------------------

  - Author: Konstantin Kruglov
  - GitHub: https://github.com/k0st1an
  - Contact: kruglovk@gmain.com
