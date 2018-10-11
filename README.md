Role Name
=========

Couchdb role to setup either standalone couchdb server or multinode couchdb cluster.

Requirements
------------

There is no dependency for this role. It use apt to install couchdb so no additional requirements.

Role Variables
--------------

This role is very straight forward. So, not many user inputs are needed. Still you can override the value of the following variables -

```
cluster_setup: True
admin_password: "superpass"
cluster_cookie: "supersecret"
```

Dependencies
------------

No dependency on any other role.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
     - role: couchdb
       cluster_setup: true
```

Inventory file should be like this -

```
[couchdb]
192.168.0.1
192.168.0.2
192.168.0.3
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
