# Dotfiles as a bare repo

Storing dotfiles as a bare repository. An experiment for now — I don’t
particularly like the idea of managing different systems on different branches,
but maybe it could work through merging individual commits and what not.

## Setup

Clone the repo with at flag `--bare` and set `--git-dir` to `$HOME/.dotfiles`
(or whatever you’d like, just make sure to reflect that in any aliases you use).

## Helpers

```bash
# Git wrapper
alias dotfiles="git --git-dir=$HOME/.dotfiles --work-tree=$HOME"

# Because I am too lazy to type out dotfiles every time
alias dots=dotfiles
```

## Idea

https://www.atlassian.com/git/tutorials/dotfiles
