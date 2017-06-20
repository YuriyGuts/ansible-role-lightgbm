yuriyguts.lightgbm
==================

An Ansible role to install LightGBM on Ubuntu-based distros.

Requirements
------------

Note:

* If the target environment requires running `pip` with elevated privileges,
  make sure to set `lightgbm_python_package_manager_become: yes` in your playbook.

* Due to possible issues with `libgomp.so` dependencies when using Anaconda,
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
