php-doc
=======
This php-doc file is an extension of Tobias Schlitt's. 
What I've added is the ability to create a doc block for the file as php code sniffer throws errors
when you dont have a phpdoc block for the file.

just go on the line of your opening php tag and enter your shortkey to create the doc block 
for me it is ctl+p. Keep in mind that you have to set up your php doc block in your vimrc file

    here is the sample of mine.
    <code>
    " PHP options
:function! PhpDocLoad()
:   source $HOME/.vim/php-doc.vim
:   inoremap <C-P><ESC> :call PhpDocSingle()<CR>i
:   nnoremap <C-P> :call PhpDocSingle()<CR>
:   vnoremap <C-P> :call PhpDocRange()<CR>
:   inoremap ( ()<Left>
:endfunction

</code>
