.PHONY: setup build lint test

setup:
	python3 -m venv .venv \
	&& source .venv/bin/activate \
	&& pip3 install -r requirements.txt

build:
	pip3 install -r requirements.txt

lint:
	python3 -m black --check ./**.py

fmt:
	python3 -m black ./**.py

test:
	echo "Not implemented"
