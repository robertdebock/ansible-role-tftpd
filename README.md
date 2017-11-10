Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

- tftproot - The directory to use as the tftproot. (default: "/tftproot")

Dependencies
------------

- robertdebock.bootstrap
- robertdebock.xinetd

Example Playbook
----------------

```
- hosts: servers
  roles:
    - robertdebock.xinetd
```

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
