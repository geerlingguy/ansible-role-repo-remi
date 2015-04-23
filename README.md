# Ansible Role: Remi Repository

Installs the Remi repository (Les RPM de Remi) for RHEL/CentOS 6.x.

## Requirements

None.

## Role Variables

None.

## Dependencies

* geerlingguy.repo-epel

## Example Playbook

    - hosts: servers
      roles:
        - { role: geerlingguy.repo-remi }

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
