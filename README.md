andrewrothstein.cassandra-cluster
=========================
![Build Status](https://github.com/andrewrothstein/ansible-cassandra-cluster/actions/workflows/build.yml/badge.svg)

Installs and configures a cassandra cluster.

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
	  cassandra_network_iface: eth0
	  cassandra_seeds:
	    ty: group
		name: cassandra-cluster
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
