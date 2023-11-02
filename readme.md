# Sandboxes

[![Licensed under ISC](https://img.shields.io/github/license/joeljuca/sandboxes "Licensed under ISC")](LICENSE)

A collection of pre-configured sandboxes to experiment with different technologies.

## Usage

Each dir is a sandbox. To use one, clone the Git repo in your machine, duplicate the desired sandbox into your local projects dir, and rename it as you wish.

### degit

If you have Node.js installed, you can use [degit](https://www.npmjs.com/package/degit) to do the hard work for you:

```
$ npx degit joeljuca/sandboxes/<sandbox-name> <dir-name>
```

### Makefiles

Each sandbox should have a `Makefile` with at least the following tasks (targets):

- `build`
- `lint`
- `fmt`
- `test`

Also, if the sandbox uses a database, the following tasks should also be present:

- `db.create`
- `db.migrate`
- `db.drop`
- `db.repl`
- `db.setup` (alias for `make db.create && make db.migrate`)
- `db.reset` (alias for `make db.drop && make db.setup`)

## License

Licensed under [ISC](LICENSE)
