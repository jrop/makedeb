<h1 align="center">Makedeb</h1>
<div align="center">
<img alt="Drone CI - Stable" src="https://img.shields.io/drone/build/hwittenborn/makedeb/stable?label=stable&server=https%3A%2F%2Fdrone.hunterwittenborn.com">
<img alt="Drone CI - Alpha" src="https://img.shields.io/drone/build/hwittenborn/makedeb/alpha?label=alpha&server=https%3A%2F%2Fdrone.hunterwittenborn.com">
</div>

## Overview ##
makedeb takes PKGBUILD files and creates Debian archives installable with APT.

*Automated installation and updates of AUR and Arch Linux packages are available with [mpm](https://github.com/hwittenborn/mpm).*

## Installation ##
First, set up the repository with the following commands:
```sh
sudo wget 'https://hunterwittenborn.com/keys/apt.asc' -O /etc/apt/trusted.gpg.d/hwittenborn.asc
echo 'deb [arch=all] https://repo.hunterwittenborn.com/debian/makedeb any main' | sudo tee /etc/apt/sources.list.d/makedeb.list
sudo apt update
```
Then, install makedeb with one of the following commands:
- makedeb (stable release):
```sh
sudo apt install makedeb
```
- makedeb (alpha release):
```sh
sudo apt install makedeb-alpha
```

As expected, don't run the alpha release if you're expecting stability. Things could break occasionally, and you'll need to know how to get around your system when it happens.

## Usage ##
Instructions can be found after installation with `makedeb --help`

A list of packages that are known to work with makedeb (Debian systems) is available in [WORKING_PACKAGES.md](./WORKING_PACKAGES.md)

Documentation on the inner working of makedeb, as well as guides to contributing, are available in the [makedeb wiki](https://github.com/hwittenborn/makedeb/wiki).

## Get in touch ##
A Matrix room is available at [#git:hunterwittenborn.com](https://matrix.to/#/#git:hunterwittenborn.com) for discussion of any of my projects. Feel free to hop in if you need any help.
