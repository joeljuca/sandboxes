# Sandbox: SQLite

[![Creative Commons Attribution 4.0 International License](https://i.creativecommons.org/l/by/4.0/80x15.png "Creative Commons Attribution 4.0 International License")](https://creativecommons.org/licenses/by/4.0/ "Creative Commons Attribution 4.0 International License")

Project bootstrapped from [joeljuca/sandboxes](https://github.com/joeljuca/sandboxes), a collection of sandboxes for random experimentations.

Bootstrap yourself a pre-configured SQLite sandbox with:

```
$ npx degit joeljuca/sandboxes/sqlite [sandbox name]
```

## Setup

This [SQLite](https://www.sqlite.org/) sandbox is set as a [Python](https://www.python.org/) project. Additionally, it uses the following Python tools:

- [venv](https://docs.python.org/3/library/venv.html)
- [yoyo-migrations](https://pypi.org/project/yoyo-migrations/)
- [SQLFluff](https://sqlfluff.com/)

SQLite and Python should be installed in your system. Everything else is installed through Python's package manager, [pip](https://docs.python.org/3/installing/index.html).

This project assumes a venv is set up under a `.venv` dir, and a SQLite database named `database.sqlite` – both in the root dir.

Set everything up quickly with:

```
$ make setup
```

It should create a venv under `.venv` with dependencies already in place, and it should create and migrate the SQLite database `database.sqlite`.

## Usage

First, you must activate your Python venv:

```
$ source .venv/bin/activate
```

Then, just make use of the pre-defined `makefile` – there are tasks for the most common scenarios:

- `make build`
- `make lint`
- `make fmt`
- `make test`
- `make db.create`
- `make db.migrate`
- `make db.drop`
- `make db.repl`
- `make db.new_migration name=<migration name>`
- `make db.setup` (alias for `make db.create && make db.migrate`)
- `make db.reset` (alias for `make db.drop && make db.setup`)

## License

Copyright 2023 Joel Jucá. Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
