Role Name
=========

An Ansible role to install LightGBM on Ubuntu-based distros.

Requirements
------------

None.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml).

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: modeling
      roles:
        - role: yuriyguts.lightgbm
          lightgbm_enable_gpu_support: no

License
-------

MIT

Author Information
------------------

Yuriy Guts ([https://github.com/YuriyGuts](https://github.com/YuriyGuts)).
