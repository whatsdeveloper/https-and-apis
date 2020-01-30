# HTTP/HTTPS and APIs

## Hypertext Transfer Protocol (Secure)

```
            userinfo          host        port
        ┌───────┴───────┐ ┌────┴────────┐ ┌┴┐
 http://john.doe:password@www.example.com:123/forum/questions/?tag=networking&order=newest#top
 └─┬─┘ └───────────┬────────────────────────┘└─┬─────────────┘└────────┬──────────────────┘└┬─┘
 scheme         authority                      path                  query             fragment
```

### Status codes

- Informational `1XX`
- Successful `2XX`
- Redirection `3XX`
- Client Error `4XX`
- Server Error `5XX`

### Example

- **Client request**

```
GET / HTTP/1.1
Host: www.example.com
```

- **Server response**

```
HTTP/1.1 200 OK
Date: Mon, 23 May 2005 22:38:34 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 138
Last-Modified: Wed, 08 Jan 2003 23:11:55 GMT
Server: Apache/1.3.3.7 (Unix) (Red-Hat/Linux)
ETag: "3f80f-1b6-3e1cb03b"
Accept-Ranges: bytes
Connection: close

<html>
  <head>
    <title>An Example Page</title>
  </head>
  <body>
    <p>Hello World, this is a very simple HTML document.</p>
  </body>
</html>
```

## APIs

![](img/API-page-graphic.png)

- **Private**: The API is only for use internally. This gives companies the most control over their API.
- **Partner**: The API is shared with specific business partners. This can provide additional revenue streams without compromising quality.
- **Public**: The API is available to everyone. This allows third parties to develop apps that interact with your API and can be a source for innovation.

![](img/How-To-Change-From-HTTP-To-HTTPS.png)
