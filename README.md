# ansible-role-fail2ban
Ansible role to install fail2ban.

## Description

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `fail2ban_jail_webdav` | false | Deploy webdav jail.  |
| `fail2ban_jail_ssh` | false | Deploy ssh jail.  |

# Testing
```
$ molecule test
```

# Debugging

Prepare instance.
```
$ molecule create
```

Test role against instance.
```
$ molecule converge
```

Inspect instance state.
```
$ molecule login
```

Verify.
```
$ molecule verify
```

Exit then clean.
```
$ molecule destroy
```

# Source

[How to install or upgrade fail2ban manually](https://github.com/fail2ban/fail2ban/wiki/How-to-install-or-upgrade-fail2ban-manually)
