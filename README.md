# My Vim/NeoVim Configuration

A simple vim-related configuration for basic file editing.

## Files

* `.ideavimrc` for IdeaVim : symbolic link to `~/.ideavimrc`
* `.vimrc` for Vim : symbolic link to `~/.vimrc`

  ``` bash
  cd && rm .vimrc
  ln -s vime/.vimrc .vimrc
  ```

* ~~`init.vim` for NeoVim : symbolic link to `~/.config/nvim/init.vim`~~

* `config/` : the root directory of configuration files
  * `plugins/` : contain separate configuration files for each plugin
  * `themes/` : contain separate configuration files for each theme
  * `args.vim` : set path variables
  * `base.vim` : a basic configuration for Vim
  * `keymaps.vim` : set key mapping
  * `plugin-list.vim` : the plugin list of vim-plug

## Usage

1. Install [NeoVim](https://github.com/neovim/neovim)
2. Install Node.js
3. `git clone git@github.com:imkasen/vime.git`
4. `cd ~/.config/ && rm -rf ./nvim/`
5. `ln -s ~/vime/ ./nvim/`
6. Install [vim-plug](https://github.com/junegunn/vim-plug)
7. Install plugins

## Plugins

* themes
  * [nightfox.nvim](https://github.com/EdenEast/nightfox.nvim)
  * ~~[github-nvim-theme](https://github.com/projekt0n/github-nvim-theme)~~
* plugins
  * [coc.nvim](https://github.com/neoclide/coc.nvim)
    * [coc-marketplace](https://github.com/fannheyward/coc-marketplace)
    * [coc-clangd](https://github.com/clangd/coc-clangd)
    * [coc-go](https://github.com/josa42/coc-go)
    * [coc-highlight](https://github.com/neoclide/coc-highlight)
  * ~~[indentLine](https://github.com/Yggdroot/indentLine)~~
  * [vim-airline](https://github.com/vim-airline/vim-airline)
  * [auto-pairs](https://github.com/jiangmiao/auto-pairs)
  * ~~[nerdcommenter](https://github.com/preservim/nerdcommenter)~~
  * ~~[vim-cpp-enhanced-highlight](https://github.com/octol/vim-cpp-enhanced-highlight)~~
  * [rainbow](https://github.com/luochen1990/rainbow)
