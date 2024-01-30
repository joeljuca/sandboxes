# Sandbox: Python

[![Licensed under ISC](https://img.shields.io/github/license/joeljuca/sandboxes "Licensed under ISC")](LICENSE)

Project bootstrapped from [joeljuca/sandboxes](https://github.com/joeljuca/sandboxes), a collection of sandboxes for random experimentations.

Bootstrap yourself a pre-configured Python sandbox with:

```
$ npx degit joeljuca/sandboxes/python [sandbox name]
```

## Setup

This [Python](https://www.python.org/) sandbox uses the following tools:

- [venv](https://docs.python.org/3/library/venv.html)
- [Black](https://black.readthedocs.io/en/stable/)

Python itself should be installed in your system. Everything else is installed through Python's package manager, [pip](https://docs.python.org/3/installing/index.html), under a virtual environment directory `.venv`.

Set everything up quickly with:

```
$ make setup
```

## Usage

First, you must activate your Python venv:

```
$ source .venv/bin/activate
```

Then, just make use of the pre-defined `Makefile` – there are tasks for the most common scenarios:

- `make build`
- `make lint`
- `make fmt`
- `make test`

## License

&copy; 2024 Joel Jucá. Licensed under [ISC](LICENSE)
