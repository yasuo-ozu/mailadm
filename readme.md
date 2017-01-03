# mailadm - mail account admin tool for Postfix + Dovecot + CyrusSASL

## Premise

- Virtual domain
- Using Maildir (instead of Mailbox)
- Postfix (virtual\_mailbox\_maps = hash:/etc/postfix/vmailbox)
- CyrusSASL (pwcheck\_method = auxprop, using /etc/sasldb2)
- Dovecot (auth-passwdfile.conf.ext, driver = passwd-file, using /etc/dovecot/users)

## Usage

```
mailadm add name@domain.tld
mailadm list
mailadm list domain.tld
mailadm remove name@domain.tld
```

## Notice

This script is really depends on GNU Bash, sed, etc.
