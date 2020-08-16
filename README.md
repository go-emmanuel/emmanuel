# Emmanuel

Emmanuel is a high performance fork of Macaron, a modular web framework in Go.

## Getting Started

The minimum requirement of Go is **1.6**.

To install Emmanuel:

	go get github.com/go-emmanuel/emmanuel

The very basic usage of Emmanuel:

```go
package main

import "github.com/go-emmanuel/emmanuel"

func main() {
	e := emmanuel.Classic()
	e.Get("/", func() string {
		return "Hello world!"
	})
	e.Run()
}
```

## Features

- Powerful routing with suburl.
- Flexible routes combinations.
- Unlimited nested group routers.
- Directly integrate with existing services.
- Dynamically change template files at runtime.
- Allow to use in-memory template and static files.
- Easy to plugin/unplugin features with modular design.
- Handy dependency injection powered by [inject](https://github.com/codegangsta/inject).
- Better router layer and less reflection make faster speed.

## Credits

- Basic design of [Martini](https://github.com/go-martini/martini).
- Fork of [Macaron](https://github.com/go-macaron)

## Changes from Macaron

This framework is a fork of [Macaron](https://github.com/go-macaron/macaron).

The following are changes made:

- Use sync.Pool for Context
- Use Fasthttp (in progress)
- Other performance tweaks


## License

This project is under the Apache License, Version 2.0.
