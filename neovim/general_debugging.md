# NeoVim Debugging 

**NeoVim debugging**

```
set log level and catch log file
export NVIM_PYTHON_LOG_FILE=/tmp/log
export NVIM_PYTHON_LOG_LEVEL=DEBUG
nvim -u main.go
nvim -u minimal.vimrc
```

source:
* https://github.com/Shougo/deoplete.nvim/issues/481


**Vim Debug-Mode**
```
vim help
:h debug-mode

start in debugger mode
nvim -D tmp.txt

show .vimrc loaded scriptnames
:scriptnames
```

source:
* https://www.gilesorr.com/blog/vim-debugger.html
* https://sanctum.geek.nz/arabesque/debugging-vim-setup/

**debugging a vim command**
```
:breakadd here // add breakpoint
:breaklist // show breakpoints
:debug LivedownPreview // execute command in debug-mode
```

further vim debugging information:
* http://albertogrespan.com/blog/debugging-your-vimrc/


