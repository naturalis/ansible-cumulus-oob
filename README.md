# Ansible Role: Cumulus out-of-band

This role will setup an out-of-band server for provisioning of Cumulus Linux switches.

Naturalis uses this role together with a private inventory.

## Requirements


## Role Variables

Available variables are listed below, along with default values:

An example would be:

```bash
oob_server: 192.168.144.5
oob_user: vault-aanmaken
oob_subnet: 192.168.144.0
oob_range: 192.168.144.100 192.168.144.254
license: vault-aanmaken
users: vault-aanmaken
authorized_keys: vault-aanmaken
oob_hosts: vault-aanmaken
```

## Dependencies


## Example Playbook

    - hosts: oob-server
      roles:
        - ansible-cumulus-oob

## License

Apache2
