# Settings for VIM

This is the settings I personally used for VIM. This settting is often used for
VIM on bash terminal, usually for C / C++ programming languages.

## Initial setups
Most likely, you will need to install VIM on bash. Go to 
```bash
cd /etc/vim
sudo vi vimrc
```
and add the following lines for personal settings
```
set nocompatible
filetype on
filtype plugin on
filetype indent on
syntax on
set number
set shiftwidth=4
set tabstop=4
set expandtab
set noback
set nowrap
set showmode
" maybe the following lines
set showmatch
set hlsearch
```

for colour, molokai is something I quite like, but you will need to install this. First.
go to 
```bash
cd /usr/share/vim/vim**/colors
```
where ** means vim version. Once you get to here, type in the following command:
```bash
curl -o molokai.vim https://raw.githubusercontent.com/tomasr/molokai/master/colors/molokai.vim
```
and then go back to vimrc file written above, and add
```bash
:colorscheme molokai
```
