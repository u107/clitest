oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g clitest
$ clitest COMMAND
running command...
$ clitest (--version)
clitest/1.0.0 win32-x64 node-v18.19.0
$ clitest --help [COMMAND]
USAGE
  $ clitest COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`clitest hello PERSON`](#clitest-hello-person)
* [`clitest hello world`](#clitest-hello-world)
* [`clitest help [COMMANDS]`](#clitest-help-commands)

## `clitest hello PERSON`

Say hello

```
USAGE
  $ clitest hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/4746/clitest/blob/v1.0.0/src/commands/hello/index.ts)_

## `clitest hello world`

Say hello world

```
USAGE
  $ clitest hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ clitest hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/4746/clitest/blob/v1.0.0/src/commands/hello/world.ts)_

## `clitest help [COMMANDS]`

Display help for clitest.

```
USAGE
  $ clitest help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for clitest.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.0.12/src/commands/help.ts)_
<!-- commandsstop -->
