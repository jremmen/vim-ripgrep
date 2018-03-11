# vim-ripgrep

    :Rg <string|pattern>

Word under cursor will be searched if no argument is passed to `Rg`

## configuration


| Setting              | Default                   | Details
| ---------------------|---------------------------|----------
| g:rg_binary          | rg                        | path to rg
| g:rg_format          | %f:%l:%c:%m               | value of grepformat 
| g:rg_command         | g:rg_binary --vimgrep     | search command
| g:rg_highlight       | false                     | true if you want matches highlighted
| g:rg_derive_root     | false                     | true if you want to find project root from cwd
| g:rg_root_types      | ['.git']                  | list of files/dir found in project root
| g:rg_window_location | botright                  | quickfix window location
    
## misc

Show root search dir

    :RgRoot
