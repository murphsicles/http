# @net/http — Core HTTP Types for Zeta

Zeta port of the [hyperium/http](https://github.com/hyperium/http) library (v1.2.0).

## Features

- `Request<T>` and `Response<T>` with builder pattern
- `Method` (GET, POST, PUT, DELETE, HEAD, OPTIONS, CONNECT, PATCH, TRACE)
- `StatusCode` with all standard codes
- `HeaderMap`, `HeaderName`, `HeaderValue`
- `Uri` with scheme, authority, path, query components
- `Version` (HTTP/0.9 through HTTP/3.0)

## Usage

```zeta
use http::{Request, Response, Method, StatusCode};

let req = Request::builder()
    .method(Method::GET)
    .uri("https://example.com/")
    .header("Accept", "text/html")
    .body("");
```

## License

MIT
