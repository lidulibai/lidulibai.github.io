---
title: SPF13-vimProfiles
date: 2017-05-14 00:10:45
tags:
---

## .vimrc.local
    let g:airline_powerline_fonts=1
    let g:EclimCompletionMethod='omnifunc'
    " let g:EclimMavenPomClasspathUpdate=0
    let g:EclimFileTypeValidate=0
    let g:spf13_no_autochdir=1

    " eclimd {
            if isdirectory(expand("~/.vim/eclim/"))
                nmap <leader>ji :JavaImport<CR>
                nnoremap <silent> <buffer> <leader>jd :JavaDocSearch -x declarations<CR>
                nnoremap <silent> <buffer> <leader>jc :JavaSearchContext<CR>
            endif
    " }

## .vimrc.before.local
    se nospell
    let g:spf13_noninvasive_completion=1
    " let g:spf13_no_autochdir=1
    let g:spf13_bundle_groups=['general', 'writing', 'programming', 'php', 'neocomplete', 'ruby', 'python', 'javascript', 'html', 'misc', 'youcompleteme']

## .vimrc.bundles.local
    " Bundle 'phongvcao/vim-stardict'
