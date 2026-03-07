# Green Ocean on Fasm + Ocaml
Has syntax, compiler, indent & theme support on Neovim.

### Preview 
![alt](https://github.com/thetrung/green-ocean.vim/blob/main/preview.png)

### Create `green-fasml.lua` in `../lua/plugins/`
```lua
vim.filetype.add({
  extension = {
    asm = "fasm",
    inc = "fasm",
  },
})
return {
  "thetrung/green-fasml.vim",
}
```
This also set syntax on `*.asm` & `*.inc` for FASM.

### Config as Default 
this usually need on `Arch/Omarchy` where `colorscheme` is synced by theme, add this to your `init.lua` :
```lua
    vim.defer_fn(function()
      vim.cmd("colorscheme green-ocean")
    end, 50)
```
 
## Based on:

fasm syntax :
https://github.com/fedorenchik/fasm.vim

colorscheme :
https://github.com/thetrung/green-fasm.vim
