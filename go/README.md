# Sandbox: Go

[![Licensed under ISC](https://img.shields.io/github/license/joeljuca/sandboxes "Licensed under ISC")](LICENSE)

Project bootstrapped from [joeljuca/sandboxes](https://github.com/joeljuca/sandboxes), a collection of sandboxes for random experimentations.

Bootstrap yourself a pre-configured Go sandbox with:

```
$ npx degit joeljuca/sandboxes/go [sandbox name]
```

## Setup

This [Go](https://go.dev/) sandbox uses the following tools:

- TBD

<!--
- [venv](https://docs.python.org/3/library/venv.html)
- [Black](https://black.readthedocs.io/en/stable/)
-->

Go itself should be installed in your system. Everything else is installed through Go's package manager.

Set everything up quickly with:

```
$ make setup
```

## Usage

First, you must build your Go program:

```
$ make build
```

Your compiled program should be available as `cli`.

You can also make use of the pre-defined `Makefile` – there are tasks for the most common scenarios:

- `make lint`
- `make fmt`
- `make test`
- `make test.watch`

## License

&copy; 2024 Joel Jucá. Licensed under [ISC](LICENSE)
