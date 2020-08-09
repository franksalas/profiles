# Bash Setup

Links for git-prompt and bash profile with resources.

![](https://media.giphy.com/media/QVOeX6dwObg8znQjZ8/giphy.gif)

## Git prompt support
This script allows you to see repositor status in your prompt
## enable
1. copy this file to somewhere (e.g. ~/.git-prompt.sh)
2. Add the following line to your .bashrc :  
`source ~/.git-prompt.sh`



## Git completion support
This script contains for completing several git  routines used.

## Enable
1. Copy this file to somewhere (e.g. ~/.git-completion.bash
2. Add the following line to your .bashrc : `source ~/.git-completion.bash`

## profile setup
Here is where we add to the bottom of our `.bashrc` file.

```bash
# Enable tab completion
source ~/git-completion.bash

# colors!
green="\[\033[0;32m\]"
blue="\[\033[0;34m\]"
purple="\[\033[0;35m\]"
reset="\[\033[0m\]"

# Change command prompt
source ~/git-prompt.sh
export GIT_PS1_SHOWDIRTYSTATE=1
# '\u' adds the name of the current user to the prompt
# '\$(__git_ps1)' adds git-related stuff
# '\W' adds the name of the current directory
export PS1="$purple\u$green\$(__git_ps1)$blue \W $ $reset"
```

## Source
- [Udacity How to use Git and Github](https://classroom.udacity.com/courses/ud775)
- [Git files](https://github.com/git/git/tree/master/contrib/completion)
