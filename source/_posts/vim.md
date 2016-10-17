---
title: vim
date: 2016-10-15 11:16:22
tags:
---
> Install Vim
```
    sudo dnf install vim
```

> Enviroment : Fedora22+, Git 1.7, vim 7.3+
```
    sh <(curl https://j.mp/spf13-vim3 -L)
```
> Make some personal change
```
    * echo 'let g:airline_powerline_fonts=1' > .vimrc.local
    
    * echo 'let g:spf13_noninvasive_completion=1' > .vimrc.before.local
    * echo 'let g:spf13_no_autochdir=1' > .vimrc.before.local
```

