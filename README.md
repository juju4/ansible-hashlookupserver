[![Actions Status - Master](https://github.com/juju4/ansible-hashlookupserver/workflows/AnsibleCI/badge.svg)](https://github.com/juju4/ansible-adduser/actions?query=branch%3Amaster)
[![Actions Status - Devel](https://github.com/juju4/ansible-hashlookupserver/workflows/AnsibleCI/badge.svg?branch=devel)](https://github.com/juju4/ansible-adduser/actions?query=branch%3Adevel)

# hashlookupserver ansible role

Setup https://github.com/adulau/hashlookup-server

## Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 2.11

### Operating systems

Tested on Ubuntu 18.04, 20.04, Centos 7 and 8.

## Example Playbook

Just include this role in your list.
For example

```
- host: myhost
  roles:
    - juju4.hashlookupserver
```

you probably want to review variables

## Variables

TBD

## Continuous integration

```
$ pip install molecule docker
$ molecule test
$ MOLECULE_DISTRO=ubuntu:20.04 molecule test --destroy=never
```


## Troubleshooting & Known issues

* NSRL uncompress in python may fail on MemoryError. If happens, just do it manually.

## License

BSD 2-clause
