# vim-ripgrep

## Usage

Search using ripgrep. The word under cursor will be searched if no argument is passed to `Rg`.

    :Rg <string|pattern>


Show root search dir:

    :RgRoot

## Installation


Using [Vim-Plug](https://github.com/junegunn/vim-plug):

Add this to your `~/.vimrc` and run `:PlugInstall`
```vim
Plug 'jremmen/vim-ripgrep'
```


Using [Vundle](https://github.com/VundleVim/Vundle.vim):

Add this to your `~/.vimrc` and run `:PluginInstall`
```vim
Plugin 'jremmen/vim-ripgrep'
```


Using [Pathogen](https://github.com/tpope/vim-pathogen):

Ensure you have `execute pathogen#infect()` in your `~/.vimrc` file and run:
```bash
git clone https://github.com/jremmen/vim-ripgrep.git ~/.vim/bundle
```

## Configuration


| Setting              | Default                   | Details
| ---------------------|---------------------------|----------
| g:rg_binary          | rg                        | path to rg
| g:rg_format          | %f:%l:%c:%m               | value of grepformat 
| g:rg_command         | g:rg_binary --vimgrep     | search command
| g:rg_highlight       | false                     | true if you want matches highlighted
| g:rg_derive_root     | false                     | true if you want to find project root from cwd
| g:rg_root_types      | ['.git']                  | list of files/dir found in project root
| g:rg_window_location | botright                  | quickfix window location
