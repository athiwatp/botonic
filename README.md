botonic
=======

Build chatbots using React

[![Version](https://img.shields.io/npm/v/botonic.svg)](https://npmjs.org/package/botonic)
[![CircleCI](https://circleci.com/gh/ericmarcos/botonic/tree/master.svg?style=shield)](https://circleci.com/gh/ericmarcos/botonic/tree/master)
[![Appveyor CI](https://ci.appveyor.com/api/projects/status/github/ericmarcos/botonic?branch=master&svg=true)](https://ci.appveyor.com/project/ericmarcos/botonic/branch/master)
[![Codecov](https://codecov.io/gh/ericmarcos/botonic/branch/master/graph/badge.svg)](https://codecov.io/gh/ericmarcos/botonic)
[![Downloads/week](https://img.shields.io/npm/dw/botonic.svg)](https://npmjs.org/package/botonic)
[![License](https://img.shields.io/npm/l/botonic.svg)](https://github.com/ericmarcos/botonic/blob/master/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g botonic
$ botonic COMMAND
running command...
$ botonic (-v|--version|version)
botonic/0.2.2 darwin-x64 node-v9.9.0
$ botonic --help [COMMAND]
USAGE
  $ botonic COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [botonic deploy [BOT_NAME]](#botonic-deploy-bot-name)
* [botonic help [COMMAND]](#botonic-help-command)
* [botonic input INPUT](#botonic-input-input)
* [botonic login](#botonic-login)
* [botonic logout](#botonic-logout)
* [botonic new NAME [TEMPLATENAME]](#botonic-new-name-templatename)
* [botonic run [INPUT]](#botonic-run-input)

## botonic deploy [BOT_NAME]

Deploy Botonic project to botonic.io cloud

```
USAGE
  $ botonic deploy [BOT_NAME]

EXAMPLE
  $ botonic deploy
  Building...
  Creating bundle...
  Uploading...
  🚀 Bot deployed!
```

_See code: [src/commands/deploy.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/deploy.ts)_

## botonic help [COMMAND]

display help for botonic

```
USAGE
  $ botonic help [COMMAND]

ARGUMENTS
  COMMAND  command to show help for

OPTIONS
  --all  see all commands in CLI
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v1.2.3/src/commands/help.ts)_

## botonic input INPUT

Get response from a single input

```
USAGE
  $ botonic input INPUT

OPTIONS
  -c, --context=context  Context of current session
  -p, --path=path        Path to botonic project. Defaults to current dir.
  -r, --route=route      Route of the current bot state.

EXAMPLE
  $ botonic input "{\"type\": \"text\", \"data\": \"hi\"}"
  Hello!
```

_See code: [src/commands/input.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/input.ts)_

## botonic login

Log in to Botonic

```
USAGE
  $ botonic login

OPTIONS
  -p, --path=path  Path to botonic project. Defaults to current dir.
```

_See code: [src/commands/login.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/login.ts)_

## botonic logout

Log out of Botonic

```
USAGE
  $ botonic logout

OPTIONS
  -p, --path=path  Path to botonic project. Defaults to current dir.
```

_See code: [src/commands/logout.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/logout.ts)_

## botonic new NAME [TEMPLATENAME]

Create a new Botonic project

```
USAGE
  $ botonic new NAME [TEMPLATENAME]

ARGUMENTS
  NAME          name of the bot folder
  TEMPLATENAME  OPTIONAL name of the bot template

EXAMPLE
  $ botonic new test_bot
  Creating...
  ✨ test_bot was successfully created!
```

_See code: [src/commands/new.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/new.ts)_

## botonic run [INPUT]

Start interactive session

```
USAGE
  $ botonic run [INPUT]

OPTIONS
  -p, --path=path  Path to botonic project. Defaults to current dir.

EXAMPLE
  $ botonic run
  Your bot is ready, start talking:
  [you] > Hi
  [bot] > Bye!
```

_See code: [src/commands/run.ts](https://github.com/hubtype/botonic/blob/v0.2.2/src/commands/run.ts)_
<!-- commandsstop -->
