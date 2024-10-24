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

## HTTP Requests and Responses

Request example:
```http
GET /users/login.html HTTP/1.1
```
- "GET": HTTP Method
- "/users/login.html": Path
- "HTTP/1.1": HTTP Version

After this, headers can be given, separated by newlines.
Finally, a request may end with a request body and data.

Response example:
```http
HTTP/1.1 200 OK
```
- "HTTP/1.1": HTTP Version
- "200 OK": Response Code

## HTTP 2.X

HTTP version 1.X sends requests as clear-text, and uses a new-line character to separate different fields and different requests. HTTP version 2.X, on the other hand, sends requests as binary data in a dictionary form.

## HTTPS

- Client Hello
- Server Hello
- Key exchange to exchange SSL certificates
- Encrypted handshake to confirm whether encryption and transfer are working
- Encrypted HTTP communication

## HTTP Downgrade Attack

Downgrades HTTPS to HTTP, making the data transferred clear-text. This is done by setting up a Man-in-the-Middle (MitM) proxy to transfer all traffic through the attacker's host without the user's knowledge.