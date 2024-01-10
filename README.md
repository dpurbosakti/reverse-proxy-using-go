# TESTING
## Check if demo servers are running
### Testing server1
On another terminal run following commands
```sh
$ curl -iv  http://localhost:9001
```

Result
```
HTTP/1.1 200 OK
Server: gunicorn/19.9.0
Date: Thu, 01 Dec 2022 21:09:14 GMT
Connection: keep-alive
Content-Type: text/html; charset=utf-8
Content-Length: 9593
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true
```

### Testing server2
```sh
$ curl -iv  http://localhost:9002
```

Result
```
HTTP/1.1 200 OK
Server: gunicorn/19.9.0
Date: Thu, 01 Dec 2022 21:09:14 GMT
Connection: keep-alive
Content-Type: text/html; charset=utf-8
Content-Length: 9593
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true
```

### Testing server3
```sh
$ curl -iv  http://localhost:9003
```

Result
```
HTTP/1.1 200 OK
Server: gunicorn/19.9.0
Date: Thu, 01 Dec 2022 21:09:14 GMT
Connection: keep-alive
Content-Type: text/html; charset=utf-8
Content-Length: 9593
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true
```

### Check if reverse proxy servers is running
```sh
$ curl -I  http://localhost:8080/server1
```

Result
```
HTTP/1.1 200 OK
Access-Control-Allow-Credentials: true
Access-Control-Allow-Origin: *
Content-Length: 9593
Content-Type: text/html; charset=utf-8
Date: Thu, 01 Dec 2022 21:11:18 GMT
Server: gunicorn/19.9.0
```