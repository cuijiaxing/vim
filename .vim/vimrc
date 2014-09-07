
" 在vim 启动的时候默认开启 NERDTree(autocmd可以缩写为au)
"autocmd VimEnter * NERDTree

"按下F2调出/隐藏 NERDTree
map <silent> <F2> :NERDTreeToggle<CR>

"将NERDTree 的窗口设置在vim窗口的右侧(默认为左侧)
let NERDTreeWinPos="left"
"在新tab中打开文件
"let NERDTreeMapOpenInTab='<ENTER>'

" 当打开NERDTree 窗口时, 自动显示Bookmarks
let NERDTreeShowBookmarks=1

"语法高亮
syntax on
"设置背景为浅色
colorscheme railscasts

"设置(软)制表符宽度为4
set tabstop=4
set softtabstop=4

"设置缩进的空格数为4
set shiftwidth=4

"设置自动缩进：即每行的缩进值与上一行相等; 使用noautoindent取消设置
set autoindent

"显示行号
set nu


"突出显示当前行
set cursorline
hi CursorLine cterm=NONE ctermbg=lightgrey ctermfg=white guibg=lightgrey guifg=white

"打开状态栏标尺
"set ruler

"关闭错误信息响铃
set noerrorbells

"配置多语言环境
if has("multi_byte")
"UTF-8编码
set encoding=utf-8
set termencoding=utf-8
set formatoptions+=mM
set fencs=utf-8,gbk
endif

if v:lang =~?'^\(zh\)\|\(ja\)\|\(ko\)'
set ambiwidth=double
endif

"Python 文件的一般设置, 比如不要tab等
autocmd FileType python set tabstop=4 shiftwidth=4 softtabstop=4 expandtab
autocmd FileType python map <F5> :!python %<CR>


"set ctags
set tags=./tags

"set omni and key mapping
filetype plugin on
set omnifunc=syntaxcomplete#Complete
highlight Pmenu ctermbg=238 gui=bold
highlight PmenuSel ctermbg=54 gui=bold

"补全完成后关闭tip提示窗
"autocmd CursorMovedI * if pumvisible() == 0|pclose|endif
"autocmd InsertLeave * if pumvisible() == 0|pclose|endif
"disable preview window
set completeopt-=preview

"use supertab
let g:SuperTabDefaultCompletionType = "context"

