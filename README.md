# My environment

Read the directory [docs](./docs) for more detailed settings for tools

## Development tools

### Install tig

Tig is an ncurses-based text-mode interface for git. It functions mainly as a Git repository browser, but can also assist in staging changes for commit at chunk level and act as a pager for output from various Git commands.

Instruction for installation [here](https://jonas.github.io/tig/).

## Install assets

### Install font `iosevka`

Installation Instructions

```sh
sudo dnf copr enable peterwu/iosevka 
```

```sh
sudo dnf search iosevka
```

```sh
sudo dnf install {font_of_choice}
```

### Install firefox-gnome-theme

<https://github.com/rafaelmardojai/firefox-gnome-theme>

### Install docker

Read detailed installation instructions [here](https://docs.docker.com/engine/install/).

Install the dnf-plugins-core package (which provides the commands to manage your DNF repositories) and set up the repository.

```sh
sudo dnf -y install dnf-plugins-core
sudo dnf config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo
```

Install Docker Engine

```sh
sudo dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

Start docker

```sh
sudo systemctl start docker
```

### Install tools for compiler

```sh
sudo dnf install make gcc-c++ gcc make bzip2 openssl-devel libyaml-devel libffi-devel readline-devel zlib-devel gdbm-devel ncurses-devel msgfmt
```
