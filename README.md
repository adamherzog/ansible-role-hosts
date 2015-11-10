hosts
=====

Configure /etc/hosts.

Role Variables
--------------

 * hosts_entries: []

    Specifies the hosts and aliases to setup.

Example Playbook
----------------

    - hosts: servers
      vars:
        hosts_entres:
          - name: www.domain.com
            ip: 1.2.3.4
            aliases: [ www ]
      roles:
         - hosts

License
-------

BSD

Author Information
------------------

Adam Herzog <adam@adamherzog.com>
Heavily based on https://github.com/bertvv/ansible-role-hosts
