# URL

src/net/url/url.go

package url



type URL struct {

	Scheme   string

	Opaque   string    // encoded opaque data

	User     \*Userinfo // username and password information

	Host     string    // host or host:port

	Path     string

	RawPath  string // encoded path hint \(Go 1.5 and later only; see EscapedPath method\)

	RawQuery string // encoded query values, without '?'

	Fragment string // fragment for references, without '\#'

}

