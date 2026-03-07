# Green Ocean on Fasm + Ocaml
Has syntax, compiler, indent & theme support on Neovim.

### Preview 
![alt](https://github.com/thetrung/green-ocean.vim/blob/main/preview.png)

### Create `green-fasml.lua` in neovim configs in `../plugins`
* this also Set `*.asm` & `*.inc` for FASM.
  
```
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
