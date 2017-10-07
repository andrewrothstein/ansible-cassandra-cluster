andrewrothstein.cassandra
=========================
[![Build Status](https://travis-ci.org/andrewrothstein/ansible-cassandra-cluster.svg?branch=master)](https://travis-ci.org/andrewrothstein/ansible-cassandra-cluster)

Installs and configures a cassandra cluster

Requirements
------------

See [meta/main.yml](meta/main.yml)

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

See [meta/main.yml](meta/main.yml)

Example Inventory
-----------------

```ini
[cassandra-cluster]
host[1-n].test
```

Example Playbook
----------------

```yml
- hosts: cassandra-cluster
  roles:
    - role: andrewrothstein.cassandra
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
