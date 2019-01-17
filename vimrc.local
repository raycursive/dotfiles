syntax on
filetype off
set ts=4
set shiftwidth=4
set softtabstop=4
set smartcase
set expandtab
set fileencodings=utf-8
set number
set showmatch
set mouse=a
set selection=exclusive
set selectmode=mouse,key
set hlsearch
set cursorline
set cursorcolumn
set scrolloff=5
set splitbelow
set splitright

set hidden

noremap H ^
noremap L $
" cnoremap <C-a> <Home>
" cnoremap <C-e> <End>

" Disable <C-a>
" nmap <C-a> <Nop>
map <C-A> ggVG$

nnoremap # *
nnoremap * #

let g:python_host_prog='/home/zhangxinyu/.local/virtualenvs/neovim2/bin/python'
let g:python3_host_prog='/home/zhangxinyu/.local/virtualenvs/neovim3/bin/python'
call plug#begin()
Plug 'Valloric/YouCompleteMe'
" Plug 'Shougo/deoplete.nvim', { 'do': ':UpdateRemotePlugins' }
" Plug 'zchee/deoplete-jedi'
Plug 'bronson/vim-trailing-whitespace'
Plug 'majutsushi/tagbar'
Plug 'bling/vim-airline'
Plug 'vim-airline/vim-airline-themes'
Plug 'scrooloose/nerdcommenter'
Plug 'scrooloose/nerdtree'
Plug 'kshenoy/vim-signature'
Plug 'Yggdroot/indentLine'
Plug 'flazz/vim-colorschemes'
Plug 'morhetz/gruvbox'
Plug 'airblade/vim-gitgutter'
Plug 'jceb/vim-orgmode'
Plug 'tpope/vim-speeddating'
Plug 'terryma/vim-smooth-scroll'
Plug 'icymind/NeoSolarized'
Plug 'altercation/vim-colors-solarized'
Plug 'vim-ctrlspace/vim-ctrlspace'
Plug 'tpope/vim-surround'
Plug 'plytophogy/vim-virtualenv'
Plug 'tmhedberg/SimpylFold'
Plug 'vim-scripts/indentpython.vim'
" Plug 'hdima/python-syntax'
" Plug 'integralist/vim-mypy'
Plug 'kana/vim-textobj-user'
Plug 'kana/vim-textobj-indent'
call plug#end()

filetype plugin indent on

" Airline
set laststatus=2
let g:airline_powerline_fonts = 1
let g:airline#extensions#tabline#enabled = 1
let g:airline#extensions#tabline#tab_nr_type = 1
let g:airline#extensions#tabline#show_tab_nr = 1
let g:airline#extensions#tabline#formatter = 'default'

" NERDSpace
let g:NERDSpaceDelims = 1

" ColorScheme
colorscheme gruvbox
set background=dark
set termguicolors
highlight Normal ctermbg=none guibg=none
if has("gui_vimr")
    " colorscheme NeoSolarized
    colorscheme gruvbox
    " colorscheme solarized8_dark_flat
endif

" YCM
set completeopt=menu,menuone
let g:ycm_add_preview_to_completeopt = 0
nnoremap <leader>gd :YcmCompleter GoToDefinitionElseDeclaration<CR>
let g:ycm_key_invoke_completion = '<C-n>'
let g:ycm_python_binary_path = '/home/zhangxinyu/.local/virtualenvs/tsf3/bin/python'

" Deoplete
" let g:deoplete#enable_at_startup = 1
" set completeopt=menu,menuone

" TagBar
nmap <leader>t :TagbarToggle<CR>
let g:tagbar_autofocus = 1

" NERDTree
nmap <leader>e :NERDTreeToggle<CR>

" Nohl
nnoremap <leader>h :noh<CR>

" GitGutter
nmap <leader>g :GitGutterLineHighlightsToggle<CR>
nmap <leader>gn :GitGutterNextHunk<CR>
nmap <leader>gp :GitGutterPrevHunk<CR>

" Pastetoggle & interact with system clipboard
set pastetoggle=<leader>v
" " Copy to clipboard
vnoremap  <leader>y  "+y
nnoremap  <leader>Y  "+yg_
nnoremap  <leader>y  "+y
nnoremap  <leader>yy  "+yy
" " Paste from clipboard
nnoremap <leader>p "+p
nnoremap <leader>P "+P
vnoremap <leader>p "+p
vnoremap <leader>P "+P

" Smooth scroll
noremap <silent> <c-u> :call smooth_scroll#up(&scroll, 0, 2)<CR>
noremap <silent> <c-d> :call smooth_scroll#down(&scroll, 0, 2)<CR>
noremap <silent> <c-b> :call smooth_scroll#up(&scroll*2, 0, 4)<CR>
noremap <silent> <c-f> :call smooth_scroll#down(&scroll*2, 0, 4)<CR>

" CtrlSpace
" let g:CtrlSpaceDefaultMapping = 0
let g:CtrlSpaceDefaultMappingKey = "<c-p>"
" noremap <silent> <c-p> :CtrlSpace <CR>
" noremap <silent> <c-p> :CtrlSpace O<CR>
let g:CtrlSpaceLoadLastWorkspaceOnStart = 1
let g:CtrlSpaceSaveWorkspaceOnSwitch = 1
let g:CtrlSpaceSaveWorkspaceOnExit = 1

set foldmethod=indent
set foldlevel=99
let g:SimplyFold_docstring_preview=1
