tftpd
=========

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-tftpd.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-tftpd)

Provides tftpd for your system.

Context
-------
This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://robertdebock.nl/) for further information.

Here is an overview of related roles:
![dependencies](https://raw.githubusercontent.com/robertdebock/drawings/artifacts/tftpd.png "Dependency")

Requirements
------------

Access to a repository providing tftpd.

Role Variables
--------------

- tftpd_tftproot - The directory to use as the tftproot. (default: "/tftproot")

Dependencies
------------

These dependencies can be used to install all requirements.

- [robertdebock.bootstrap](https://travis-ci.org/robertdebock/ansible-role-bootstrap)
- [robertdebock.xinetd](https://travis-ci.org/robertdebock/ansible-role-xinetd) (This is a hard dependency, because this role depends on a handler defined in the xinetd role.

Download the dependencies by issuing this command:
```
ansible-galaxy install --role-file requirements.yml
```

Compatibility
-------------

This role has been tested against the following distributions and Ansible version:

|distribution|ansible 2.3|ansible 2.4|ansible 2.5|
|------------|-----------|-----------|-----------|
|alpine-latest|no|no|no|
|alpine-edge|no|no|no|
|archlinux|yes|yes|yes|
|centos-6|yes|yes|yes|
|centos-latest|yes|yes|yes|
|debian-stable|yes|yes|yes|
|debian-latest|yes|yes|yes|
|debian-wheezy|yes|yes|yes|
|fedora-latest|yes|yes|yes|
|fedora-rawhide|yes|yes|yes|
|opensuse-leap|yes|yes|yes|
|opensuse-tumbleweed|yes|yes|yes|
|ubuntu-artful|yes|yes|yes|
|ubuntu-latest|yes|yes|yes|

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

Robert de Bock](https://robertdebock.nl/) <robert@meinit.nl>
