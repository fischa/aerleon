# Service Files

Service files define symbolic names for services, commonly udp/tcp ports. Policy files may reference these names.

```yaml
terms:
  - name: accept-ssh-requests
    source-address: INTERNAL
    destination-port: SSH
    protocol: tcp
    counter: ssh
    action: accept
```

## YAML

```yaml
services:
  WHOIS:
    - port: 43
      protocol: udp
  SSH:
    - port: 22
      protocol: tcp
  TELNET:
    - port: 23
      protocol: tcp
  SMTP:
    - port: 25
      protocol: tcp
  MAIL_SERVICES:
    - name: SMTP
    - name: ESMTP
    - name: SMTP_SSL
    - name: POP_SSL
```

## *.svc

```text
WHOIS = 43/udp
SSH = 22/tcp
TELNET = 23/tcp
SMTP = 25/tcp
MAIL_SERVICES = SMTP
                ESMTP
                SMTP_SSL
                POP_SSL
...skipped...
```

Users may wish to auto-generate address book files to keep them up to date. JSON and CSV are accepted for this reason.
