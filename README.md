tftpd
=========

Provides tftpd

Requirements
------------

Access to a repository providing tftpd.

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
    - robertdebock.tftpd
```

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
