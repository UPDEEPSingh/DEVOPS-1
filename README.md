name: updeep

on:
	push:
		branches: [main]

jobs:
	build:
		runs-on: ubuntu-latest
		steps:
-  uses: actions/checkout@v2
    with:
	fetch-depth: 0
- run: make
