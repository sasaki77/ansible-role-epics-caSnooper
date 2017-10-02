# Ansible Role: EPICS csSnooper

Installs EPICS csSnooper on RHEL/CentOS.

## Requirements

- ansible >= 2.3

## Role Variables
Refer to `defaults/main.yml` in detail.
```
epics_casnooper_extension: 
  url: "https://www.aps.anl.gov/epics/download/extensions/caSnooper2_1_2_3.tar.gz"
  unarchived_name: "caSnooper2_1_2_3"
  release: false
```

## Dependencies

- [ansible-role-epics-base](https://github.com/sasaki77/ansible-role-epics-base)

## Example Playbook
```
- hosts: epics-base
  roles:
    - role: ansible-role-epics-base
    - role: ansible-role-epics-csSnooper
```

## License

None.

## Author Information

This role was created by Shinya Sasaki.
