yuriyguts.lightgbm
==================

An Ansible role to install LightGBM on Ubuntu-based distros.

Requirements
------------

This role assumes that the user on the target system can install Python packages without `sudo`.
If this is not the case, add `become: yes` to the role parameters in your playbook.

**Note**: Due to possible issues with `libgomp.so` dependencies when using Anaconda,
the role adds `anaconda` to the list of channels and upgrades the `libgcc` package 
to the latest version.

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
