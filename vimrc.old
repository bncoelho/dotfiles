
call pathogen#infect()
syntax on
filetype plugin indent on

let g:solarized_termtrans = 1
colorscheme solarized
call togglebg#map("<F5>")

" Yank text to the OS X clipboard"
noremap <leader>y "*y
noremap <leader>yy "*Y

" Preserve indentation while pasting text from the OS X clipboard"
noremap <leader>p :set paste<CR>:put  *<CR>:set nopaste<CR>


let g:Powerline_theme="solarized256"
let g:Powerline_colorscheme="solarized256"
let g:Powerline_symbols = 'fancy'
set guifont=Monaco-Powerline
set encoding=utf-8

set number
set incsearch
set ruler


set softtabstop=2
let mapleader = ","

"highlight OverLength ctermbg=red ctermfg=white guibg=#592929"
"match OverLength /\%100v.\+/"

" Highlight long lines {{{
function HighlightLongLines()
    let w:highlight_long_lines
        \ = exists('w:highlight_long_lines') ?
        \ ! w:highlight_long_lines : 1
    if w:highlight_long_lines
        let w:m1=matchadd('Search', '\%<97v.\%>93v', -1)
        let w:m2=matchadd('ErrorMsg', '\%>96v.\+', -1)
    else
        call matchdelete(w:m1)
        call matchdelete(w:m2)
    endif
endfunction
" Enable it by default in all windows
"au BufWinEnter * call HighlightLongLines()
" Map it to <F3>
nnoremap <silent> <F3> :call HighlightLongLines()<CR>
"}}}

autocmd FileType ruby map <F9> :w<CR>:!ruby -c %<CR>
