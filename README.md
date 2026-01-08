# Green Ocean on Fasm + Ocaml
Has syntax, compiler, indent & theme support on Neovim.

### Preview 
![alt](https://github.com/thetrung/green-ocean.vim/blob/main/preview.png)

### Set Flat Assembler syntax by default for `*.asm` files

Add following to your `autocmds.lua` or `init.lua` on NeoVim :

```
autocmd BufReadPre *.asm let g:asmsyntax = "fasm"
```

### Create `green-fasml.lua` in `../plugins`

```
return {
  "thetrung/green-fasml.vim",
}
```

### Config as Default 
this usually need on `Arch/Omarchy` where `colorscheme` is synced by theme, add this to your `init.lua` :
```
    vim.defer_fn(function()
      vim.cmd("colorscheme green-ocean")
    end, 50)
```
 
## Based on:

### fasm support :

https://github.com/fedorenchik/fasm.vim

### colorscheme :

https://github.com/thetrung/green-fasm.vim
