.PHONY: setup build lint test db.create db.migrate db.drop db.repl db.new_migration db.setup db.reset

setup:
	python3 -m venv .venv \
	&& source .venv/bin/activate \
	&& pip3 install -r requirements.txt \
	&& make db.setup

build:
	pip3 install -r requirements.txt

lint:
	sqlfluff lint ./migrations/*.sql

fmt:
	sqlfluff format ./migrations/*.sql

test:
	make build \
	&& make db.setup

db.create:
	sqlite3 database.sqlite 'select 1'

db.migrate:
	yoyo apply

db.drop:
	rm database.sqlite || true

db.repl:
	sqlite3 -init .sqliterc database.sqlite

db.new_migration:
	yoyo new --sql -m $(name)

db.setup:
	make db.create && make db.migrate

db.reset:
	make db.drop && make db.setup
