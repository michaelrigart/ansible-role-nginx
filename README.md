Ansible Nginx Role
==================
[![Build Status](https://travis-ci.org/michaelrigart/ansible-role-nginx.svg?branch=master)](https://travis-ci.org/michaelrigart/ansible-role-nginx)

An ansible role for installing and configuring Nginx from a PPA.

Role Variables
--------------

```yaml
nginx_ppa: the ppa you want to use
nginx_package: name of the nginx package you want to install
nginx_path: path of the nginx installation
nginx_service_state: state for the nginx service
nginx_service_enabled: indicate if you want the nginx service enabled
nginx_config: dictionary that holds the nginx configuration
```

View the default vars - defaults/main.yml - for a more detailed example.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: MichaelRigart.nginx, sudo: Yes }
```

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>