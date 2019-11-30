# Web Cheat Sheet

[:arrow_backward: Algebra / Web Designer / Module 1 - Introduction To Web Design and Image Manipulation](./)

---

**How the web works**

1. The client requests data from the server at a specified resource.
2. The server receives and processes the request.
3. The server responds to the client with the processed result.

The requests are commonly done via HTTP or HTTPS protocols.

A request contains request headers and may contain a request body in the case of `POST`, `PUT`, and `PATCH` requests.

A response contains response headers and may contain a response body.

Example general headers:

```
Request URL: https://www.google.com/
Request Method: GET
Status Code: 200 
Remote Address: 172.217.20.4:443
Referrer Policy: no-referrer-when-downgrade
```

Example response headers:

```
cache-control: private, max-age=0
content-encoding: br
content-length: 66255
content-type: text/html; charset=UTF-8
date: Sun, 03 Nov 2019 08:41:59 GMT
set-cookie: ...
status: 200
```

Example request headers:

```
accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
accept-encoding: gzip, deflate, br
accept-language: hr,en-US;q=0.9,en;q=0.8,en-GB;q=0.7
cookie: ...
user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.70 Safari/537.36
```

**Common request methods**

* `GET` - _"Retrieve data from the server at the specified resource."_
* `POST` - _"Send data to the server at the specified resource."_
* `PATCH` - _"Send data to the server to partially modify the specified resource."_
* `PUT` - _"Send data to the server to create or update a specified resource."_
* `DELETE` - _"Delete specified resource."_
* `HEAD` - Same as `GET`, but without the response body.
* `OPTIONS` - _"Retrieve data from the server about methods and operations the server supports."_

**The difference between `POST`, `PUT`, and `PATCH`**

* `POST` - Non-idempotent. Implies creating or modifying a resource using sent data with possible side effects.
* `PUT` - Idempotent. Implies creating or replacing a resource using sent data without side effects.
* `PATCH` - Non-idempotent. Implies partially modifying a resource using set data with possible side effects.

> _Idempotent_ - making the same request once or several times successively has the same effect (no side effect).
>
> _Non-idempotent_ - making the same request once or several times may have additional side effects.

**HTTP status code groups**

* `1xx` - Request status.
* `2xx` - Request was successful.
* `3xx` - Request was redirected.
* `4xx` - Client error (e.g. invalid request).
* `5xx` - Server error (e.g. unavailable resource).

**Common HTTP status codes**

* `200 OK` - The request has succeeded.
* `201 Created` - The request has succeeded and a new resource was created.
* `301 Moved Permantently` - The requested resource has a new permanent URI.
* `400 Bad Request` - The request could not be processed by the server because of a client error.
* `401 Unauthorized` - The request requires user authentication.
* `403 Forbidden` - The server refuses to fulfill the request.
* `404 Not Found` - The server cannot find a resource matching the requested URI.
* `500 Internal Server Error` - The request could not be processed because of a server error.

**URL structure**

`https://google.com/search?q=algebra#results`

* `https://` - Scheme / Protocol. Examples: `http`, `https`, `ftp`, `mailto`, `tel`.
* `google.com` - Authority. Examples: `google.com`, `user@server.net`, `cpanel.myhosting.com:1234`.
* `/search` - Location / Path. Examples: `/search`, `/documents/presentation.pdf`.
* `?q=algebra` - Query. Examples: `?q=algebra`, `?foo=1&bar=2&xyz=3,4,5`.
* `#results` - Fragment. Examples: `#results`, `#main`.
