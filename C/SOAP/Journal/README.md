# Intro

This example sends a journal request to the fiskaltrust.Service via SOAP.

A journal request is sent to a specified url and CashBox and the response is printed.

This example can be used as a starting point to implement the [fiskaltrust.Interface](https://github.com/fiskaltrust/interface-doc).

> _**Note:** The german journal is being implemented at the moment in the fiskaltrust.Service. Since the implementation is similar, you can use the austrian service for testing._

# Requirements

## Toolchain

To compile the example the `C` compiler [`gcc`](https://gcc.gnu.org/install/) and the buildtool [`make`](https://www.gnu.org/software/make/) is needed.

> _**Note:** On windows we recomend installing these with a package manager like [scoop](https://scoop.sh/) or [chocolatey](https://chocolatey.org/)_

## gSOAP

To build the example, the [gSOAP library](https://www.genivia.com/products.html#gsoap) needs to be available. You can download this library from [here](https://sourceforge.net/projects/gsoap2/).

> _**Note:** We tested the example with version 2.8.x other versions may not work._

### Windows

Download and unpack the gSOAP library from https://sourceforge.net/projects/gsoap2/.

### Linux

Install the library via your distributions package manager.

| Distribution  | Command                      |
|---------------|------------------------------|
| Ubuntu/Debian | `apt-get install gsoap`      |
| Fedora        | `dnf install gsoap`          |

## WSDL

To build the SOAP interface the wsdl file for the fiskaltrust.Interface is needed.

You can find this file in the folder [`/dist/WSDL`](https://github.com/fiskaltrust/interface-doc/tree/master/dist/WSDL) in the [fiskaltrust.Interface](https://github.com/fiskaltrust/interface-doc) repository.

#### Manual

You can manually install the library according to [these instructions](https://www.genivia.com/downloads.html#unix).

# Building

## Windows

  1. Run the powershell script `configure.ps1` and follow the instructions.
  2. Run the `make` command.

> _**Example:**_
> ```
> .\configure.ps1
> make
> ```

## Linux

  1. Run the powershell script `configure.sh` and follow the instructions.
  2. Run the `make` command.

> _**Example:**_
> ```
> ./configure.sh
> make
> ```
