ansible-psql
============

[![Build Status](https://travis-ci.org/k0st1an/ansible-psql.svg?branch=master)](https://travis-ci.org/k0st1an/ansible-psql) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-k0st1an.psql-blue.svg?style=flat)](https://galaxy.ansible.com/k0st1an/psql/)

Deploy PostgreSQL.


Tested
------

  - Debian Jessie
  - ansible v1.9.1


Synopsis
--------

  - Install PostgreSQL
  - Create user (optional, default is disable)
  - Remote access for user (optional, default is disable)


Role Variables
--------------

You can see all variable of role in file `default/main.yml`.


Project structure
-----------------

Create directories:


    ├── defaults
    │   └── main.yml
    ├── files
    │   ├── pg_hba-9.4.conf.orig
    │   └── postgresql-9.4.conf.orig
    ├── handlers
    │   └── main.yml
    ├── LICENSE
    ├── meta
    │   └── main.yml
    ├── README.md
    ├── tasks
    │   ├── configuration.yml
    │   ├── install.yml
    │   ├── main.yml
    │   ├── preparation.yml
    │   └── user.yml
    └── templates
        └── pg_hba.conf.j2


License
-------

MIT

Author Information
------------------

  - Author: Konstantin Kruglov
  - GitHub: https://github.com/k0st1an
  - Contact: kruglovk@gmain.com
