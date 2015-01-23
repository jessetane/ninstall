# ninstall
A bash script to install node & npm on unix-like systems. Binaries can be fetched from [iojs.org](https://iojs.org/dist) or [nodejs.org](http://nodejs.org/dist).

## Why
Cos [io.js](https://iojs.org) happened, but also because most of the popular solutions either depend on node itself, or are just more complicated than I have the need for.

## How
Install the latest iojs:
```bash
$ ninstall
```

Install a specific version of iojs:
```bash
$ ninstall 1.0.2
```

Install to somewhere other than /usr/local
```bash
$ PREFIX=/opt ninstall
```

Install the latest Joyent node:
```bash
$ JOYENT=true ninstall
```

Install a specific version of Joyent node:
```bash
$ JOYENT=true ninstall 0.10
```

## Install
Dependencies:
* [bash](http://linux.die.net/man/1/bash)
* [cd](http://linux.die.net/man/1/cd)
* [rm](http://linux.die.net/man/1/rm)
* [curl](http://linux.die.net/man/1/curl)
* [grep](http://linux.die.net/man/1/grep)
* [sed](http://linux.die.net/man/1/sed)
* [sort](http://linux.die.net/man/1/sort)
* [mktemp](http://linux.die.net/man/1/mktemp)
* [tar](http://linux.die.net/man/1/tar)
* [rsync](http://linux.die.net/man/1/rsync)

```bash
$ curl -fLO# https://github.com/jessetane/ninstall/archive/1.0.0.tar.gz
$ tar xf ninstall-1.0.0.tar.gz
$ cd ninstall-1.0.0
$ cp bin/ninstall /usr/local/bin
```

## Releases
The latest stable release is published as a tarball on github.
* [1.x](https://github.com/jessetane/ninstall/archive/1.0.0.tar.gz)
 * First pass.

## License
Copyright © 2014 Jesse Tane <jesse.tane@gmail.com>

This work is free. You can redistribute it and/or modify it under the
terms of the [WTFPL](http://www.wtfpl.net/txt/copying).

No Warranty. The Software is provided "as is" without warranty of any kind, either express or implied, including without limitation any implied warranties of condition, uninterrupted use, merchantability, fitness for a particular purpose, or non-infringement.
