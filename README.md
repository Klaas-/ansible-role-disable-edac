Ansible Role: Disable EDAC
=========

[![Build Status](https://travis-ci.org/Klaas-/ansible-role-disable-edac.svg?branch=master)](https://travis-ci.org/Klaas-/ansible-role-disable-edac)

This role is designed to disable EDAC related modules.

A lot of hardware vendors force/recommend disabling EDAC because it interferes with their own monitoring.
* [Lenovo](https://support.lenovo.com/de/en/solutions/ht107942)
* [Dell](https://www.dell.com/support/article/us/en/04/sln28338A9/edac-errors-in-messages-log-in-redhat-enterprise-linux-rhel-and-poweredge)
* [HP](https://support.hpe.com/hpsc/doc/public/display?docId=emr_na-a00016026en_us)


Requirements
------------

Ansible 1.4+

Role Variables
--------------

These are the variables that can be passed to the role:

    edac_modules: [ 'moduleNames', ... ]

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - ansible-role-disable-edac

License
-------

GPLv3

Author Information
------------------

[Klaas Demter](https://github.com/Klaas-/)
