Ansible Varnish BasicAuth VMOD
==============================

Installs the Varnish basic auth VMOD
(https://www.varnish-cache.org/vmod/basicauth).

Tested with Ubuntu 14.04

Requirements
------------

N/A

Role Variables
--------------

Below are the variables used in this role and their defaults:

    varnish_version: 4.0.3
    varnish_basic_auth_vmod_repo: http://git.gnu.org.ua/cgit/vmod-basicauth.git

The varnish_version is used to compile the vmod, so it must match the
version of varnish you will be running.

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: varnish
      roles:
         - { role: mnn.varnish-basicauth, varnish_version: 4.0.3 }

License
-------

GPLv3

Author Information
------------------

Written by Justin Caratzas <bigjust@lambdaphil.es> for Mother Nature Network.
