# vpkg

Vundle and vim-plug etc are bloated.

Vpkg is a vim plugin ~~manager~~ helper written in under 50 lines of posix shell using vim's built-in package system.

## Installation 

This is just a helper script, put it anywhere you want _(preferably somewhere in your $PATH)_.

You should probably have

```vim
set nocompatible              
filetype plugin on 
```

in your vimrc. 

### Dependencies

* vim 7.4+
* git

## Usage 

`vpkg -i user repo` install a plugin

`vpkg -r repo` remove a plugin 

`vpkg -u` update plugins

`vpkg -l` list plugins 

### Post-install

Post install, update, remove actions can be configured with environment variables:

`POSTI`

`POSTR`

`POSTU`

## TODO 

- [x] update all the plugins
- [ ] better argument handling 
- [ ] update plugins simultaneously 
- [x] post-install
- [ ] install multiple plugins at once
