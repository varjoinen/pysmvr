# pysmvr, semver util for Python
[![Build Status](https://travis-ci.org/varjoinen/pysmvr.svg?branch=master)](https://travis-ci.org/varjoinen/pysmvr)

Provides commandline tool and functions for [semantic versions](https://semver.org/):

 * validation of version strings
 * increment of versions (major, minor or patch)
 * decrement of versions
 * parsing version string to dict
 * serializing version dict to string

## Installation

```
pip install pysmvr
```

## Usage

```
usage: pysmvr [-h] [--type {major,minor,patch}] [-s STEP] [-i | -d] [version]

Semantic versioning tool

positional arguments:
  version               Semantic version

optional arguments:
  -h, --help            show this help message and exit
  --type {major,minor,patch}
                        Semantic version part to process, defaults to PATCH
  -s STEP, --step STEP  Increment/decrement for --inc/--dec
  -i, --inc             Increase version defined with --type [type]
  -d, --dec             Decrease version defined with --type [type]
```