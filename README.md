Zephir Language
===============

This is the repo for Zephir language.

xx is the parser for the language:

You will need json-c installed on your machine:

* [json-c](https://github.com/json-c/json-c)

Compilation:

```bash
gcc parser.c scanner.c -o xx -ljson-c -g3
```

Compile a xx file:

```bash
php compiler.php
```

The code produced is placed in ext/, there you can perform the standard compilation:

```bash
cd ext/
phpize
./configure --enable-test
make && sudo make install
```