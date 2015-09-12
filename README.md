# bash-alias-completion
Bash Completion for Aliases

### The Problem and its Solution

Suppose you have an alias like this:

```shell
alias gc='git clone'
``

If you'll `type gc --` followed by a **[TAB]** you won't get any bash completion for the available options. To overcome this problem you can use script in file `alias_completion.sh`. This script shouldn't be called normally, but sourced (use either `source alias_completion.sh` or `. alias_completion.sh`) after the aliases are defined. IMHO the best way is to put it at the very end of file `~/.bashrc`.

