# Intro

This example sends a signing request to the fiskaltrust.Service via REST.

A zero receipt is sent to a specified url and CashBox and the response is printed.

> _**Note:** If the http statuscod204 is returned the CashBox may not yet be activated and you'll need to send a start receipt first. For instructions on how to do this please consult our videos about [sending requests to the fiskaltrust.Service](https://www.youtube.com/playlist?list=PL9QFfhi6nFj94kZBTxxL3kyar2Q7yTejU)_

This example can be used as a starting point to implement the [fiskaltrust.Interface](https://github.com/fiskaltrust/interface-doc)

# Requirements

## Toolchain

To compile the example the `C` compiler [`gcc`](https://gcc.gnu.org/install/) and the buildtool [`make`](https://www.gnu.org/software/make/) is needed.

> _**Note:** On windows we recomend installing these with a package manager like [scoop](https://scoop.sh/) or [chocolatey](https://chocolatey.org/)_

## curl

To build the example, the [curl library](https://curl.haxx.se/libcurl/) needs to be available. You can download this library from [here](https://curl.haxx.se/download.html).

> _**Note:** We tested the example with version 7.x.x other versions may not work._

### Windows

Building the curl library for windows is a complicated process. [This](https://albertino80.github.io/building.html) guide is a good starting point.

> _**Note:** We do not recommend working with C and REST on windows since building curl takes a lot of effort._

### Linux

Install the library via your distributions package manager.

| Distribution  | Command                    |
|---------------|----------------------------|
| Ubuntu/Debian | `apt-get install libcurl4` |
| Fedora        | `dnf install libcurl`      |
| OpenSUSE      | `zypper install libcurl4`  |

# Building

## Linux

  1. Run the `make` command.