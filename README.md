# Role ansible_galaxy_role.motd

The role will setup a motd message.

On Red Hat and old Debian systems the motd is a text file that will be copied as 
/etc/motd.d/99-homeco and /etc/issue.net respectively.

On newer Debian systems v.9 and later that support dynamic motd the message file
is executable shell script /etc/update-motd.d/99-homeco

## Requirements
Tested on:
* Debian 8 and up
* Ubuntu
* Red Hat and CentOS

## Role Variables
*None*

## Example Playbook

```yaml
- name: PlaybookName
  hosts: all
  roles:
    - role: ansible_galaxy_role.motd
```
