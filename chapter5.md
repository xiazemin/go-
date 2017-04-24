# URL

src/net/url/url.go

package url

标示一个已经解析的URL

通用的表达格式是：	scheme://\[userinfo@\]host/path\[?query\]\[\#fragment\]



type URL struct {

```
Scheme   string

Opaque   string    // encoded opaque data

User     \*Userinfo // username and password information

Host     string    // host or host:port

Path     string

RawPath  string // encoded path hint \(Go 1.5 and later only; see EscapedPath method\)

RawQuery string // encoded query values, without '?'

Fragment string // fragment for references, without '\#'
```

}

