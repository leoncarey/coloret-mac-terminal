# coloret-mac-terminal
Your terminal more cute.

##### How to install?
Open your `.bash_profile` and paste the code below:

```sh
parse_git_branch() {
    git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1="\[\033[0;35m\][\u@\h] \[\033[0;36m\]\w\[\033[0;33m\]\$(parse_git_branch)\[\033[00m\]$ "
```
