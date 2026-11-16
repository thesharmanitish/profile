---
title: 'Magic Variables In Bash'
date: 2019-07-05
type: docs
aliases:
  - /projects/til/2019-07-05_magic-variables-in-bash/
---
## Magic Variables in Bash

 - `$0` - `$99`
    x-th argument provided to the script/function. `$0` is always the script name even when accessed from within a function. `$1+` will work in functions.

 - `$?`
    Exit code of the last process.

 - `$_`
    Last argument.

 - `$!`
    PID of last process.

 - `$@`
    All arguments.

Note: Always quote variables to avoid word-splitting (except when using `[[` for tests). Run `shellcheck` to make sure.
