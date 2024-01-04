packages
========

Install packages and configure your editor as the editor alternative.

Role Variables
--------------

| Name          | Comment                              | Default value |
|---------------|--------------------------------------|---------------|
| packages_site  | A list of packages which will be installed on all machines | `[]`          |
| packages_server | A list of packages which will be installed only on machines in the server host group | `[]`          |
| packages_client | A list of packages which will be installed only on machines in the client host group | `[]`          |
| packages_editor | A list of packages which will be installed only on machines in the client host group | `/usr/bin/vim`          |

Example Playbook
----------------
```yaml
- name: Install basic packages
  hosts: all
  collections:
    - oxivanisher.linux_base
  roles:
    - role: oxivanisher.linux_base.packages
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
