# Ansible Role: Cumulus out-of-band

This role will setup an out-of-band server for provisioning of Cumulus Linux switches.

Naturalis uses this role together with a private inventory.

## Role Variables

Available variables are listed below, along with default values:

An example would be:

```bash
admin_users:
  - username: admin-user
    public_key: AAAAB3J
oob_server: 192.168.0.1
oob_user: testuser
oob_subnet: 192.168.0.0
oob_range: 192.168.0.100 192.168.0.254
oob_name_servers:
  - 192.168.0.1
  - 1.1.1.1
license: test-license
oob_hosts:
oob_dhcp_interface: enp3s0
```

## Example Playbook

    - hosts: oob-server
      roles:
        - ansible-cumulus-oob

## License

Apache2
