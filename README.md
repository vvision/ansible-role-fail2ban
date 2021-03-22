# ansible-role-fail2ban
Ansible role to install fail2ban.

## Description

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `fail2ban_jail_apache` | false | Deploy apache jails. |
| `fail2ban_jail_wordpress` | false | Deploy wordpress jails. |
| `fail2ban_jail_shaarli` | false | Deploy Shaarli jail. |
| `fail2ban_jail_webdav` | false | Deploy webdav jail.  |

## TODO

https://github.com/fail2ban/fail2ban/wiki/How-to-install-or-upgrade-fail2ban-manually
