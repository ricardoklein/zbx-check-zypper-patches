ricardoklein.zbx-check-zypper-patches
=========

Simply deploy a cronjob to output the number of pending patches on a openSUSE/SLES box with
a UserParameter (zypper_patches) to allow it to be collected.
 
Requirements
------------

You need to have the zabbix agent installed, try my [zabbix-agent role](https://galaxy.ansible.com/ricardoklein/ansible_zabbix_agent).
This role will not setup Zabbix for you (yet?).

Role Variables
--------------

Everything is setup by defaults/main.yml (you can check there and overrite in your vars).

Dependencies
------------

[zabbix-agent](https://galaxy.ansible.com/ricardoklein/ansible_zabbix_agent) min version 4.0.0

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: ricardoklein.zbx-check-zypper-patches }
```
License
-------

GPL

Author Information
------------------

If you want to suggest changes or request new features, please feel free to create a issue or send a pull request.
