# DNS

## Hosts File

Browsers usually first look up records in the local `/etc/hosts` file, only contacting a DNS server when the record doesn't exist there.

## Encrypted DNS Servers

A clear-text DNS server may still reveal the visited URL of a request to an attacker. Using an encrypted DNS server (e.g. `8.8.8.8` or `1.1.1.1`) can resolve this issue.