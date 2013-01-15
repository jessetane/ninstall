```
     _         _       _ _ 
 ___|_|___ ___| |_ ___| | |
|   | |   |_ -|  _| .'| | |
|_|_|_|_|_|___|_| |__,|_|_|

```
## What
Install and switch between versions of [node](https://github.com/joyent/node).

## Why
[nave](https://github.com/isaacs/nave), [nvm](https://github.com/creationix/nvm), etc are really powerful, but they're also kind of complicated. This is a very basic shell script that just gets & installs binaries.

## How
Run the script and pass the version of node you'd like to install. If it doesn't already exist in $PREFIX/lib, the script will attempt to download the binaries from [nodejs.org](http://nodejs.org). Once $PREFIX/lib contains an acceptable version, the script symlinks the necessary components out to $PREFIX/. That's it. If you have $PREFIX/bin in your PATH, running `node -v` should reflect the changes immediately.

## Usage
`ninstall v0.9.5`

## Install
`curl -O https://raw.github.com/jessetane/ninstall/master/ninstall && chmod +x ninstall`

## Dependencies
* curl
* bash

## Notes
* Be sure to set the variables at the top of the script to match your installation environment! For example, $PREFIX is set to your home directory by default.
* OS specific binaries only exist as far back as v0.8.6, so anything older than that likely won't work.

## License
MIT
