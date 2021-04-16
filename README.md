# Ansible Role: Darktable

[![CI](https://github.com/pmikus/ansible-role-darktable/actions/workflows/CI.yml/badge.svg)](https://github.com/pmikus/ansible-role-darktable/actions/workflows/CI.yml)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-darktable&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-darktable)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-darktable&metric=bugs)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-darktable)

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    darktable_package: "darktable"

Name of package in package repository.

    opensuse_url: "http://download.opensuse.org/repositories/graphics"

OpenSuse repository is used as per [Darktable/install](https://www.darktable.org/install/).

    darktable_package_state: "present"

Install package (optionally you can change to "absent" to uninstall).

    darktable_apt_key: "3247B7519EDBEAB422E900A3040524A84C70D8B5"

APT GPG key.

    darktable_apt_key_state: "present"

Install APT GPG key (optionally you can change to "absent" to roll back).

    darktable_apt_state: "present"

Install APT repository (optionally you can change to "absent" to roll back).

## Dependencies

None

## Example Playbook

    - hosts: localhost
      roles:
        - pmikus.ansible-role-darktable

## License

MIT / BSD

## Author Information

This role was created by [Peter Mikus](https://www.linkedin.com/in/petermikus/).
