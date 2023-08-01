# .zshrc

## Install zsh-z

```sh
git clone https://github.com/agkozak/zsh-z ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-z
```

## Install zsh-autosuggestions

```sh
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Zshrc config

```r
HISTFILE=~/.histfile
HISTSIZE=1000
SAVEHIST=1000

export ZSH="$HOME/.oh-my-zsh"

ZSH_THEME="robbyrussell"

plugins=(git zsh-autosuggestions zsh-syntax-highlighting asdf)

source $ZSH/oh-my-zsh.sh

alias python=/usr/bin/python3
alias yc="yarn commit"
alias tgs="tig status"

export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"

# pnpm
export PNPM_HOME="/home/lordszn/.local/share/pnpm"
export PATH="$PNPM_HOME:$PATH"
```
