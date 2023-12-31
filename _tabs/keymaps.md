---
layout: post
icon: fas fa-keyboard
order: 4
toc: true
post_style: page
---

## CandyVim Keybindings

Comma (,) is the default `Leader` key.

Check out the `which-key` menu and `lua/config/keybindings.lua` for most used maps.

### File Explorer

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| <C - e>      | Open File Explorer                            |
| Backspace    | Back to file explorer (in editor normal mode) |
| g?           | Open commands menu                            |
| a            | Create new file/directory                     |
| x            | Cut                                           |
| c            | Copy                                          |
| y            | Copy name                                     |
| r            | Rename                                        |
| I            | Toggle git ignore files                       |

### Searching

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| <C - p>      | Telescope git files |
| <S - p>      | Telescope live grep |
| s            | Enables lightspeed  |
| , s d        | Search dotfiles     |
| , s h        | Search file history |
| , s s        | Search history      |

### Working with LSP:

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| <C - Space> or , c a | Code action                                       |
| <S - K>              | Show documentation under cursor                   |
| gd                   | Go to definition                                  |
| gr                   | Go to references                                  |
| ]g                   | Go to next diagnostic                             |
| [g                   | Go to prev diagnostic                             |
| , c f                | Format document (usually ESLint/Prettier)         |
| , c r                | Rename                                            |
| , c q                | Quick fix - when I exactly know if it will fix it |
| , c d                | Local diagnostics list                            |
| , c o                | Organize imports                                  |

### Working with Git:

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| , g g        | Lazygit - for committing and branch change |
| , g s        | Telescope status - change/search file with git changes |
| ]c           | Go to next change hunk |
| [c           | Go to prev change hunk |
| , g d        | Advanced powerful diff view with many filters for debugging code, checking previous changes etc. |
| , g m        | View hunk diff of a line under cursor |
| , g h r      | Reset changed hunk under cursor -  check what changed in that line and type 'u' to go back |
| , g h s      | Stage hunk under cursor - stage specific lines and then just do a commit |
| , g l c      | Quick check of previous commit in current buffer, <C-s> inside to switch preview |
| , g w c      | Creates a new worktree. Recommended directory is `../path` |
| , g w w      | Switches to a worktree. <C-d> removes worktree. |

### Working with Project:

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| <C - e>      | Toggles nvim-tree file explorer |
| , p w        | Find word under cursor in project - find where component is used. Type '<'. |
| , p f        | Find file under cursor in project - find files which contain text under cursor.|
| , p t        | Finds TODOs/NOTES in project |
| , p l        | Switch between projects |
| , p s        | Save session to load it later from Dashboard |

### Commenting

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| gcc          | Create/remove comment      |
| gc (visual)  | Create/remove comment      |
| gcO          | Create comment line before |
| gco          | Create comment line after  |

### Table Mode / Alignment

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| ga (visual)  | Aligns selection based on separator (comma, semi-colon, colon etc.)               |
| , t m        | Enables Table Mode. Do it in markdown file with some table and you will see magic |
| , t i C      | (Only when Table Mode Enabled) Insert column before                               |
| , t i c      | (Only when Table Mode Enabled) Insert column after                                |
| , t d c      | (Only when Table Mode Enabled) Delete column                                      |
| , t d r      | (Only when Table Mode Enabled) Delete row                                         |
| , t s        | (Only when Table Mode Enabled) Sort table alphabetically                          |

### Eye Candy

| **Key Bindings** | **Description**   |
| :--------------- | ----------------: |
| `,Gg`        | Cellular automaton    |
| `,Gr`        | Make it rain          |
| `,Da`        | Hatch Crab            |
| `,Dc`        | Hatch Cat             |
| `,Dd`        | Hatch Duck            |
| `,Dg`        | Hatch Ghost           |
| `,Dh`        | Hatch Horse           |
| `,Di`        | Hatch Chick           |
| `,Ds`        | Hatch slow duck       |
| `,Dt`        | Hatch Dinosaur        |
| `,DA`        | Hatch All             |
| `,Dk`        | Cook Duck             |
| `,DK`        | Cook Many Ducks       |
| `,//`        | Alpha dashboard       |
| `,Gb`        | Blackjack game        |
| `,Gv`        | Play Vim be good      |
| `,Gs`        | Play Sudoku           |
| `,Ga`        | Hack auto typing mode |
| `,Gf`        | Hack current buffer   |
| `,Gh`        | Hack fake buffer      |

### Other VERY useful bindings

| **Key Bindings** | **Description** |
| :--------------- | --------------: |
| <S - q>      | Smartly closes current buffer without breaking UI |
| <C - a>      | Increase number, switch between true/false/const/let/function/arrow function/increment dates etc. |
| <C - n>      | Finds next occurrence of word and puts multi-cursor there. [Read more](https://github.com/mg979/vim-visual-multi/wiki) |
| <C - o>      | Jumps to previous cursor in jumplist. I use it very often. |
| v <ENTER>    | Smartly selects next subjects of current treesitter context |
| s            | Standalone jump to any word with `folke/flash.nvim` |
| ciq          | Change inside ANY quotes (``or '' or "" etc.) with`mini.ai` |
| cib          | Change inside ANY brackets ({} or [] or () etc.) with `mini.ai` |
| za           | Toggle folds. LSP and nvim-ufo automatically add to supported files in smart way. |
| zM           | Close all folds |
| zR           | Open all folds |
| zr           | Open all folds except imports/comments |
| gJ           | Smartly joins lines based on treesitter |
| gS           | Smartly splits lines based on treesitter |
| < F12 >      | Opens/closes terminal |
| ~            | Switch function arguments smartly |
