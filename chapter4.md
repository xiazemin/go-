# Request

／src/net/request.go

标示服务端收到的或者客户端发出的http请求，客户端和服务端用法基本一样

type Request struct {

Method string //区分请求类型\(GET, POST, PUT, etc.\)

URL \*url.URL//区分URL是被服务端请求的还是客户端发出的请求

对于客户端请求，多数情况下是空的

对于服务端被请求的URL从 RequestURI的Request-Line 提取

