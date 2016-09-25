# vim-ripgrep

    :Rg <string|pattern>

## configuration


| Setting          | Default                   | Details
| -----------------|---------------------------|----------
| g:rg_binary      | rg                        | path to rg
| g:rg_format      | %f:%l:%c:%m               | value of grepformat 
| g:rg_command     | <g:rg_binary> --vimgrep   | search command
| g:rg_derive_root | false                     | true if you want to find project root from cwd
| g:rg_root_types  | ['.git']                  | list of files/dir found in project root
    
## misc

Show root search dir

    :RgRoot
