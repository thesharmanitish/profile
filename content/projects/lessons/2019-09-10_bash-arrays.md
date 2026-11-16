---
title: 'Bash Arrays'
date: 2019-09-10
type: docs
aliases:
  - /projects/til/2019-09-10_bash-arrays/
---
## Bash Arrays

Declare a variable with `ARRAY=(one two three)` and reference it using `echo ${ARRAY[*]}` or `echo ${ARRAY[2]}` for a single element.

Note that brackets are not required in for statements: `for i in 1 2 3; do echo $i; done`

