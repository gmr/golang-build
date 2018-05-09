golang-build
============
Alpine based image for running go build, that includes `git`, `make`,
and `dep`.

Usage
-----
Run with `go build`:

```bash
docker run --rm -t -i -v `pwd`:/go/src/[PROJECT] -w /go/src/[PROJECT] gavinmroy/golang-build:1.10.1 go build
```

Or use a `Makefile` that runs `dep ensure`:

```bash
docker run --rm -t -i -v `pwd`:/go/src/[PROJECT] -w /go/src/[PROJECT] gavinmroy/golang-build:1.10.1 make
```
