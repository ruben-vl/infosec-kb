# Client URL

Command-line tool that supports HTTP along with many other protocols.

## Basic GET request

```bash
curl inlanefreight.com
```

## Download Response

Flag `-O` can be used to download the response with the remote file name. Flag `-o` can be used to download it and specify the file name.

## Silent

Flag `-s` can be used to silence the printing of status messages from cURL.

## Skip Certificate Check

Flag `-k` can be used to skip the certificate check. Only use this for testing a local web application or for practice purposes.

## Verbose

Flag `-v` can be used to print both the request and response. The `-vvv` flag shows even more verbose output.

## Showing Headers

Flag `-I` is used to only display the response headers through a HEAD request. Flag `-i` is used to display both the headers and the response body.

## Setting Headers

Request headers can be set using the `-H` flag. The flag `-A` can be used to set the User-Agent header specifically.

## HTTP Basic Auth Credentials

To provide credentials through cURL, the `-u` flag can be used, with `user:password` as the argument. The credentials can also be put directly in the url, in between the scheme and host. A third way is by directly setting the Authorization header with the `-H` flag.

## Other Request Methods

The flag `-X` can be used with the method as an argument. To add e.g. POST data, the `-d` flag is used.

## Follow Redirection

The flag `-L` is used to follow redirection.

## Setting Cookies

A cookie can be set using the `-b` flag, e.g.

```bash
curl -b 'PHPSESSID=c1nsa6op7vtk7kdis7bcnbadf1' http://<SERVER_IP>:<PORT>/
```

or by specifying the Cookie header, e.g.

```bash
curl -H 'Cookie: PHPSESSID=c1nsa6op7vtk7kdis7bcnbadf1' http://<SERVER_IP>:<PORT>/
```

