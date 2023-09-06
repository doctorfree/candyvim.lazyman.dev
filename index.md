---
layout: post
title: CandyVim Neovim Configuration
toc: true
post_style: page
---

<h2 align="center">CandyVim Neovim Configuration</h2>

An Eye Candy Neovim config built to work most efficiently with Frontend Development

This is based on
[Ecovim](https://github.com/ecosse3/nvim){:target="_blank"}{:rel="noopener noreferrer"}
with a lot of useless eye candy thrown in to demonstrate how useful Neovim is
even loaded up with candy.

**[Note:]** the default namespace for the
[Lazyman configuration](https://lazyman.dev/info/Lazyman.html) is now `ecovim`
which is an enhanced version of `CandyVim`.

## Features

- Configured for TypeScript Development (React.js, Next.js, Vue.js, Angular, Node.js etc.)
- Great default theme: [Tokyonight](https://github.com/folke/tokyonight.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Lazy loaded via [lazy.nvim](https://github.com/folke/lazy.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Highly performant (90ms load time)
- Extendable LSP configuration via [mason.nvim](https://github.com/williamboman/mason.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Support for :robot: AI: [ChatGPT](https://openai.com/blog/chatgpt/){:target="_blank"}{:rel="noopener noreferrer"}, [GitHub Copilot](https://github.com/features/copilot){:target="_blank"}{:rel="noopener noreferrer"}, [Codeium](https://codeium.com/){:target="_blank"}{:rel="noopener noreferrer"} and [Tabnine](https://www.tabnine.com/){:target="_blank"}{:rel="noopener noreferrer"}
- Support for [TailwindCSS](https://tailwindcss.com/){:target="_blank"}{:rel="noopener noreferrer"} with highlighted colors
- JSON autocompletion for most popular Frontend configs
- NPM packages autocompletion in _package.json_
- Internal [Jest](https://github.com/facebook/jest){:target="_blank"}{:rel="noopener noreferrer"} testing and [Coverage](https://github.com/andythigpen/nvim-coverage){:target="_blank"}{:rel="noopener noreferrer"} support
- Debugging with [nvim-dap](https://github.com/mfussenegger/nvim-dap){:target="_blank"}{:rel="noopener noreferrer"} (works with React.js & React Native)
- Automatic Treesitter-based folding with imports folded by default
- Current code context via [nvim-navic](https://github.com/SmiteshP/nvim-navic){:target="_blank"}{:rel="noopener noreferrer"}
- Beautiful and functional custom statusline built with [galaxyline.nvim](https://github.com/glepnir/galaxyline.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Git management with [Lazygit](https://github.com/jesseduffield/lazygit){:target="_blank"}{:rel="noopener noreferrer"}, custom telescope commits view with [git-delta](https://github.com/dandavison/delta){:target="_blank"}{:rel="noopener noreferrer"}, [gitsigns](https://github.com/lewis6991/gitsigns.nvim){:target="_blank"}{:rel="noopener noreferrer"} & [diffview](https://github.com/sindrets/diffview.nvim){:target="_blank"}{:rel="noopener noreferrer"}, custom git blame

And of course usage of [telescope](https://github.com/nvim-telescope/telescope.nvim){:target="_blank"}{:rel="noopener noreferrer"}, [nvim-tree](https://github.com/kyazdani42/nvim-tree.lua){:target="_blank"}{:rel="noopener noreferrer"}, [barbar](https://github.com/romgrk/barbar.nvim){:target="_blank"}{:rel="noopener noreferrer"}, [cmp](https://github.com/hrsh7th/nvim-cmp){:target="_blank"}{:rel="noopener noreferrer"}, [treesitter](https://github.com/nvim-treesitter/nvim-treesitter){:target="_blank"}{:rel="noopener noreferrer"}, [blankline](https://github.com/lukas-reineke/indent-blankline.nvim){:target="_blank"}{:rel="noopener noreferrer"} & more!

## Screenshots

Dashboard

![Dashboard](https://raw.githubusercontent.com/wiki/doctorfree/CandyVim/screenshots/6-alpha.png)

Overview

![Neovim](https://raw.githubusercontent.com/wiki/doctorfree/CandyVim/screenshots/5-main.png)

[More screenshots](https://candyvim.lazyman.dev/screenshots)

## [Installation](https://candyvim.lazyman.dev/install)

See the [Install tab](https://candyvim.lazyman.dev/install) for installation instructions.

## Configuration

To change CandyVim related config use the `config/CandyVim.lua` file.

To change vim settings use the `config/options.lua` file.

To change plugin related settings use the specific `plugins/[name].lua` file. Some of the plugin config can be set up during plugin installation in `config/plugins.lua` file, where you can add new plugins.

## [Keybindings](https://candyvim.lazyman.dev/keymaps)

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

- [Łukasz Kurpiewski](https://github.com/ecosse3){:target="_blank"}{:rel="noopener noreferrer"}
- [Ronald Record](https://github.com/doctorfree){:target="_blank"}{:rel="noopener noreferrer"}

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
