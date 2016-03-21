apt role
========

This role configures apt, Debian's package manager.

It will also support the update of the cache and the upgrade of the system packages.

Requirements
------------

None.

Role Variables
--------------

By default the role will update the package cache, but will not touch the system packages itself.
However, you can overwrite that behaviour by setting:

```yaml
apt_update: yes
apt_upgrade: no
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - apt

License
-------

MIT

Author Information
------------------

confirm IT solutions, dbarton
