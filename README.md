# vim-config
My current vim optimizations for 🎨 and better ⌨️ experience.

![alt Vim after applying optimizations](https://github.com/jdredman/vim-config/blob/main/vim-optimized.png?raw=true)

Add the followint to your `~/.vimrc` (if you dont have this file you may have to create it) and customize to your preferences.

```vim
" Show line and character numbers
set number
set ruler

" Auto indent by filetype
if has('filetype')
  filetype indent on
endif

" Keep same indent on return when theres no auto indent
set autoindent

" Set color scheme 
" Options -> default, blue, darkblue, delek, desert, elford, evening, 
" industry, koehler, morning, murphy, pablo, peachpuff, ron, shine,
" slate, torte, zellner
colorscheme slate

" Enable syntax highlighting
if has('syntax')
  syntax on
endif

" Reduce indentation width
set shiftwidth=4
set tabstop=4

" Make comments gray
hi comment ctermfg=darkgray

" Ask to save on exit
set confirm

" Show error nudge rather than audio
set visualbell

" Vim command autocomplete
set wildmenu

" Redraw only when needed
set lazyredraw

" Highlight character matches ([{}])
set showmatch

" Search while typing
set incsearch

" Highlight search matches
set hlsearch

" remap leader to comma for easier reach
let mapleader=","

" Key binding for easier clearing of search highlighting
nnoremap <leader><space> :nohlsearch<CR>

" Enable use of mouse for input
if has('mouse')
  set mouse=a
endif
```
