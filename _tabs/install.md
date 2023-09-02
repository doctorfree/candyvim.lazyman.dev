---
layout: post
icon: fas fa-arrow-circle-down
order: 1
toc: true
post_style: page
---

# CandyVim Neovim Configuration Installation

## Install Lazyman

[Lazyman](https://lazyman.dev) provides tools to manage multiple Neovim configurations
and a shell function to fuzzy search and select among them.

```bash
git clone https://github.com/doctorfree/nvim-lazyman $HOME/.config/nvim-Lazyman
$HOME/.config/nvim-Lazyman/lazyman.sh
```

## Install the CandyVim Neovim configuration

```bash
lazyman -w CandyVim
```

Alternately, use the `lazyman` command menu interface to install `CandyVim`.

## Configure the shell environment

```bash
export NVIM_APPNAME="nvim-CandyVim"
alias nvim="NVIM_APPNAME=nvim-CandyVim nvim"
```

Alternately, use the `nvims` Lazyman shell function and select `CandyVim`.
