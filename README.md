# Green Ocean on Fasm + Ocaml

Has syntax, compiler, indent & theme support on Neovim.

## Set Flat Assembler syntax by default for `*.asm` files

Add following to your `autocmds.lua` or `init.lua` on NeoVim :

```
autocmd BufReadPre *.asm let g:asmsyntax = "fasm"
```
 
## Based on:

### fasm support :

https://github.com/fedorenchik/fasm.vim

### colorscheme :

https://github.com/thetrung/green-fasm.vim
