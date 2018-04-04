# nvim Error

```
[deoplete] deoplete failed to load: Vim(call):E117: Unknown function: _deoplete. Try the :UpdateRemotePlugins command and restart Neovim. See also :CheckHealth.
Press ENTER or type command to continue
```

* check if both python2 and python3 are properly installed/linked
* run in Neovim `:CheckHealth`

## nvim config
```
let g:python_host_prog  = '/usr/bin/python2'
let g:python3_host_prog  = '/usr/local/bin/python3'
```

## properly install python
```
brew install python@2
brew install python@3

brew info python
brew info python2
brew info python3

python -V
python2 -V
python3 -V

/usr/local/bin/python2
/usr/local/bin/python3
```

## neovim setup

https://github.com/zchee/deoplete-jedi/wiki/Setting-up-Python-for-Neovim
