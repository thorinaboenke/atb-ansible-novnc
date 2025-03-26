Ansible role to install NoVNC
=============================

This role installs novnc with x11vnc and websockify.
Optionally a user specific x11vnc session can be started on Display :1 with create_user_session = true.

Requirements
------------

A debian based linux distribution

Role Variables
--------------

```yaml
novnc_packages:
  - websockify
  - x11vnc
  - novnc
create_user_session: false
vnc_user: ""
vnc_password: ""
```

Dependencies
------------

No dependencies

Example Playbook
----------------

The following playbook installs the novnc-role:

```yaml
    - hosts: servers
      roles:
         - role: novnc
```

License
-------

GPL-3.0

Author Information
------------------

Wolfgang Hotwagner
