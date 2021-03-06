ansible_role_zabbix_proc_mem

=========

Installs the zabbix agent process memory scripts

Galaxy link
------------

https://galaxy.ansible.com/kaihei777/ansible-role-zabbix-proc-mem/

Requirements
------------

- dj-wasabi.zabbix-agent

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Custom Zabbix Scripts
--------------

Define these variables to copy scripts to your respective scripts path.

* `zabbix_agent_externalscriptspath`: List of externalscripts to be added to `zabbix_agent_externalscriptspath`

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
        # ansible_role_zabbix_proc_mem
        zabbix_agent_externalscriptspath: /usr/lib/zabbix/externalscripts
        # dj-wasabi.zabbix-agent
        zabbix_agent_userparameters:
          - name: proc_mem
      roles:
         - { role: kaihei777.ansible_role_zabbix_proc_mem }

Example Zabbix Custom Template
----------------

See. 
[Sample Zabbix Custom Template](sample/zabbix/Custom_Template_Proc_memory.xml)


License
-------

MIT / BSD

Author Information
------------------

This role was created in 2020 by Kaihei Sameshima.
