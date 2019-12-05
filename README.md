# iso8601

[![GoDoc][godoc-image]][godoc-url]
[![Build Status][build-image]][build-url]
[![Coverage Status][coverage-image]][coverage-url]
[![Go Report Card][goreport-image]][goreport-url]

ISO8601 date, time, duration parser and formatter.

ISO8601 is format of time/duration in MPEG-DASH .MPD files. See [stackoverflow](https://stackoverflow.com/questions/23800812/the-format-of-time-duration-in-mpeg-dash-mpd-file).

```go
package main

import (
  "fmt"
  "time"

  "github.com/go-x-pkg/iso8601"
)

func main() {
  // PT3M15S
  fmt.Println(iso8601.Duration(3*time.Minute + 15*time.Second))
}
```

```
PT0.1S
PT1M6.762S
PT20S
PT3M15S
PT3M15S
P6DT4H54M18S
P12W6DT4H54M43S
P2Y12W6DT4H54M18S
P6D
P2Y
PT3M
```

[godoc-image]: https://godoc.org/github.com/go-x-pkg/iso8601?status.svg
[godoc-url]: https://godoc.org/github.com/go-x-pkg/iso8601

[build-image]: https://travis-ci.org/go-x-pkg/iso8601.svg?branch=master
[build-url]: https://travis-ci.org/go-x-pkg/iso8601

[coverage-image]: https://coveralls.io/repos/github/go-x-pkg/iso8601/badge.svg?branch=master
[coverage-url]: https://coveralls.io/github/go-x-pkg/iso8601?branch=master

[goreport-image]: https://goreportcard.com/badge/github.com/go-x-pkg/iso8601
[goreport-url]: https://goreportcard.com/report/github.com/go-x-pkg/iso8601
