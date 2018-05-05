# config for tmux and vim

## tmux

config `tmux.conf`

### Fast Pane-Switching

I want to be able to simply say M-<direction> to go where I want to go (remember: M is for Meta, which is usually your Alt key). With this modification I can simply press Alt-left to go to the left pane (and other directions respectively)

### Mouse mode

Enable mouse mode to make it easier to change block panel text, etc.

### Sane Split Commands

use `Ctrl+b Shift+|` for vertical and use `Ctrl+b Shift+_` for horizontal

### Getting 256 colors

Getting 256 colors terminal inside tmux

### change color

Changing the colors and design of tmux

### block and copy with mouse

block the text dont release the mouse and press enter to copy use `Ctrl+shift+v` to paste

## vim

- install vim and plugin follow instruction on http://moelove.info/vim/
- change the to dracula
- add custom commands

```
" esc alternative
imap jj <Esc>
cmap jj <c-c>

" exit virtual map
vmap v <Esc>

" leave shift to get : just press ;
map ; :

" Switch between the last two files
let g:mapleader=','
nnoremap <leader><leader> <c-^>

" Every unnecessary keystroke that can be saved is good for your health :)
nnoremap <C-H> <C-W><C-H>
nnoremap <C-J> <C-W><C-J>
nnoremap <C-K> <C-W><C-k>
nnoremap <C-L> <C-W><C-L>

" Display extra whitespace
set list listchars=tab:»·,trail:·

```

Credits:

- http://moelove.info/vim/
- https://draculatheme.com/vim/
- https://github.com/rizafahmi/dotfiles/blob/master/neovim/init.vim
- https://www.hamvocke.com/blog/a-guide-to-customizing-your-tmux-conf/
