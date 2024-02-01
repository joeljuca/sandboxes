.PHONY: setup build lint fmt test

setup:
	python3 -m venv .venv

build:
	pip3 install -r requirements.txt

lint:
	python3 -m black --check ./**.py

fmt:
	python3 -m black ./**.py

test:
	echo "Not implemented"
