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
ZSH_THEME="robbyrussell"

# History
HISTFILE=~/.histfile
HISTSIZE=1000
SAVEHIST=1000

# Promp
PROMPT='%n@%m:%15<..<%~%<<%# '

# Plugins
plugins=(
  z
  git 
  docker
  docker-compose
  zsh-autosuggestions 
  zsh-syntax-highlighting
  asdf
)

# Alias
alias nc='npm commit'
alias ni='npm install'
alias tgs='tig status'
alias h='htop'
alias la='ls -a'
alias lla='ls -la'

# Stamp
HIST_STAMPS="mm/dd/yyyy

# Python
export PATH=~/.local/bin/:$PATH

# Env
export EDITOR=vim
export TERMINAL=alacritty
export VISUAL=vim
export DISABLE_AUTO_UPDATE="true"
```
