emo app role
============

This role installs and configures the EMO app.

Requirements
------------

None.

Role Variables
--------------

EMO app will run under it's own user. The UID and GIDs are defined by:

```yaml
emo_app_uid: 888
emo_app_gid: 888
```

The name and path of the app can easily be changed via:

```yaml
emo_app_name: 'emo_app'
emo_app_path: '/opt/{{ emo_app_name }}'
```

To modify the repository and/or the installed version overwrite the following defaults:

```yaml
emo_app_repo: https://github.com/domibarton/emo-app.git
emo_app_version: master
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - emo_app

License
-------

MIT

Author Information
------------------

confirm IT solutions, dbarton
