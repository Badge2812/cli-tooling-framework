
# cli-tooling-framework

## Overview

The aim of this framework is to provide a simple and versatile JavaScript based tooling from which it is possible to create CLIs and various other command-line tools. 

## Dependencies

- Arg
- Chalk
- Debug
- Ajv + BetterAjvErrors
- Cosmicconfig

## Operation

Once the framework has been cloned it is as simple as setting up a link using npm-link to allow for local testing and debugging

Inside the **tool** Directory
```
npm link
```
Then inside the **testProject** Directory
```
npm link tool
```

## Debugging

Debugging is achieved using the debug library, and the script for running a debug session is as follows
```bash
# Basic Debugging Syntax
$ DEBUG=[options] tool [command]
# Will run the start command with debugging available on everything while excluding any debugging from the binary.
$ DEBUG=*,-bin tool --start
```
