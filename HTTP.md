# HyperText Transfer Protocol

## Port

Default port: 80
- When using HTTPS, a request to port `80` will be redirected through a `301 Moved Permanently` response to port `443`

## Abbreviations

- FQDN: Fully Qualified Domain Name
- URL: Uniform Resource Locator

## URL Structure

ex: http://admin:password@inlanefreight.com:80/dashboard.php?login=true#status
- "http://": Scheme
- "admin:password": User
- "inlanefreight.com": Host
- "80": Port
- "dashboard.php": Path
- "?login=true": Query String
- "#status": Fragment

## HTTPS

- Client Hello
- Server Hello
- Key exchange to exchange SSL certificates
- Encrypted handshake to confirm whether encryption and transfer are working
- Encrypted HTTP communication