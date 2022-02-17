# My NeoVim/Vim Configuration

A simple vim-related configuration for basic file editing. ~~（人生苦短，还是用 VS Code 吧）~~

* Vim: set some basic configuration and key bindings
* NeoVim: add plugins and their settings in addition to the above configuration

## Usage

1. Install [NeoVim](https://github.com/neovim/neovim)

   ``` Bash
   curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
   chmod u+x nvim.appimage
   ```

2. Install Node.js (required by `coc.nvim`)
3. Install [nvime](https://github.com/imkasen/nvime)

   ``` Bash
   cd && git clone git@github.com:imkasen/nvime.git
   cd ~/.config/ && rm -rf ./nvim/
   ln -s ~/nvime ./nvim
   ```

4. Install [vim-plug](https://github.com/junegunn/vim-plug)
5. Install [plugins](#Plugins)

## File Structure

* `.ideavimrc` for IdeaVim : symbolic link to `~/.ideavimrc`
* `.vimrc` for Vim : symbolic link to `~/.vimrc`

  ``` bash
  cd && rm .vimrc
  ln -s nvime/.vimrc .vimrc
  ```

* `init.vim` for NeoVim : ~~symbolic link to `~/.config/nvim/init.vim`~~
* `autoload/` : this directory is used for autoloading, some common functions are here.
* `config/` : the root directory of configuration files
  * `editors/` : contain separate configuration files for each editor
  * `other/` : other configuration files, e.g. `coc-settings.json`
  * `plugins/` : contain separate configuration files for each plugin, files are named as `<plugin_name>.vim`
  * `args.vim` : set path variables
  * `base.vim` : a basic configuration for Vim
  * `keymaps.vim` : set key mapping
  * `plugin-list.vim` : the plugin list of `vim-plug`

## Plugins

* themes
  * [nightfox.nvim](https://github.com/EdenEast/nightfox.nvim)
  * ~~[github-nvim-theme](https://github.com/projekt0n/github-nvim-theme)~~
* plugins
  * [coc.nvim](https://github.com/neoclide/coc.nvim)
    * [coc-marketplace](https://github.com/fannheyward/coc-marketplace)
    * [coc-clangd](https://github.com/clangd/coc-clangd)
    * [coc-cmake](https://github.com/voldikss/coc-cmake)
    * [coc-css](https://github.com/neoclide/coc-css)
    * [coc-eslint](https://github.com/neoclide/coc-eslint)
    * [coc-go](https://github.com/josa42/coc-go)
    * [coc-highlight](https://github.com/neoclide/coc-highlight)
    * [coc-markdownlint](https://github.com/fannheyward/coc-markdownlint)
    * [coc-json](https://github.com/neoclide/coc-json)
    * [coc-pyright](https://github.com/fannheyward/coc-pyright)
    * [coc-sh](https://github.com/josa42/coc-sh)
    * [coc-vimlsp](https://github.com/iamcco/coc-vimlsp)
    * [coc-xml](https://github.com/fannheyward/coc-xml)
    * [coc-yaml](https://github.com/neoclide/coc-yaml)
  * ~~[indentLine](https://github.com/Yggdroot/indentLine)~~
  * [vim-airline](https://github.com/vim-airline/vim-airline)
  * [vim-airline-themes](https://github.com/vim-airline/vim-airline-themes)
  * [auto-pairs](https://github.com/jiangmiao/auto-pairs)
  * [nerdcommenter](https://github.com/preservim/nerdcommenter)
  * ~~[vim-cpp-enhanced-highlight](https://github.com/octol/vim-cpp-enhanced-highlight)~~
  * [rainbow](https://github.com/luochen1990/rainbow)

## Reference

* [vime](https://github.com/fgheng/vime)
