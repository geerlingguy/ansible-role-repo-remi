# Ansible Role: Remi Repository

[![CI](https://github.com/geerlingguy/ansible-role-repo-remi/workflows/CI/badge.svg?event=push)](https://github.com/geerlingguy/ansible-role-repo-remi/actions?query=workflow%3ACI)

Installs [Remi's RPM repository](http://rpms.famillecollet.com/) for RHEL/CentOS.

## Requirements

On RHEL 8 or newer, you should make sure to install or enable the EPEL repository. I recommend using the `geerlingguy.repo-epel` repository.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    remi_repo_url: "https://rpms.remirepo.net/enterprise/remi-release-{{ ansible_distribution_major_version }}.rpm"

The URL from which the Remi repo `.rpm` will be downloaded and installed.

    remi_repo_gpg_key_url: "https://rpms.remirepo.net/enterprise/{{ ansible_distribution_major_version }}/RPM-GPG-KEY-remi"

Remi repo GPG key location. Can be set to a local file or to the URL from Remi's website.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - geerlingguy.repo-remi

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
