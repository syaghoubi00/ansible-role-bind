# Bind

An Ansible role to install [Bind9](https://www.isc.org/bind/) ([Gitlab](https://gitlab.isc.org/isc-projects/bind9))

## Platforms

- RHEL 9

## Requirements

None.

## Role Variables

`bind_config_file:` - Path to a custom `named.conf`

`bind9_zones_dir:` - Path to a directory containing zone files

## Dependencies

`ansible.posix.firewalld`: For opening the CoreDNS port with `firewalld`

## Example Playbook

```yaml
- hosts: dns_servers
  roles:
    - syaghoubi00.bind
```

## License

GPL-3.0-or-later

## Author Information

Created by Sebastian Yaghoubi
