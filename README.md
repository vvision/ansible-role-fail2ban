# ansible-role-fail2ban

[![CI](https://github.com/vvision/ansible-role-fail2ban/workflows/CI/badge.svg?event=push)](https://github.com/vvision/ansible-role-fail2ban/actions?query=workflow%3ACI)

Installs fail2ban on Debian servers.

## Requirements

## Role Variables

    fail2ban_deb_url: https://github.com/fail2ban/fail2ban/releases/download/0.11.2/fail2ban_0.11.2-1.upstream1_all.deb
    
Fail2ban debian package url. Role will expect an acs file at ``fail2ban_deb_url`` + ``.asc``.

    fail2ban_keyserver_url: hkps://keyserver.ubuntu.com

Key server to use when checking package signature.

### Default Jail configuration

    fail2ban_ignoreip: "127.0.0.1/8"

Space separated list of IPs to ignore.
"ignoreip" can be an IP address, a CIDR mask or a DNS host.

    fail2ban_bantime: 3600

Default ban time for all jails.

    fail2ban_maxretry: 3

Default max retry for all jails.

### Jails configuration

    fail2ban_activate_ssh_jail: false

Whether to activate ssh jail.

    fail2ban_ssh_jail_bantime: 86400

Ban time for ssh jail.

## Dependencies

None.

## License

MIT

## Author Information

This role was created in 2021 by Victor Voisin.
