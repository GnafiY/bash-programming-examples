# bash-programming-examples

Some examples for bash programming.

## About bash cmds

You may go to following sites for details about bash cmds.

https://ss64.com/

https://github.com/Idnan/bash-guide

## Examples for bash

```bash
# split input string($1) with given separator($2)
split() {
    local str=$1        # source string
    local separator=$2  # separator, for example ' ', '\' or ','
    local splitted=($(echo $str | tr "${separator}" "\n"))  # result
    echo "${splitted[@]}"
}

:<<__COMMENT__
$ split 'a/b/c/d/e/g' '/'
a b c d e g
__COMMENT__
```
