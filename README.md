# CDD

cdd is a zsh command to move the directory that supports Tmux, Screen and multi session

## Installation

### Using zgen

Include the load command in your .zshrc

```
zgen load yuki-ycino/cdd
zgen save
```

### Using zplug

Load cdd as a plugin in your .zshrc

```
zplug "yuki-ycino/cdd"
```

### Using Antigen

Bundle cdd in your .zshrc

```
antigen bundle yuki-ycino/cdd
antigen apply
```

## Settings

Add the following lines to your .zshrc:

```
chpwd_functions+=_cdd_chpwd
```

## Usage

With no argument, move to the last directory moved

### Completion
```
$ cdd<Tab>
[cdd directory]
1.1                        ==>  ~/repos/github.com/hoge/hoge
1.2                        ==>  ~/repos/github.com/hoge/fuga
1.4   1.5                  ==>  ~/repos/github.com/hoge/hogefuga
2.1   5.3                  ==>  ~
2.2                        ==>  ~/Downloads/
3.1   7.1  1.3  3.3        ==>  ~/dotfiles
3.4                        ==>  ~/backup
last  3.2                  ==>  ~/repos/github.com/yuki-ycino/cdd
[cdd command]
add      ==>  add the directory to ~/.cdd
delete   ==>  delete the directory from ~/.cdd
```

Read:

* http://m4i.hatenablog.com/entry/2012/01/26/064329
* https://github.com/m4i/cdd
