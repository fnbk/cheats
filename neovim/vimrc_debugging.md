# debugging NeoVim plugins

## Go Plugin

**:Gvdiff**

```
call s:command("-bang -bar -nargs=* -complete=customlist,s:EditComplete Gvdiff :execute s:Diff('keepalt vert ',<bang>0,<f-args>)")
function! s:Diff(vert,keepfocus,...) abort
```

https://github.com/tpope/vim-fugitive/blob/master/plugin/fugitive.vim

```
:h autoload, :h <sid>, :h script-local
```

https://vi.stackexchange.com/questions/3732/vimscript-help-with-autoloading-scope-sid


## fixing vim-livedown plugin

**prozess finden, der port 1337 nutzt**
```
lsof -i tcp:1337
lsof -i -P -n // zeigt mehr informationen an
```

**livedown**
```
livedown start "/Users/florian/primary/go/src/bitbucket.scm.otto.de/scm/primary/notes/vim_debugging.md" --open --port 1337 --browser "'google chrome'"
```

links:
* https://github.com/shime/livedown
* https://github.com/shime/vim-livedown
