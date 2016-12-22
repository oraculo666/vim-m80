# vim-m80

This is a simple [Vim](http://www.vim.org) plugin to highlight 8080 and Z80 assembly code based on Microsoft's [MACRO-80](http://www.msxarchive.nl/pub/msx/programming/asm/m80l80.txt) assembler and the [Z80](https://www.scribd.com/document/282095677/um0080) processor documentations. It still has no advanced preprocessor highlighting rules but is should already do the basics like opcodes and directives keyword highlighting as well as numbers, strings and comments.

## Install
* [Vundle](https://github.com/gmarik/vundle)
    * add the following to your vundle config:
    * `Plugin 'oraculo666/vim-m80'`
    * run `:PluginInstall` in Vim command mode.

The plugin should automatically recognize '.mac' files.

## Mappings
* Insert Mode
    * `<leader>-` - Inserts a full line comment separator

## Notes
* The `colorcolumn` is set to 132 as a reminder since the real M-80 can't process lines longer than that.
* `fileformat` set to `dos`. M-80 doesn't support unix line endings.
* `fileencoding` set to `latin1`. Extended ASCII character encoding.
* Tabs set at 8 spaces. Identifiers can be long but only the first 6 characters are significant.

## Screenshots
![MSX assembly code](https://i.sli.mg/uUEIV6.png)
_MSX Z80 assembly code (Molokai color scheme)_

![Highlights](https://i.sli.mg/Uxjals.png)
_Some highlighting features_

