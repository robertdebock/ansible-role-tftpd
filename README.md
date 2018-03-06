tftpd
=========

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-tftpd.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-tftpd)

Provides tftpd for your system.

Requirements
------------

Access to a repository providing tftpd.

Role Variables
--------------

- tftpd_tftproot - The directory to use as the tftproot. (default: "/tftproot")

Dependencies
------------

These dependencies can be used to install all requirements.

- robertdebock.bootstrap
- robertdebock.xinetd

Download the dependencies by issuing this command:
```
ansible-galaxy install --role-file requirements.yml
```

Example Playbook
----------------

```
- hosts: servers
  roles:
    - role: robertdebock.bootstrap
    - role: robertdebock.xinetd
    - role: robertdebock.tftpd
```

Install this role using `galaxy install robertdebock.tftpd`.

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
