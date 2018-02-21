ansible-role-cfg-snmpd
======================
## Vars
* TODO

## Example Playbook

```
---
- hosts: all
  remote_user: user
  become: yes
  become_method: sudo
  vars:
      snmpd_communities: 
          - name: 'public'
            type: 'ro'
            hosts: 
                - '192.168.1.0/24'
      snmpd_location: 'Example IL'
      snmpd_syscontact: 'root@example.com'
  roles:
        - ansible-role-snmpd
```
