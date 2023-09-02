---
layout: post
title: CandyVim Neovim Configuration
toc: true
post_style: page
---

<h2 align="center">CandyVim Neovim Configuration</h2>

An Eye Candy Neovim config built to work most efficiently with Frontend Development

This is based on [Ecovim](https://github.com/ecosse3/nvim) with a lot of useless eye candy
thrown in to demonstrate how useful Neovim is even loaded up with candy.

## Features

- Configured for TypeScript Development (React.js, Next.js, Vue.js, Angular, Node.js etc.)
- Great default theme: [Tokyonight](https://github.com/folke/tokyonight.nvim)
- Lazy loaded via [lazy.nvim](https://github.com/folke/lazy.nvim)
- Highly performant (90ms load time)
- Extendable LSP configuration via [mason.nvim](https://github.com/williamboman/mason.nvim)
- Support for :robot: AI: [ChatGPT](https://openai.com/blog/chatgpt/), [GitHub Copilot](https://github.com/features/copilot), [Codeium](https://codeium.com/) and [Tabnine](https://www.tabnine.com/)
- Support for [TailwindCSS](https://tailwindcss.com/) with highlighted colors
- JSON autocompletion for most popular Frontend configs
- NPM packages autocompletion in _package.json_
- Internal [Jest](https://github.com/facebook/jest) testing and [Coverage](https://github.com/andythigpen/nvim-coverage) support
- Debugging with [nvim-dap](https://github.com/mfussenegger/nvim-dap) (works with React.js & React Native)
- Automatic Treesitter-based folding with imports folded by default
- Current code context via [nvim-navic](https://github.com/SmiteshP/nvim-navic)
- Beautiful and functional custom statusline built with [galaxyline.nvim](https://github.com/glepnir/galaxyline.nvim)
- Git management with [Lazygit](https://github.com/jesseduffield/lazygit), custom telescope commits view with [git-delta](https://github.com/dandavison/delta), [gitsigns](https://github.com/lewis6991/gitsigns.nvim) & [diffview](https://github.com/sindrets/diffview.nvim), custom git blame

And of course usage of [telescope](https://github.com/nvim-telescope/telescope.nvim), [nvim-tree](https://github.com/kyazdani42/nvim-tree.lua), [barbar](https://github.com/romgrk/barbar.nvim), [cmp](https://github.com/hrsh7th/nvim-cmp), [treesitter](https://github.com/nvim-treesitter/nvim-treesitter), [blankline](https://github.com/lukas-reineke/indent-blankline.nvim) & more!

## Screenshots

Dashboard

![Dashboard](https://raw.githubusercontent.com/wiki/doctorfree/CandyVim/screenshots/6-alpha.png)

Overview

![Neovim](https://raw.githubusercontent.com/wiki/doctorfree/CandyVim/screenshots/5-main.png)

[More screenshots](https://candyvim.lazyman.dev/screenshots)

## Installation

**Just clone GitHub repo into ~/.config/nvim-CandyVim**

**Prerequisities**

- Make sure you have installed the latest version of Neovim v0.9.0+ (nightly is preferred).
- Have wget, curl, unzip, git, make, pip, python, npm, node, luarocks, fd, ripgrep and cargo installed on your system. You can check if you are missing anything with `:checkhealth` command.
- Have any nerd font installed. _Fira Code_ has been used in screenshots. You can download it from [nerdfonts.com](https://www.nerdfonts.com/font-downloads).

**After install configuration:**

1. Selected treesitter Languages are installed by default.
   To check it run `:TSInstallInfo`.
   Make sure to run `:TSInstall <lang>` for specific language you want to install.
2. LSP servers are enabled by default. You can check installed LSP servers by `:Mason` command.

## Configuration

To change CandyVim related config use the `config/CandyVim.lua` file.

To change vim settings use the `config/options.lua` file.

To change plugin related settings use the specific `plugins/[name].lua` file. Some of the plugin config can be set up during plugin installation in `config/plugins.lua` file, where you can add new plugins.

## Keybindings

See the [Keymaps tab](https://candyvim.lazyman.dev/keymaps) for details on CandyVim key bindings.

Comma (,) is the default Leader key.

Check out the `which-key` menu and `keybindings.lua` for most used maps.

## Performance

Measured on M1.

CandyVim started in 91.13ms

## Future Todo

| **Description** | **Progress** |
| :-------------- | -----------: |
| Support more LSPs (not only frontend? - already possible via Mason)  | ![50%](https://progress-bar.dev/50/?title=progres)                 |
| Better configuration of additional LSPs (already possible via Mason) | ![50%](https://progress-bar.dev/50/?title=planned)                 |
| Project Logo                                                         | ![Planned](https://progress-bar.dev/0/?title=planned&color=b8860b) |
| Auto resize for more consistent UI behavior                          | ![Planned](https://progress-bar.dev/0/?title=planned&color=b8860b) |
| Reload in-time support                                               | ![Planned](https://progress-bar.dev/0/?title=planned&color=b8860b) |

| **Description** | **Progress** |
| :-------------- | -----------: |
| lazy.nvim instead of packer                     | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Better support for null-ls and local formatting | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Better support to project word refactor         | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Support for nvim-dap debugger for React         | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Support ESLint & Prettier in Native LSP         | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Replace coc-explorer with nvim-tree.lua         | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Replace coc.nvim with Native LSP                | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Change fzf.nvim to telescope.nvim               | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Update statusline to support LSP diagnostics    | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Rewrite most config to lua                      | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Support TailwindCSS with colors                 | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Provide current screenshots                     | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |
| Create shell installer for Linux & MacOS        | ![100%](https://progress-bar.dev/100/?title=done&color=555555) |

## Authors

- [\u0141ukasz Kurpiewski](https://github.com/ecosse3)
- [Ronald Record](https://github.com/doctorfree)

<div align="center">
  <p align="center">
    <a href="https://ronrecord.com" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="domain"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/domain.png"
    /></a>
    <a href="https://www.reddit.com/user/No-Blackberry-3160" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="reddit"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/reddit.png"
    /></a>
    <a href="https://github.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="github"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/github.png"
    /></a>
    <a href="https://gitlab.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="gitlab"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/gitlab.png"
    /></a>
    <a href="https://twitter.com/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="twitter"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/twitter.png"
    /></a>
    <a href="https://youtube.com/c/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="youtube"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/youtube.png"
    /></a>
    <a href="https://linkedin.com/in/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="linkedin"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/linkedin.png"
    /></a>
    <a href="https://instagram.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="instagram"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/instagram.png"
    /></a>
    <a href="https://noc.social/@doctorwhen" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="mastodon"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/mastodon.png"
    /></a>
    <a href="https://en.wikipedia.org/wiki/User:Doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="wikipedia"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/wikipedia.png"
    /></a>
  </p>
</div>
