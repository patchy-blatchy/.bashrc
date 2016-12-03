## Prompt

1. Do all changes in file .bash_profile. Also you can change your .bashrc, but in this case it won't run changes automatically. To run changes in .bashrc execute this line  source ~/.bashrc

```
export PS1="\W \$"
```
This line will change your prompt. It gives: 
> ~/Desktop $ 

```
export PS1="\w\[\033[33m\] (\$(git branch 2>/dev/null | grep '^*' | colrm 1 2))\[\033[32m\]$ "
```

> ~/your_folder (your_branch)$ 

This will change your prompt to display not only your working directory but also your current git branch in color. If you want to change color output you can easily do it. Just pick up possible colors below.

## ANSI color codes

| Code color  | Color output |
| ------------- | ------------- |
| RS="\[\033[0m\]"  | # reset |
| HC="\[\033[1m\]"  | # hicolor  |
| UL="\[\033[4m\]"  | # underline |
| INV="\[\033[7m\]"  | # inverse background and foreground  |
| FBLK="\[\033[30m\]"  | # foreground black  |
| FRED="\[\033[31m\]"  | # foreground red  |
| FGRN="\[\033[32m\]"  | # foreground green |
| FYEL="\[\033[33m\]"  | # foreground yellow  |
| FBLE="\[\033[34m\]"  | # foreground blue  |
| FMAG="\[\033[35m\]"  | # foreground magenta  |
| FCYN="\[\033[36m\]"  | # foreground cyan  |
| FWHT="\[\033[37m\]" | # foreground white  |
| BBLK="\[\033[40m\]"  | # background black  |
| BRED="\[\033[41m\]"  | # background red  |
| BGRN="\[\033[42m\]"  | # background green |
| BYEL="\[\033[43m\]"  | # background yellow  |
| BBLE="\[\033[44m\]"  | # background blue  |
| BMAG="\[\033[45m\]" | # background magenta  |
| BCYN="\[\033[46m\]"  | # background cyan  |
| BWHT="\[\033[47m\]"  | # background white  |
