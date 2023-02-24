![Ansible Lint](https://github.com/johanneskastl/ansible-role-set_timezone/workflows/Ansible%20Lint/badge.svg)

set_timezone
=========

Set the timezone in /etc/localtime

Requirements
------------

None.

Role Variables
--------------

- `desired_timezone`: (String) The desired timezone, e.g. `Europe/Berlin`. Defaults to `Etc/UTC`.

Dependencies
------------

None

Example Playbook (using the default of Etc/UTC)
----------------

    - hosts: servers
      roles:
        - role: 'johanneskastl.set_timezone'

Example Playbook for timezone "Europe/Berlin"
----------------

    - hosts: servers
      roles:
        - role: 'johanneskastl.set_timezone'
          desired_timezone: 'Europe/Berlin'

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
