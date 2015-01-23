# ninstall
A bash script to install and switch between versions node on unix-like systems. Versions >= 1.x are fetched from [iojs.org](https://iojs.org/dist), < from [nodejs.org](http://nodejs.org/dist).

## Why
Cos [io.js](https://iojs.org) happened. Also most of the other popular solutions either depend on node itself, or are just more complicated than I have the need for.

## How
Install the latest version of node:
```bash
$ ninstall
```

Install a specific version:
```bash
$ ninstall 1.0.3
```

Install the latest patch version:
```bash
$ ninstall 0.10
```

Install to somewhere other than /usr/local
```bash
$ PREFIX=/opt ninstall
```

## Download
```bash
$ curl -L# https://github.com/jessetane/ninstall/archive/2.0.0.tar.gz \
  | tar x --strip-components 2 -C /usr/local/bin
```

## Dependencies
* [bash](http://linux.die.net/man/1/bash)
* [cd](http://linux.die.net/man/1/cd)
* [rm](http://linux.die.net/man/1/rm)
* [mkdir](http://linux.die.net/man/1/mkdir)
* [curl](http://linux.die.net/man/1/curl)
* [grep](http://linux.die.net/man/1/grep)
* [sed](http://linux.die.net/man/1/sed)
* [sort](http://linux.die.net/man/1/sort)
* [mktemp](http://linux.die.net/man/1/mktemp)
* [tar](http://linux.die.net/man/1/tar)
* [rsync](http://linux.die.net/man/1/rsync)

## Inspiration
* [`n`](https://github.com/tj/n)

## Releases
The latest stable release is published as a tarball on github.
* [2.x](https://github.com/jessetane/ninstall/archive/2.0.0.tar.gz)
 * Remove the need to manually specify iojs vs node
 * Check cache before doing internets if possible
* [1.x](https://github.com/jessetane/ninstall/archive/1.0.0.tar.gz)
 * First pass.

## License
Copyright © 2014 Jesse Tane <jesse.tane@gmail.com>

This work is free. You can redistribute it and/or modify it under the
terms of the [WTFPL](http://www.wtfpl.net/txt/copying).

No Warranty. The Software is provided "as is" without warranty of any kind, either express or implied, including without limitation any implied warranties of condition, uninterrupted use, merchantability, fitness for a particular purpose, or non-infringement.
