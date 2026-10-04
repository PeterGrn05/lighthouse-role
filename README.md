Lighthouse-role
=========

Установка Lighthouse и Nginx через Ansible.

Requirements
------------

- Ansible
- Ubuntu

Role Variables
--------------

| Vars                    | Description                                                   |
| ----------------------- | ------------------------------------------------------------- |
| lighthouse_packages     | Packages to use                                               |
| lighthouse_archive_url  | Reference to original repository of Lighthouse                |
| lighthouse_archive_path | Path to Archive                                               |
| lighthouse_root         | Lighthouse root                                               |



Example Playbook
----------------

```yaml

  - name: Установка и настройка Nginx с Lighthouse
  hosts: lighthouse-01
  roles: lighthouse
  become: true
  tags:
    - lighthouse

```

License
-------

MIT

Author Information
------------------

Горин Пётр
